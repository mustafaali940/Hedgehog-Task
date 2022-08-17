## creating Docker compose using 3 Tier


version: '2'
services:
  fe:
    image: kammana/emp-fe-comp:1.0
    container_name: emp-fe
    ports:
     - "4200:4200"
    networks:
     -javahome-app
mongodb:
  container_name: empapi

