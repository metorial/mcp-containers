
# Desktop Commander MCP

A containerized version of "Desktop Commander MCP"

> Repository: [wonderwhy-er/DesktopCommanderMCP](https://github.com/wonderwhy-er/DesktopCommanderMCP)

## Description

Search, update, manage files and run terminal commands with AI


## Usage

The containers are built automatically and are available on the GitHub Container Registry.

1. Pull the Docker image:

```bash
docker pull ghcr.io/metorial/mcp-container--wonderwhy-er--desktopcommandermcp--desktop-commander-mcp
```

2. Run the container:

```bash
docker run -i --rm \ 
ghcr.io/metorial/mcp-container--wonderwhy-er--desktopcommandermcp--desktop-commander-mcp  "npm run start"
```

- `--rm` removes the container after it exits, so you don't have to clean up manually.
- `-i` allows you to interact with the container in your terminal.




## Usage with Claude

```json
{
  "mcpServers": {
    "desktop-commander-mcp": {
      "command": "docker",
      "args": [
        "run",
        "-i",
        "--rm",
        "ghcr.io/metorial/mcp-container--wonderwhy-er--desktopcommandermcp--desktop-commander-mcp",
        "npm run start"
      ],
      "env": {}
    }
  }
}
```

# License

Please refer to the license provided in [the project repository](https://github.com/wonderwhy-er/DesktopCommanderMCP) for more information.

## Contributing

Contributions are welcome! If you notice any issues or have suggestions for improvements, please open an issue or submit a pull request.

<div align="center">
  <sub>Containerized with ❤️ by <a href="https://metorial.com">Metorial</a></sub>
</div>
  