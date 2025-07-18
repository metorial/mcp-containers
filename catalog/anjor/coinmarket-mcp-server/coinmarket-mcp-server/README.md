
# Coinmarket MCP server

A containerized version of "Coinmarket MCP server"

> Repository: [anjor/coinmarket-mcp-server](https://github.com/anjor/coinmarket-mcp-server)

## Description

An MCP server that integrates with the Coinmarket API


## Usage

The containers are built automatically and are available on the GitHub Container Registry.

1. Pull the Docker image:

```bash
docker pull ghcr.io/metorial/mcp-container--anjor--coinmarket-mcp-server--coinmarket-mcp-server
```

2. Run the container:

```bash
docker run -i --rm \ 
-e COINMARKET_API_KEY=coinmarket-api-key \
ghcr.io/metorial/mcp-container--anjor--coinmarket-mcp-server--coinmarket-mcp-server  "coinmarket_service"
```

- `--rm` removes the container after it exits, so you don't have to clean up manually.
- `-i` allows you to interact with the container in your terminal.



### Configuration

The container supports the following configuration options:




#### Environment Variables

- `COINMARKET_API_KEY`




## Usage with Claude

```json
{
  "mcpServers": {
    "coinmarket-mcp-server": {
      "command": "docker",
      "args": [
        "run",
        "-i",
        "--rm",
        "ghcr.io/metorial/mcp-container--anjor--coinmarket-mcp-server--coinmarket-mcp-server",
        "coinmarket_service"
      ],
      "env": {
        "COINMARKET_API_KEY": "coinmarket-api-key"
      }
    }
  }
}
```

# License

Please refer to the license provided in [the project repository](https://github.com/anjor/coinmarket-mcp-server) for more information.

## Contributing

Contributions are welcome! If you notice any issues or have suggestions for improvements, please open an issue or submit a pull request.

<div align="center">
  <sub>Containerized with ❤️ by <a href="https://metorial.com">Metorial</a></sub>
</div>
  