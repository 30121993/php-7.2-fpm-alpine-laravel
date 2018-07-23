# PHP 7.2 FPM Docker definition

This is based on the [laradock Dockerfile](https://github.com/laradock/laradock/blob/master/php-fpm/Dockerfile) but with the following changes:
 * removed all the optional features for speed
 * includes composer so we can bundle our source, run a composer install and ship the image to ECR with no further steps required
 * mcrypt php extension
 * mailparse php extension
 * bash - may be removed shortly
 * mysql-client - may be removed shortly 

Available on Dockerhub here: [netfiradev/php-7.2-fpm-alpine-laravel-ready](https://hub.docker.com/r/netfiradev/php-7.2-fpm-alpine-laravel-ready/)  