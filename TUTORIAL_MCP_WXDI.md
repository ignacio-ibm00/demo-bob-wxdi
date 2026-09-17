# Cómo agregar el MCP de Watsonx.data Intelligence (WxDI) a Bob

### 1. Requisito previo
Tener instalado **uv**:
```bash
# macOS / Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# Windows
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

---

### 2. Configurar `.bob/mcp.json`
Agrega el servidor en el archivo `.bob/mcp.json` de tu proyecto:

```json
{
  "mcpServers": {
    "wxdi-mcp-server": {
      "command": "uvx",
      "args": [
        "ibm-watsonx-data-intelligence-mcp-server",
        "--transport",
        "stdio"
      ],
      "env": {
        "DI_SERVICE_URL": "https://api.ca-tor.dai.cloud.ibm.com",
        "DI_APIKEY": "<TU_APIKEY>",
        "DI_ENV_MODE": "SaaS",
        "LOG_FILE_PATH": "/tmp/di-mcp-server-logs"
      },
      "disabled": false
    }
  }
}
```

---

### 3. Recargar y Probar
1. Recarga la ventana de tu IDE / Bob para inicializar el MCP.
2. Pídele a Bob:
   > *"Consulta los términos de negocio y linaje de datos en Watsonx Data Intelligence"*
