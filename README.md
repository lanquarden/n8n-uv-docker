# n8n-uv Docker Image

This repository contains a custom Docker image for [n8n](https://n8n.io/) with additional tools for installing uv/uvx based MCP servers.

## Features

- Based on the official `n8n` Docker image.
- Pre-installed [Astral uv/uvx](https://astral.sh/uv/).

## Usage

To pull and run the Docker image:

```bash
# Replace <version> with the desired version tag
docker pull ghcr.io/lanquarden/n8n-uv:<version>
docker run -p 5678:5678 ghcr.io/lanquarden/n8n-uv:<version>
```

## Building the Image

To build the Docker image locally:

```bash
docker buildx -t n8n-uv --build-arg VERSION=<version> .
```

## Publishing to GitHub Container Registry

This repository includes a GitHub Actions workflow to automatically build and publish the Docker image to `ghcr.io` upon demand

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.