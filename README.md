# vlt Docker Image

This project provides a Docker image that includes the vlt client from Hashicorp. The vlt client is used to interact with Vault, a tool for securely accessing secrets. For more information on the commands available with the vlt client, please refer to the [official documentation](https://developer.hashicorp.com/hcp/docs/vault-secrets/commands).

## Docker Hub Repository

The Docker image for this project is available on Docker Hub: [artnie/vlt](https://hub.docker.com/r/artnie/vlt).

## Usage

You can pull the image from Docker Hub and run it as follows:

```sh
docker pull artnie/vlt
docker run --rm -it artnie/vlt --help
```

## Local Development

If you want to build and run the Docker image locally, you can use the following commands:

#### Build the Docker Image

```sh
docker build -t local_vlt_image .
```

#### Run the Docker Image

```sh
docker run --rm -it --name local_vlt_container local_vlt_image --version
```

These commands will build the Docker image with the tag local_vlt_image and then run it in a container named local_vlt_container, displaying the version of the vlt client installed in the image.