# ci-cd-optimizer-agent
Intelligent CI/CD Pipeline Optimiser &amp; Auto-Tuner

## Power BI Modeling MCP Server

This repository includes a VS Code MCP configuration (`.vscode/mcp.json`) for the [Power BI Modeling MCP Server](https://github.com/microsoft/powerbi-modeling-mcp), which lets GitHub Copilot Chat interact with Power BI semantic models (Power BI Desktop, Fabric workspaces, or PBIP projects).

### Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/download)
- [GitHub Copilot Chat](https://marketplace.visualstudio.com/items?itemName=GitHub.copilot-chat) extension
- [Node.js](https://nodejs.org/en) (used by `npx` to download the MCP server on first run)

### Usage

1. Open this repository in VS Code.
2. Open GitHub Copilot Chat and confirm **powerbi-modeling-mcp** is listed as an available tool/server (it is auto-detected from `.vscode/mcp.json`). If it isn't available, ensure the "MCP servers in Copilot" setting is enabled for your GitHub account/organization.
3. Connect to a semantic model using natural language, for example:
   - `Connect to '[File Name]' in Power BI Desktop`
   - `Connect to semantic model '[Semantic Model Name]' in Fabric Workspace '[Workspace Name]'`
   - `Open semantic model from PBIP folder '[Path to the definition/TMDL folder]'`
4. Ask Copilot Chat to perform modeling changes (e.g., rename fields, add descriptions, refactor measures, translate the model, or validate DAX).

> [!WARNING]
> Always back up your semantic model before letting an AI agent make changes, and be cautious about sharing chat sessions since responses may include sensitive model data.
