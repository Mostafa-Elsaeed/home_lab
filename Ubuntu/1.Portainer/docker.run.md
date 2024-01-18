docker run -d \
  --name portainer \
  --restart always \
  -p 9000:9000 \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -v /mnt/HDD/AppsData/portianer/data:/data \
  --network main_network \
  --volume portainer_data:/data \
  portainer/portainer-ce:latest