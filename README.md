<div align="center" >🤝 Show your support - give a ⭐️ if you liked the content
</div>

---

# **Awesome MCP Security [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)**

Everything you need to know about Model Context Protocol (MCP) security.

## Table of Contents

- [Awesome MCP Security](#awesome-mcp-security-)
  - 📔 [Security Considerations](#-security-considerations)
  - 📃 [Papers](#-papers)
  - 📺 [Videos](#-videos)
  - 📕 [Articles and Blog Posts](#-articles-and-blog-posts)
  - 🧑‍🚀 [Code](#-code)
  - 💻 [Other Useful Resources](#-other-useful-resources)
 
## 📔 Security Considerations
Official Security Considerations from the [Official MCP Specification Rev: 2025-03-26](https://modelcontextprotocol.io/specification/2025-03-26/server/tools)

- Servers **MUST**:
  - Validate all tool inputs
  - Implement proper access controls
  - Rate limit tool invocations
  - Sanitize tool outputs
    
- Clients **SHOULD**:
  - Prompt for user confirmation on sensitive operations
  - Show tool inputs to the user before calling the server, to avoid malicious or accidental data exfiltration
  - Validate tool results before passing to LLM
  - Implement timeouts for tool calls
  - Log tool usage for audit purposes
    
> [!WARNING]  
> For trust & safety and security, clients **MUST** consider tool annotations to be untrusted unless they come from trusted servers.

> [!WARNING]  
> For trust & safety and security, there **SHOULD** always be a human in the loop* with the ability to deny tool invocations.
>
> Applications **SHOULD**:
>
> - Provide UI that makes clear which tools are being exposed to the AI model.
> - Insert clear visual indicators when tools are invoked.
> - Present confirmation prompts to the user for operations, to ensure a human is in the loop.

> [!NOTE]  
> *Human-in-the-Loop (HITL) means that user help monitor and guide automated tasks, like deciding whether to accept tool requests in Cursor.
 
## 📃 Papers

- (2025-04) [MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits by Brandon Radosevich, John Halloran](https://arxiv.org/abs/2504.03767)
- (2025-03) [Model Context Protocol (MCP): Landscape, Security Threats, and Future Research Directions by Xinyi Hou, Yanjie Zhao, Shenao Wang, Haoyu Wang](https://arxiv.org/abs/2503.23278)

## 📺 Videos

- (09.04.2025) [MCP Servers are Security Nightmares... by Better Stack](https://www.youtube.com/watch?v=CRKYNyMc4PM)
- (03.04.2025) [MCP Security: Vetting Servers to Mitigate Tool Poisoning Attacks by JeredBlue](https://www.youtube.com/watch?v=LYUDUOevtqk)
- (03.04.2025) [Model Context Protocol (MCP) Security Concerns by Cory Wolff](https://www.youtube.com/watch?v=3DEqIquWCQ4)
 
## 📕 Articles and Blog Posts

- (09.04.2025) [Model Context Protocol has prompt injection security problems by Simon Willisons](https://simonwillison.net/2025/Apr/9/mcp-prompt-injection/)
- (07.04.2025) [Running MCP Tools Securely by mcp.run](https://docs.mcp.run/blog/2025/04/07/mcp-run-security/)
- (07.04.2025) [WhatsApp MCP Exploited: Exfiltrating your message history via MCP by invariantlabs.ai](https://invariantlabs.ai/blog/whatsapp-mcp-exploited)
- (07.04.2025) [An Introduction to MCP and Authorization by auth0](https://auth0.com/blog/an-introduction-to-mcp-and-authorization/)
- (06.04.2025) [The “S” in MCP Stands for Security by Elena Cross](https://elenacross7.medium.com/%EF%B8%8F-the-s-in-mcp-stands-for-security-91407b33ed6b)
- (04.04.2025) [MCP Servers are not safe! by Mehul Gupta](https://medium.com/data-science-in-your-pocket/mcp-servers-are-not-safe-bfbc2bb7aef8)
- (01.04.2025) [MCP Security Notification: Tool Poisoning Attacks by invariantlabs.ai](https://invariantlabs.ai/blog/mcp-security-notification-tool-poisoning-attacks)
- (31.03.2025) [Securing the Model Context Protocol by Alex Rosenzweig](https://block.github.io/goose/blog/2025/03/31/securing-mcp/)
- (29.03.2025) [MCP Servers: The New Security Nightmare by equixly.com](https://equixly.com/blog/2025/03/29/mcp-server-new-security-nightmare)
- (23.03.2025) [AI Model Context Protocol (MCP) and Security by Cisco](https://community.cisco.com/t5/security-blogs/ai-model-context-protocol-mcp-and-security/ba-p/5274394)

## 🧑‍🚀 Code
- (07.04.2025) [mcp-injection-experiments by invariantlabs-ai](https://github.com/invariantlabs-ai/mcp-injection-experiments)

## 💻 Other Useful Resources

- (31.03.2025) [I gave Claude root access to my server... Model Context Protocol explained by Fireship](https://www.youtube.com/watch?v=HyzlYwjoXOQ)
- (17.03.2025) [Model Context Protocol (MCP): The Key To Agentic AI by Jack Herrington](https://www.youtube.com/watch?v=VChRPFUzJGA)
- [Official MCP Specification](https://modelcontextprotocol.io/specification/2025-03-26/server/tools)
- [Model Context Protocol - Official MCP website](https://modelcontextprotocol.io/) 

 
# 😎 Contributing
👍🎉 First off, thanks for taking the time to contribute! 🎉👍

[Please read and follow our contributing guide](https://github.com/Puliczek/awesome-mcp-security/blob/main/CONTRIBUTING.md)

Thanks! 🦄


# 🤝 Show your support

<div>🤝 Show your support - give a ⭐️ if you liked the content</div>

# ✔️ Disclaimer
This project can only be used for educational purposes. Using this resource against target systems without prior permission is illegal, and any damages from misuse of this software will not be the responsibility of the author.
