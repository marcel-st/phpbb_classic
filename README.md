# Docker image for legacy PHPBB versions

##
This docker container is created to supply a Centos 6 image that is pre-configured to host a legacy PHPBB forum. It is not recommended that you use legacy versions, but if you must.....

## Usage

 docker create \
  --name phpbb_classic \
  -v </path/to/your/webroot>:/var/www/html \
  -p 80:80 \
  lgalastacia/phpbb_classic 

## Parameters

- --name : Give the docker container a logical name
- -v : map a local location to a location in the container
- -p : map network ports
