## create composer container for build symfony app
<!-- services:
  installer:
    image: composer:latest
    volumes:
      - ./:/app
    working_dir: /app
    ports:
      - 8000:8000 -->
## run command for build container and deleted
 docker-compose run --rm --service-ports installer bash

 ## install symfony
curl -sS https://get.symfony.com/cli/installer | bash

export PATH="$HOME/.symfony5/bin:$PATH"


symfony new my_project_directory --version="6.3.*" --webapp

## config git ()
  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"