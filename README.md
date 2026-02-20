# Awesome MCP DevTools [![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

[![Discord](https://img.shields.io/discord/1312302100125843476?logo=discord&label=discord)](https://glama.ai/mcp/discord)
[![Subreddit subscribers](https://img.shields.io/reddit/subreddit-subscribers/mcp?style=flat&logo=reddit&label=subreddit)](https://www.reddit.com/r/mcp/)

A curated list of developer tools, SDKs, libraries, utilities, and resources for working with **Model Context Protocol (MCP)** servers.

> [!IMPORTANT]
> Browse [MCP servers](https://glama.ai/mcp/servers)

## Contents

- [Awesome MCP DevTools ](#awesome-mcp-devtools-)
  - [Contents](#contents)
  - [Community](#community)
  - [Legend](#legend)
  - [SDKs](#sdks)
    - [JavaScript/TypeScript](#javascripttypescript)
    - [Python](#python)
    - [Java](#java)
    - [Go](#go)
    - [Rust](#rust)
    - [Kotlin](#kotlin)
    - [C#/.NET](#cnet)
    - [Scala](#scala)
    - [Dart](#dart)
    - [Ruby](#ruby)
    - [Elixir](#elixir)
    - [C/C++](#cc)
    - [Swift](#swift)
    - [Bash](#bash)
  - [Frameworks](#frameworks)
  - [Testing Tools](#testing-tools)
    - [Authorization Testing](#authorization-testing)
  - [Libraries](#libraries)
  - [Utilities](#utilities)
    - [Proxies and Gateways](#proxies-and-gateways)
    - [Development Tools](#development-tools)
  - [Hosting](#hosting)
  - [Templates](#templates)
  - [Resources](#resources)
  - [Tutorials](#tutorials)
  - [Related awesome lists:](#related-awesome-lists)

---

## Community

* [r/mcp Reddit](https://www.reddit.com/r/mcp)
* [Discord Server](https://glama.ai/mcp/discord)

## Legend

* 🎖️ official MCP resource
* programming language
  * #️⃣ - C# Codebase
  * 〽️ – Scala codebase
  * ☕ - Java codebase
  * 🎯 - Dart codebase
  * 🏎️ – Go codebase
  * 🐍 – Python codebase
  * 💎 – Ruby codebase
  * 📇 – TypeScript codebase
  * 🔶 - Kotlin codebase
  * 🦀 – Rust codebase
  * 🌊 – C/C++ codebase
  * 🍎 – Swift codebase
  * 💧 – Elixir codebase
  * 👾 – Bash codebase

## SDKs

> Software Development Kits for MCP server development.

<details><summary>How are SDKs ordered?</summary>

SDKs are ordered by their popularity as determined by GitHub stars.

If an SDK is part of a monorepo, it should have a name in the form of `github-owner/github-repo#project-name`.

If an SDK is part of a monorepo, its popularity is counted as 0 stars.
</details>

### JavaScript/TypeScript

- [FastMCP](https://github.com/punkpeye/fastmcp) 📇 - A high-level framework for building MCP servers in TypeScript
- [QuantGeekDev/mcp-framework](https://github.com/QuantGeekDev/mcp-framework) 📇 - Fast and elegant TypeScript framework for building MCP servers
- [wong2/LiteMCP](https://github.com/wong2/litemcp) 📇 - A high-level framework for building MCP servers in JavaScript/TypeScript
- [ModelFetch](https://github.com/phuctm97/modelfetch) 📇 - A runtime-agnostic SDK to create and deploy MCP servers anywhere TypeScript/JavaScript runs
- [ribeirogab/simple-mcp](https://github.com/ribeirogab/simple-mcp) 📇 - A simple TypeScript library for creating MCP servers
- [firebase/genkit#mcp](https://github.com/firebase/genkit/tree/main/js/plugins/mcp) 📇 – Provides integration between [Genkit](https://github.com/firebase/genkit/tree/main) and the Model Context Protocol (MCP)
- [MCPcat](https://github.com/mcpcat/mcpcat-typescript-sdk) 📇 - User analytics, session tracking, and live debugging for MCPs
- [Mastra AI](https://github.com/mastra-ai/mastra) 📇 - Mastra is a Typescript-based AI agent framework that can be used to author MCP servers.

### Python

- [FastMCP](https://github.com/jlowin/fastmcp) 🐍 - A high-level framework for building MCP servers in Python
- [mcp-use](https://github.com/mcp-use/mcp-use) 🐍 - Open source python library to very easily connect any LLM to any MCP server both locally and remotely.
- [langchain-mcp](https://github.com/rectalogic/langchain-mcp) 🐍 - Provides MCP tool calling support in LangChain
- [tadata-org/fastapi_mcp](https://github.com/tadata-org/fastapi_mcp) 🐍 - Provides MCP wrapping on top of existing FastAPI REST endpoints
- [easymcp](https://github.com/promptmesh/easymcp) 🐍 - A high level asyncio native client SDK with native support for namespaced servers and caching.
- [mcp-cli](https://github.com/tileshq/mcp-cli) 🐍 - A lightweight CLI MCP client to connect with remote MCP servers.
- [MCPcat](https://github.com/mcpcat/mcpcat-python-sdk) 🐍 - User analytics, session tracking, and live debugging for MCPs
- [basementstudio/xmcp](http://github.com/raw-labs/mxcp) 🐍 - Open-source framework for building secure, testable, enterprise-grade MCP tools from SQL or Python on top of dbt + DuckDB.

### Java

- [quarkus-mcp-server](https://github.com/quarkiverse/quarkus-mcp-server) ☕ - Java SDK for building MCP servers using Quarkus
- [spring-ai-mcp](https://github.com/spring-projects-experimental/spring-ai-mcp) ☕ - Java SDK and Spring Framework integration for building MCP client and MCP servers
- [tinystruct-mcp](https://github.com/tinystruct/tinystruct-mcp) ☕ - Java SDK and establishing an extensible MCP server based on lightweight tinystruct framework
  
### Go

- [ggoodman/mcp-server-go](https://github.com/ggoodman/mcp-server-go) 🏎️ - Build MCP servers that scale from a 20‑line stdio prototype to a horizontally scaled, OIDC‑protected streaming HTTP deployment — without rewriting business logic.
- [mark3labs/mcp-go](https://github.com/mark3labs/mcp-go) 🏎️ - Golang SDK for building MCP Servers and Clients
- [metoro-io/mcp-golang](https://github.com/metoro-io/mcp-golang) 🏎️ - Golang framework for building MCP Servers, focussed on type safety
- [strowk/foxy-contexts](https://github.com/strowk/foxy-contexts) 🏎️ - Golang library to write MCP Servers declaratively with functional testing included

### Rust

- [linux-china/mcp-rs-template](https://github.com/linux-china/mcp-rs-template) 🦀 - MCP CLI server template for Rust
- [Epistates/TurboMCP](https://github.com/Epistates/turbomcp) 🦀 - TurboMCP SDK: Enterprise MCP SDK
- [poem-web/poem#poem-mcpserver](https://github.com/poem-web/poem/tree/master/poem-mcpserver) 🦀 - MCP Server implementation for Poem

### Kotlin

- [http4k MCP SDK](https://mcp.http4k.org) 🔶 - Functional, testable Kotlin SDK based around the popular [http4k](https://http4k.org) Web toolkit

### C#/.NET

- [salty-flower/ModelContextProtocol.NET](https://github.com/salty-flower/ModelContextProtocol.NET) #️⃣ - A C# SDK for building MCP servers on .NET 9 with NativeAOT compatibility ⚡ 🔌

### Scala

- [mullerhai/sakura-mcp](https://github.com/mullerhai/sakura-mcp) 〽️ - Scala MCP Framework for Building effective agents with MCP servers and clients

### Dart

- [leehack/mcp_dart](https://github.com/leehack/mcp_dart/) 🎯 - This library aims to provide a simple and intuitive way to implement MCP servers and clients in Dart 

### Ruby

- [modelcontextprotocol/ruby-sdk](https://github.com/modelcontextprotocol/ruby-sdk) 💎 🎖️ - Official Ruby SDK for building MCP servers
- [tidewave-ai/tidewave_rails](https://github.com/tidewave-ai/tidewave_rails) 💎 - Ruby on Rails MCP, speed up development with AI assistants that understand your web application, how it runs, and what it delivers

### Elixir

- [tidewave-ai/tidewave_phoenix](https://github.com/tidewave-ai/tidewave_phoenix) 💧 - Phoenix MCP, speed up development with AI assistants that understand your web application, how it runs, and what it delivers

### C/C++

- [micl2e2/mcpc](https://github.com/micl2e2/mcpc) 🌊 - Modern C SDK for building MCP servers/clients.

### Swift

- [modelcontextprotocol/swift-sdk](https://github.com/modelcontextprotocol/swift-sdk) 🍎 🎖️ - Official Swift SDK for building with MCP.

### Bash

- [yaniv-golan/mcp-bash-framework](https://github.com/yaniv-golan/mcp-bash-framework) 👾 - Zero-dependency Bash implementation for building MCP servers, supporting features like tool handling, schema validation, progress streaming, and cross-platform compatibility.



## Frameworks

> High-level frameworks for working with MCP servers

- [cordum-io/cordum](https://github.com/cordum-io/cordum) 🏎️ – Agent orchestration platform with a native MCP server and security built in: gRPC safety kernel for policy evaluation before tool execution, output scanning for PII/secrets/injection, full audit trail, multi-tenant isolation, and CAP protocol with ECDSA verification.
- [hasmcp/hasmcp-ce](https://github.com/hasmcp/hasmcp-ce) 🤖📇🏎️ - Convert your API to MCP server with built-in authentication, authorization, real-time request/response logs and metrics. HasMCP is a no-code, self-hosted API to MCP server bridge.
- [lastmile-ai/mcp-agent](https://github.com/lastmile-ai/mcp-agent) 🤖 🔌 - Build effective agents with MCP servers using simple, composable patterns
- [mcpdotdirect/template-mcp-server](https://github.com/mcpdotdirect/template-mcp-server) 📇 - A CLI tool to create a new MCP server project with TypeScript support
- [p-funk/FEGIS](https://github.com/p-funk/FEGIS) 🐍 - A semantic programming framework for LLMs that compiles YAML archetypes into structured tools with built-in memory and meaning. Each interaction becomes part of an emergent knowledge graph, enabling persistent, semantic retrieval and reuse.
- [sebastianbuzdugan/framework-rai-mcp](https://github.com/sebastianbuzdugan/framework-rai-mcp) 📇 - A responsible AI MCP server framework focused on ethical deployment in startups and enterprise prototypes.
- [sendaifun/solana-agent-kit#agent-kit-mcp-server](https://github.com/sendaifun/solana-agent-kit/tree/main/examples/agent-kit-mcp-server) - Solana MCP SDK
- [stephencme/create-mcp-ts](https://github.com/stephencme/create-mcp-ts) 📇 - Create a new MCP server in TypeScript, batteries included - supports user-defined templates!
- [Upsonic/gpt-computer-assistant](https://github.com/Upsonic/gpt-computer-assistant) 🐍 – Framework to build vertical AI agent
- [microsoft/semantic-kernel](https://github.com/microsoft/semantic-kernel) 🐍 #️⃣ – Enterprise-ready orchestration framework MCP compatible from Microsoft to build intelligent AI agents and multi-agent systems.
- [xmcp](https://github.com/basementstudio/xmcp) 📇 - A TypeScript framework with file-system routing & complete toolkit

## Testing Tools 
> Tools for testing MCP servers and clients 

- [mclenhard/mcp-evals](https://github.com/mclenhard/mcp-evals) 🤖 - Package and Github action for running evals. 
- [mcpjam/inspector](https://github.com/MCPJam/inspector) - Testing and debugging MCP servers.
- [modelcontextprotocol/inspector](https://github.com/modelcontextprotocol/inspector) 📇 🎖️ - UI for testing MCP servers.
- [wong2/mcp-cli](https://github.com/wong2/mcp-cli) 🤖 - Command line inspector for manual testing
- [muppet-kit/inspector](https://github.com/muppet-dev/kit) - MCP Inspector with AI-assisted debugging and testing capabilities.
- [loopwork-ai/Companion](https://github.com/loopwork-ai/Companion) - Companion is a utility for testing and debugging your MCP servers on macOS, iOS, and visionOS.
- [greynewell/mcpbr](https://github.com/greynewell/mcpbr) 🐍 - Benchmark runner for evaluating MCP server performance and agentic capabilities.

### Authorization Testing
> Resources for testing MCP servers with authentication and authorization

- [NapthaAI/http-oauth-mcp-server](https://github.com/NapthaAI/http-oauth-mcp-server) 📇 - Example implementation of a remote MCP server with OAuth authentication
- [modelcontextprotocol/python-sdk](https://github.com/modelcontextprotocol/python-sdk/tree/main/examples/servers/simple-auth/mcp_simple_auth) 🐍 🎖️ - Example authenticated SSE server in the official Python SDK

Public test endpoints:
- [Asana MCP Server](https://mcp.asana.com/sse) - Production SSE endpoint for testing OAuth flows
- [Sentry MCP Server](https://mcp.sentry.dev/sse) - Production SSE endpoint for testing OAuth flows  
- [Atlassian MCP Server](https://mcp.atlassian.com/v1/sse) - Production SSE endpoint for testing OAuth flows (requires allowlisting)

## Libraries

> Reusable code libraries and components for MCP servers

- [marimo-team/codemirror-mcp](https://github.com/marimo-team/codemirror-mcp) 📇 - CodeMirror extension that implements MCP for resource mentions and prompt commands
- [jhgaylor/express-mcp-handlder](https://github.com/jhgaylor/express-mcp-handler) 📇 - Bind an MCP server to an express server using the StreamableHTTP Transport
- [JoshuaSiraj/mcp_auto_register](https://github.com/JoshuaSiraj/mcp_auto_register) 🐍 – Tool to automate the registration of functions and classes from a Python package into a FastMCP instance
- [isaacwasserman/mcp-langchain-ts-client](https://github.com/isaacwasserman/mcp-langchain-ts-client) 📇 – Use MCP provided tools in LangChain.js
- [traceloop/openllmetry#opentelemetry-instrumentation-mcp](https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-mcp) 🐍 - OpenTelemetry instrumentation for MCP Python that captures tool calls, notifications, listing, initialization handshakes and propagates traces from client to server.

## Utilities

> Useful tools for debugging, proxying, testing, and working with MCP servers

### Proxies and Gateways

- [adiom-data/grpcmcp](https://github.com/adiom-data/grpcmcp) 🏎️ - A MCP Server that allows access to gRPC API services.
- [boilingdata/mcp-server-and-gw](https://github.com/boilingdata/mcp-server-and-gw) 📇 - An MCP stdio to HTTP SSE transport gateway
- [emicklei/mcp-log-proxy](https://github.com/emicklei/mcp-log-proxy) 🏎️ - An MCP proxy server that offers a Web UI to see the complete message flow.
- [EvalsOne/MCP-Connect](https://github.com/EvalsOne/MCP-Connect) 📇 - A tiny tool that enables cloud-based AI services to access local Stdio based MCP servers via HTTP/HTTPS
- [fangyinc/mcpport](https://github.com/fangyinc/mcpport) 🐍 - A lightweight gateway & registry for MCP servers with NAT traversal support, allowing edge devices to provide MCP services across networks. Features include WebSocket/SSE/HTTP endpoints, authentication, IPv6 support, and a CLI tool for easy registration of stdio-based MCP servers.
- [hamidra/yamcp](https://github.com/hamidra/yamcp) 📇 - An MCP workspace manager to bundle and manage MCP servers in dedicated local workspaces (e.g., for coding, design, research).
- [lightconetech/mcp-gateway](https://github.com/lightconetech/mcp-gateway) 📇 - A gateway demo for MCP SSE Server
- [mcpjungle/MCPJungle](https://github.com/mcpjungle/MCPJungle) 🌳 - Self-hosted MCP Registry and Proxy for ai agents
- [multi-mcp](https://github.com/kfirtoledo/multi-mcp) 🐍 - A flexible and dynamic Multi-MCP Proxy Server that acts as a single MCP server while connecting to and routing between multiple backend MCP servers over STDIO or SSE. Deployable on Kubernetes by exposing a single port, and supports dynamic addition and removal of MCP servers at runtime.
- [punkpeye/mcp-proxy](https://github.com/punkpeye/mcp-proxy) 📇 - A TypeScript SSE proxy for MCP servers that use `stdio` transport
- [SecretiveShell/MCP-Bridge](https://github.com/SecretiveShell/MCP-Bridge) 🐍 – An openAI middleware proxy to use MCP in any existing openAI compatible client
- [sparfenyuk/mcp-proxy](https://github.com/sparfenyuk/mcp-proxy) 🐍 – An MCP stdio to SSE transport gateway
- [TBXark/mcp-proxy](https://github.com/TBXark/mcp-proxy) 🏎️ - An MCP proxy server that aggregates multiple MCP resource servers through a single HTTP server

### Development Tools

- [inercia/mcpshell](https://github.com/inercia/mcpshell) 🏎️ - Use shell scripts as MCP tools.
- [ithena-one/ithena-cli](https://github.com/ithena-one/ithena-cli) 🏎️ - Wraps MCP commands to log interactions locally, facilitating debugging and interaction audits. Optional cloud.
- [f/MCPTools](https://github.com/f/mcptools) 🏎️ - A command-line development tool for inspecting and interacting with MCP servers
- [flux159/mcp-chat](https://github.com/flux159/mcp-chat) 📇 - A CLI based client to chat and connect with any MCP server
- [mark3labs/mcphost](https://github.com/mark3labs/mcphost) 🏎️ - A CLI host application that enables LLMs to interact with external tools through MCP
- [strowk/mcp-autotest](https://github.com/strowk/mcp-autotest) 🏎️ - A command-line tool for running YAML based language-agnostic autotests
- [strowk/synf](https://github.com/strowk/synf) 🦀 - Tool to hot-reload MCP server on changes to saved files
- [strowk/mcptee](https://github.com/strowk/mcptee/) 🏎️ - Tool to proxy MCP and log inputs and outputs to YAML file
- [StacklokLabs/toolhive](https://github.com/Stacklok/toolhive) 🏎️ - A lightweight utility designed to simplify the deployment and management of MCP servers, ensuring ease of use, consistency, and security through containerization
- [addozhang/spring-rest-to-mcp](https://github.com/addozhang/spring-rest-to-mcp) 🏎️ - An [OpenRewrite](https://docs.openrewrite.org/) recipe collection that automatically converts Spring Web REST APIs to Spring AI Model Context Protocol (MCP) server tools.
- [taskade/mcp](https://github.com/taskade/mcp/tree/main/packages/openapi-codegen) 📇 - Generate MCP tools from OpenAPI schemas. Supports auto-linking, response normalization, and MCP server integration.

## Hosting

> Libraries & platforms for hosting MCP servers.

- [Glama](https://glama.ai/mcp/servers) – offers hosting of open-source MCP servers, enabling developers and enterprises to easily discover build, manage MCP servers.
- [Smithery](https://smithery.ai/) - cloud hosting MCP servers as a service via docker containers
- [vitorbari/mcp-operator](https://github.com/vitorbari/mcp-operator) - Kubernetes operator for MCP servers with automatic protocol validation, horizontal scaling, and built-in observability.

## Templates

> Example code ready to be made into a component of an MCP system.

- [fastmcp-boilerplate](https://github.com/punkpeye/fastmcp-boilerplate) 📇 – A simple MCP server built using FastMCP, TypeScript, ESLint, and Prettier.
- [dart-mcp-server-template](https://github.com/jhgaylor/dart-mcp-server-template) 🎯 - A template repository for creating Dart MCP servers. Provides a starting point with Docker configuration, http+stdio transport bindings, and a standard Dart project structure
- [rails-mcp-startup-boilerplate](https://github.com/f/mcp-startup-boilerplate) 💎 - A Rails template for creating Paid MCP servers compatible with Claude Integrations. It uses Rails 8.0.2, Devise, Doorkeeper, FastMCP and Stripe. Has a built-in UI.


## Resources

> Documentation, guides, standards, and learning materials for Model Context Protocol and MCP server development.

- [Model Context Protocol Specification](https://modelcontextprotocol.io/) — Official MCP specification
- [Model Context Protocol (MCP) Quickstart](https://glama.ai/blog/2024-11-25-model-context-protocol-quickstart)

## Tutorials

* [Setup Claude Desktop App to Use a SQLite Database](https://youtu.be/wxCCzo9dGj0)
* [amirshk/mcp-secrets-plugin](https://github.com/amirshk/mcp-secrets-plugin) 🐍 - A reference code to securely store and retrieve sensitive information using the system's native keychain
* [AI Agents for beginners by Microsoft](https://youtu.be/OhI005_aJkA?si=4nclgu-qAGgM57RJ) 🐍 #️⃣ Full Course (Lessons 1–10) using Semantic Kernel – Theoretical and practical content (1 hour)

## Related awesome lists:

- [awesome-mcp-servers](https://github.com/punkpeye/awesome-mcp-servers)
- [awesome-mcp-clients](https://github.com/punkpeye/awesome-mcp-clients)
