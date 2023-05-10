# docker-media-server-rspbr

# Docker Media Server for Raspberry Pi

![Raspberry Pi with media server](raspberry-pi-media-server.jpg)

This repo contains a set of Docker Compose configuration files to set up a media server on a Raspberry Pi (or other Linux machine). The Docker containers included in this set of files allow for streaming of multimedia content from sources such as Plex, Sonarr, Radarr, Lidarr, and Jackett.

## Prerequisites

- Docker and Docker Compose should be installed on your Raspberry Pi or Linux machine. Follow the instructions below to install them:

### Installing Docker

1. Update your package index: `sudo apt-get update`
2. Install Docker: `sudo apt-get install docker.io`
3. Start the Docker service: `sudo systemctl start docker`
4. Set Docker to start on boot: `sudo systemctl enable docker`

### Installing Docker Compose

1. Download the latest version of Docker Compose: `sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`
2. Make the downloaded file executable: `sudo chmod +x /usr/local/bin/docker-compose`
3. Verify that Docker Compose was installed correctly: `docker-compose --version`

## Installation

1. Clone this repo to your Raspberry Pi or Linux machine.
2. Modify the configuration files to suit your needs.
3. Run `docker-compose up -d` from the root directory of the repo to start the containers.
4. Access the media server via the URLs of the various components (e.g. http://localhost:32400/web for Plex).

## Configuration

Each container included in this repo has its own configuration file that can be edited to customize its behavior. These files are located in the `config` directory of the repo.

## Usage

Once the containers are up and running, you can begin adding multimedia content to the media server. Each container has its own set of instructions for adding content, which can be found in their respective documentation.

## Support

If you encounter any issues while using this media server setup, please open an issue on the Github repo.

## Contributing

If you would like to contribute to this project, please fork the repo and submit a pull request with your changes.
