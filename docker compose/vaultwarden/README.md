To generate ADMIN TOKEN for Vaultwarden run command below in ssh session in OMV. 

docker run --rm -it vaultwarden/server /vaultwarden hash

if permission is denied ad ssh-user to docker-user group first with command below

sudo usermod -aG docker username

remove the ' from hashed token and replace the $ with $$

YouTube link: https://youtu.be/cT4Aeu1w5CQ showing vaultwarden.yml file being used with openmediavault

Docker Hub link: https://hub.docker.com/r/vaultwarden/server

Vaultwarden wiki: https://github.com/dani-garcia/vaultwarden/wiki

CHANGE_TO_COMPOSE_DATA_PATH is a parameter used in openmediavault to specify the default container appdata path.
