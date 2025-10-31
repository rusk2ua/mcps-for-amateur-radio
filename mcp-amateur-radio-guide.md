# MCP Servers for Amateur Radio Development

A comprehensive guide to Model Context Protocol (MCP) servers useful for non-programmers developing VHF/UHF/SHF and EME Amateur Radio software and websites.

## Table of Contents

- [Recommended MCP Servers](#recommended-mcp-servers)
- [Configuration Documentation by IDE/Tool](#configuration-documentation-by-idetool)
- [Additional Resources](#additional-resources)
- [Configuration File Locations](#configuration-file-locations)

## Recommended MCP Servers

| MCP Server | Purpose | Why Useful for Amateur Radio |
|---|---|---|
| **Filesystem** | Access and manage local files and directories | Essential for reading/writing configuration files, log files, and working with radio control software files |
| **Sequential Thinking** | Extended reasoning and problem-solving | Helps break down complex RF propagation calculations, antenna design problems, and EME path loss analysis |
| **Memory** | Store and retrieve information across sessions | Keep track of satellite passes, QSO details, station configurations, and project progress |
| **Brave Search** | Web search capabilities | Research propagation reports, look up callsigns, find technical specifications for radios and antennas |
| **Fetch** | Retrieve web page content | Pull real-time propagation data, check band conditions, access repeater databases and Amateur Radio resources |
| **GitHub** | Repository management | Store and version control your software projects, access existing Amateur Radio code repositories |
| **SQLite** | Database operations | Manage QSO logs, contact databases, repeater frequencies, and EME scheduling information |
| **Time** | Current time and timezone info | Critical for EME scheduling, satellite tracking, contest logging with accurate UTC timestamps |
| **Google Maps** | Location and mapping data | Calculate beam headings, distances for grid square calculations, and visualize coverage areas |
| **Everything** | Access to multiple integrated tools | Combines file, web, and data operations for comprehensive development workflow |

### Key Recommendations for Your Use Case

- **Start with**: Filesystem, Memory, and Brave Search
- **For EME work**: Add Time and Google Maps for precise scheduling and bearing calculations
- **For website development**: Include Fetch to pull live propagation data and band conditions
- **For logging software**: SQLite is essential for managing contacts and QSO databases

## Configuration Documentation by IDE/Tool

### Claude Desktop

| MCP Server | Documentation URL |
|---|---|
| Filesystem | https://modelcontextprotocol.io/docs/develop/connect-local-servers |
| Filesystem | https://support.claude.com/en/articles/10949351-getting-started-with-local-mcp-servers-on-claude-desktop |
| General MCP | https://www.anthropic.com/engineering/desktop-extensions |
| GitHub | https://www.docker.com/blog/connect-mcp-servers-to-claude-desktop-with-mcp-toolkit/ |
| Sequential Thinking | https://www.docker.com/blog/connect-mcp-servers-to-claude-desktop-with-mcp-toolkit/ |
| Multiple Servers | https://www.mcplist.ai/blog/setup-mcp-server-claude-desktop/ |

### Cursor IDE

| MCP Server | Documentation URL |
|---|---|
| Filesystem | https://docs.cursor.com/context/model-context-protocol |
| GitHub | https://docs.cursor.com/context/model-context-protocol |
| Multiple Servers | https://snyk.io/articles/how-to-add-a-new-mcp-server-to-cursor/ |
| Composio (100+ servers) | https://composio.dev/blog/how-to-connect-cursor-to-100-mcp-servers-within-minutes |
| liblab MCP | https://liblab.com/docs/mcp/howto-connect-mcp-to-cursor |

### Windsurf IDE

| MCP Server | Documentation URL |
|---|---|
| General MCP | https://docs.windsurf.com/windsurf/cascade/mcp |
| Filesystem | https://windsurf.com/university/tutorials/configuring-first-mcp-server |
| PostgreSQL | https://apidog.com/blog/windsurf-mcp-servers/ |
| GitHub | https://natoma.ai/blog/how-to-enabling-mcp-in-windsurf |
| Zapier | https://actions.zapier.com/docs/platform/windsurf/ |
| liblab MCP | https://liblab.com/docs/mcp/howto-connect-mcp-to-windsurf |

### VS Code

| MCP Server | Documentation URL |
|---|---|
| General MCP | https://code.visualstudio.com/docs/copilot/chat/mcp-servers |
| MCP Developer Guide | https://code.visualstudio.com/api/extension-guides/ai/mcp |
| Agent Mode Servers | https://code.visualstudio.com/mcp |
| General Setup | https://medium.com/towards-agi/how-to-set-up-and-use-vscode-mcp-server-352c1e6f42e9 |
| Agent Mode + MCP | https://code.visualstudio.com/blogs/2025/05/12/agent-mode-meets-mcp |
| Composio (100+ servers) | https://composio.dev/blog/how-to-add-100-mcp-servers-to-vs-code-in-minutes |

### Visual Studio 2022

| MCP Server | Documentation URL |
|---|---|
| General MCP | https://learn.microsoft.com/en-us/visualstudio/ide/mcp-servers?view=vs-2022 |

### Universal Resources (All Tools)

| Resource | Documentation URL |
|---|---|
| Official Spec | https://modelcontextprotocol.io/quickstart/server |
| Official Introduction | https://www.anthropic.com/news/model-context-protocol |
| GitHub Registry | https://github.com/modelcontextprotocol |
| MCP Directory/Gallery | https://www.mcplist.ai/ |
| Smithery (MCP Discovery) | https://smithery.ai |
| OpenTools MCP Discovery | https://opentools.com/ |
| Windsurf MCP Hub | https://windsurf.run/ |

## Additional Resources

### Tutorials and Guides

| Resource Type | URL | Description |
|---|---|---|
| MCP Tutorial | https://www.datacamp.com/tutorial/mcp-model-context-protocol | Comprehensive MCP guide with demo project |
| MCP Complete Guide | https://medium.com/@nimritakoul01/the-model-context-protocol-mcp-a-complete-tutorial-a3abe8a7f4ef | Complete MCP tutorial with architecture details |
| Troubleshooting | https://www.danliden.com/posts/20250412-mcp-quickstart.html | FastMCP server setup and debugging |
| Custom MCP Server | https://apidog.com/blog/build-a-custom-mcp-server/ | Build custom MCP servers for Cursor |
| Docker MCP Setup | https://www.docker.com/blog/connect-mcp-servers-to-claude-desktop-with-mcp-toolkit/ | Using Docker for MCP servers |

## Configuration File Locations

### Claude Desktop

- **macOS**: `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows**: `%APPDATA%\Claude\claude_desktop_config.json`

### Cursor

- **Global**: `~/.cursor/mcp.json`
- **Project**: `.cursor/mcp.json`

### Windsurf

- **Configuration**: `~/.codeium/windsurf/mcp_config.json`

### VS Code

- **Workspace**: `.vscode/mcp.json`
- **User**: User profile configuration via Command Palette

---

## Contributing

This guide is designed for Amateur Radio operators developing software for VHF/UHF/SHF and EME applications. If you have additional MCP servers or resources that would be useful for the Amateur Radio community, please feel free to contribute.

## License

This document is provided as-is for the Amateur Radio community. Feel free to share and modify as needed.

## About MCP

The Model Context Protocol (MCP) is an open protocol that standardizes how applications provide context to Large Language Models (LLMs). It enables AI assistants to securely access tools, data sources, and services while maintaining user control and privacy.

---

**73, Rus, K2UA**

*Last Updated: October 31, 2025*
