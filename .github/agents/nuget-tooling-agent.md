---
name: nuget-tooling-agent
description: An agent that additionally has access to the nuget MCP tools
mcp-servers:
  nuget-mcp-server-via-agent:
    type: 'local'
    command: 'dnx'
    args: ['NuGet.Mcp.Server@1.1.19', '--yes']
    tools: ['*']
---

# NuGet Tooling Agent

This is an agent that has access to NuGet MCP tools via a local MCP server that can be used to perform various NuGet related tasks. Other functionality of the underlying agent remains unchanged.