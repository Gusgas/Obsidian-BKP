---  
services:  
  jellyseerr:  
    image: ghcr.io/fallenbagel/jellyseerr:latest  
    init: true  
    container_name: jellyseerr  
    environment:  
      - LOG_LEVEL=debug  
      - TZ=Asia/Tashkent  
    network: patopatoso  
    ports:  
      
      - 5055:5055  
    volumes:  
      - jellyseerr-data:/app/config  
    healthcheck:  
      test: wget --no-verbose --tries=1 --spider http://localhost:5055/api/v1/status || exit 1  
      start_period: 20s  
      timeout: 3s  
      interval: 15s  
      retries: 3  
    restart: unless-stopped  
  
volumes:  
  jellyseerr-data:  
    external: true