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
  - 📕 [Articles, X threads and Blog Posts](#-articles-x-threads-and-blog-posts)
  - 🧑‍🚀 [Tools and code](#-tools-and-code)
  - 💻 [Other Useful Resources](#-other-useful-resources)
 
## 📔 Security Considerations
Official Security Considerations from the [Official MCP Specification Rev: 2025-03-26](https://modelcontextprotocol.io/specification/2025-03-26/server/tools)

> [!NOTE] 
> 15.04.2025: The current MCP [auth specification](https://modelcontextprotocol.io/specification/2025-03-26/basic/authorization) is in progress of being replaced by a more [robust specification](https://github.com/modelcontextprotocol/specification/pull/284). Please join the conversation if you have concerns around the current auth specification.

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

- (11.04.2025) [This MCP Server Trick Can Steal Your API Keys by Prompt Engineering](https://www.youtube.com/watch?v=86e49wcXst4)
- (09.04.2025) [MCP Servers are Security Nightmares... by Better Stack](https://www.youtube.com/watch?v=CRKYNyMc4PM)
- (03.04.2025) [MCP Security: Vetting Servers to Mitigate Tool Poisoning Attacks by JeredBlue](https://www.youtube.com/watch?v=LYUDUOevtqk)
- (03.04.2025) [Model Context Protocol (MCP) Security Concerns by Cory Wolff](https://www.youtube.com/watch?v=3DEqIquWCQ4)
 
## 📕 Articles, X threads and Blog Posts 

- (11.04.2025) [Diving Into the MCP Authorization Specification by Allen Zhou](https://www.descope.com/blog/post/mcp-auth-spec)
- (11.04.2025) [Vulnerability Discovered in Base-MCP: Hackers Can Redirect Transactions on Cursor AI and Anthropic Claude by @jlwhoo7](https://x.com/jlwhoo7/status/1911056723710026120)
- (09.04.2025) [Here's an example of remote MCP malware that steals your .env secrets in @cursor_ai by Maciej Pulikowski](https://x.com/pulik_io/status/1910053590921535992)
- (09.04.2025) [Old Security Rakes In New MCP Yards by Den Delimarsky](https://den.dev/blog/security-rakes-mcp/)
- (09.04.2025) [Model Context Protocol has prompt injection security problems by Simon Willisons](https://simonwillison.net/2025/Apr/9/mcp-prompt-injection/)
- (07.04.2025) [(RFC) Update the Authorization specification for MCP servers #284 by localden](https://github.com/modelcontextprotocol/modelcontextprotocol/pull/284)
- (07.04.2025) [Improving The Model Context Protocol Authorization Spec - One RFC At A Time by Den Delimarsky](https://den.dev/blog/model-context-protocol-oauth-rfc/)
- (07.04.2025) [Running MCP Tools Securely by mcp.run](https://docs.mcp.run/blog/2025/04/07/mcp-run-security/)
- (07.04.2025) [WhatsApp MCP Exploited: Exfiltrating your message history via MCP by invariantlabs.ai](https://invariantlabs.ai/blog/whatsapp-mcp-exploited)
- (07.04.2025) [An Introduction to MCP and Authorization by auth0](https://auth0.com/blog/an-introduction-to-mcp-and-authorization/)
- (06.04.2025) [The “S” in MCP Stands for Security by Elena Cross](https://elenacross7.medium.com/%EF%B8%8F-the-s-in-mcp-stands-for-security-91407b33ed6b)
- (04.04.2025) [MCP Servers are not safe! by Mehul Gupta](https://medium.com/data-science-in-your-pocket/mcp-servers-are-not-safe-bfbc2bb7aef8)
- (03.04.2025) [Let's fix OAuth in MCP by Aaron Parecki](https://aaronparecki.com/2025/04/03/15/oauth-for-model-context-protocol)
- (03.04.2025) [MCP Resource Poisoning Prompt Injection Attacks by Bernard IQ](https://www.bernardiq.com/blog/resource-poisoning/)
- (01.04.2025) [MCP Security Notification: Tool Poisoning Attacks by invariantlabs.ai](https://invariantlabs.ai/blog/mcp-security-notification-tool-poisoning-attacks)
- (31.03.2025) [The MCP Authorization Spec Is... a Mess for Enterprise by Christian Posta](https://blog.christianposta.com/the-updated-mcp-oauth-spec-is-a-mess/)
- (31.03.2025) [Securing the Model Context Protocol by Alex Rosenzweig](https://block.github.io/goose/blog/2025/03/31/securing-mcp/)
- (29.03.2025) [MCP Servers: The New Security Nightmare by equixly.com](https://equixly.com/blog/2025/03/29/mcp-server-new-security-nightmare)
- (23.03.2025) [AI Model Context Protocol (MCP) and Security by Cisco](https://community.cisco.com/t5/security-blogs/ai-model-context-protocol-mcp-and-security/ba-p/5274394)
- (13.02.2025) [Chained commands (&&) bypass yolo mode “denylist” in Cursor by lukemmtt](https://forum.cursor.com/t/chained-commands-bypass-yolo-mode-denylist/50775)

## 🧑‍🚀 Tools and code
- (15.04.2025) [MCP-Shield – Detect security issues in MCP servers by riseandignite](https://github.com/riseandignite/mcp-shield)
- (10.04.2025) [mcp-scan by invariantlabs-ai](https://github.com/invariantlabs-ai/mcp-scan)
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
