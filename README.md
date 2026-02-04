# docker-test                                                                                                                                                                           
                                                                                                                                                                                          
  Test project for Docker + Caddy load balancing. A Caddy reverse proxy distributes requests across two backend servers (`caddy1`, `caddy2`) using round-robin.                           
                                                                                                                                                                                          
  ## Usage                                                                                                                                                                                

  ```sh
  docker build -t docker-test .

  Files

  - Caddyfile -- reverse proxy config (listens on localhost:80)
  - Dockerfile -- base image (debian:stable-slim)
  - index1.html / index2.html -- pages served by each backend
