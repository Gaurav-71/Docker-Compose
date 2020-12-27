# Operating System Assignment 2020

To create a Docker-compose yaml for the following Multi-container app (Drupal postgres)

## Container 1 (front-end)

  Front-end image - drupal:8-apache
  
  Container port - 80
  
  volumes 
          - /var/www/html/modules

          - /var/www/html/profiles

          - /var/www/html/themes

          - /var/www/html/sites

## Container 2 (database)

  Back-end image - postgres:10
  
  environment variable -  POSTGRES_PASSWORD: example

Note: Bring up both the containers on same user defined bridge network

# Docker Commands

  docker pull drupal

  docker pull postgres
  
  docker-compose config

  docker-compose up -d

  docker-compose down

  docker-compose ps
