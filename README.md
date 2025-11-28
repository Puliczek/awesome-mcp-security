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
  - 💾 [MCP Security Servers](#-mcp-security-servers)
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

- (2025-08) [Systematic Analysis of MCP Security](https://arxiv.org/pdf/2508.12538)
- (2025-05) [Beyond the Protocol: Unveiling Attack Vectors in the Model Context Protocol Ecosystem](https://arxiv.org/abs/2506.02040)
- (2025-05) [Enterprise-Grade Security for the Model Context Protocol (MCP): Frameworks and Mitigation Strategies](https://arxiv.org/pdf/2504.08623)
- (2025-04) [Simplified and Secure MCP Gateways for Enterprise AI Integration by Ivo Brett](https://arxiv.org/abs/2504.19997)
- (2025-04) [MCP Guardian: A Security-First Layer for Safeguarding MCP-Based AI System by Sonu Kumar, Anubhav Girdhar, Ritesh Patil, Divyansh Tripathi](https://arxiv.org/abs/2504.12757)
- (2025-04) [MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits by Brandon Radosevich, John Halloran](https://arxiv.org/abs/2504.03767)
- (2025-03) [Model Context Protocol (MCP): Landscape, Security Threats, and Future Research Directions by Xinyi Hou, Yanjie Zhao, Shenao Wang, Haoyu Wang](https://arxiv.org/abs/2503.23278)

## 📺 Videos

- (13.06.2025) [MCP Auth: The Future of AI Agent Security - by Arcade.dev](https://youtu.be/zj29lslZxFg?si=j1YYkhycoQcE_rJ0)
- (17.05.2025) [A2A - MCP SECURITY Threats: Protect your AI Agents by Discover AI](https://www.youtube.com/watch?v=h_6unQxHyb4)
- (06.05.2025) [Making MCP Production Ready – Building MCP for Enterprise - by Arcade.dev](https://youtu.be/f1sLBGWnByc?si=wwa7Qm_vDM7VyElr)
- (11.04.2025) [This MCP Server Trick Can Steal Your API Keys by Prompt Engineering](https://www.youtube.com/watch?v=86e49wcXst4)
- (09.04.2025) [MCP Servers are Security Nightmares... by Better Stack](https://www.youtube.com/watch?v=CRKYNyMc4PM)
- (03.04.2025) [MCP Security: Vetting Servers to Mitigate Tool Poisoning Attacks by JeredBlue](https://www.youtube.com/watch?v=LYUDUOevtqk)
- (03.04.2025) [Model Context Protocol (MCP) Security Concerns by Cory Wolff](https://www.youtube.com/watch?v=3DEqIquWCQ4)
- (02.06.2025) [Agentic Access: OAuth Isn't Enough | Zero Trust for AI Agents w/ Nick Taylor (Pomerium + MCP)](https://www.youtube.com/watch?v=KY1kCZkqUh0)

## 📕 Articles, X threads and Blog Posts

- (14.08.2025) [MCP Security Best Practices: How to Prevent Risks and Threats by Dmitriy Redkin](https://mcpmanager.ai/blog/mcp-security-best-practices/)
- (08.08.2025) [we hijacked cursor via jira mcp by submitting a support ticket by @mbrg0](https://x.com/mbrg0/status/1953932780855013682)
- (28.07.2025) [We built the security layer MCP always needed by Cliff Smith](https://blog.trailofbits.com/2025/07/28/we-built-the-security-layer-mcp-always-needed/)
- (24.07.2025) [Security Advisory: Anthropic's Slack MCP Server Vulnerable to Data Exfiltration by WUNDERWUZZI](https://embracethered.com/blog/posts/2025/security-advisory-anthropic-slack-mcp-server-data-leakage/)
- (11.07.2025) [Securing Model Context Protocol (MCP) with Teleport and AWS](https://goteleport.com/blog/securing-model-context-protocol-with-teleport-and-aws)
- (10.07.2025) [Critical mcp-remote Vulnerability Enables Remote Code Execution, Impacting 437,000+ Downloads by Ravie Lakshmanan](https://thehackernews.com/2025/07/critical-mcp-remote-vulnerability.html)
- (06.07.2025) [Combine the Supabase MCP with another MCP that provides exposure to untrusted tokens and a way to send data back out again by Simon Willison](https://x.com/simonw/status/1941674715720057258)
- (05.07.2025) [Neon official remote MCP exploited!](https://www.tramlines.io/blog/neon-official-remote-mcp-exploited-and-guardrailed-with-tramlines)
- (19.06.2025) [Cato CTRL Threat Research: PoC Attack Targeting Atlassian's Model Context Protocol (MCP) Introduces New "Living Off AI" Risk](https://www.catonetworks.com/blog/cato-ctrl-poc-attack-targeting-atlassians-mcp/)
- (18.06.2025) [Asana Discloses Data Exposure Bug in MCP Server by Greg Pollock](https://www.upguard.com/blog/asana-discloses-data-exposure-bug-in-mcp-server)
- (30.05.2025) [Poison everywhere: No output from your MCP server is safe by Simcha Kosman](https://www.cyberark.com/resources/threat-research-blog/poison-everywhere-no-output-from-your-mcp-server-is-safe)
- (26.05.2025) [GitHub MCP Exploited: Accessing private repositories via MCP by invariantlabs.ai](https://invariantlabs.ai/blog/mcp-github-vulnerability)
- (20.05.2025) [Securing the Model Context Protocol: Building a safer agentic future on Windows](https://blogs.windows.com/windowsexperience/2025/05/19/securing-the-model-context-protocol-building-a-safer-agentic-future-on-windows/)
- (16.05.2025) [MCP Security in 2025](https://www.prompthub.us/blog/mcp-security-in-2025)
- (02.05.2025) [Security Best Practices by Model Context Protocol](https://modelcontextprotocol.io/specification/draft/basic/security_best_practices)
- (30.04.2025) [Insecure credential storage plagues MCP by Keith Hoodlet](https://blog.trailofbits.com/2025/04/30/insecure-credential-storage-plagues-mcp/)
- (29.04.2025) [Deceiving users with ANSI terminal codes in MCP by Keith Hoodlet](https://blog.trailofbits.com/2025/04/29/deceiving-users-with-ansi-terminal-codes-in-mcp/)
- (29.04.2025) [Building Own MCP - Augmented LLM for Threat Hunting by Eito Tamura](https://tierzerosecurity.co.nz/2025/04/29/mcp-llm.htm)
- (23.04.2025) [How MCP servers can steal your conversation history by Keith Hoodlet](https://blog.trailofbits.com/2025/04/23/how-mcp-servers-can-steal-your-conversation-history)
- (21.04.2025) [Jumping the line: How MCP servers can attack you before you ever use them](https://blog.trailofbits.com/2025/04/21/jumping-the-line-how-mcp-servers-can-attack-you-before-you-ever-use-them/)
- (19.04.2025) [OAuth's Role in MCP Security by Gunnar Peterson](https://defensiblesystems.substack.com/p/oauths-role-in-mcp-security)
- (17.04.2025) [Research Briefing: MCP Security by Rami McCarthy](https://www.wiz.io/blog/mcp-security-research-briefing)
- (17.04.2025) [MCP Not Safe - Reasons and Ideas by Phala Network](https://phala.network/posts/MCP-Not-Safe-Reasons-and-Ideas)
- (15.04.2025) [MCP can be a security nightmare for building AI Agents by Rakesh Gohel](https://www.linkedin.com/posts/rakeshgohel01_mcp-can-be-a-security-nightmare-for-building-activity-7317536567315636225-zKFp/?utm_source=share&utm_medium=member_desktop&rcm=ACoAAB_LYZwBepPqbIN5g8KzxPVSyzHNUgJhBew)
- (15.04.2025) [Model Context Protocol (MCP) aka Multiple Cybersecurity Perils by Chris Martorella](https://chrismartorella.ghost.io/model-context-protocol-mcp-aka-multiple-cybersecurity-perils/)
- (14.04.2025) [Model Context Protocol (MCP) Security by Evren](https://evren.ninja/mcp-security.html)
- (14.04.2025) [Security Analysis: Potential AI Agent Hijacking via MCP and A2A Protocol Insights by Nicky](https://medium.com/@foraisec/security-analysis-potential-ai-agent-hijacking-via-mcp-and-a2a-protocol-insights-cd1ec5e6045f)
- (14.04.2025) [MCP Security Checklist: A Security Guide for the AI Tool Ecosystem by slowmist](https://github.com/slowmist/MCP-Security-Checklist)
- (13.04.2025) [Everything Wrong with MCP by Shrivu Shankar](https://blog.sshh.io/p/everything-wrong-with-mcp)
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
- (18.03.2025) [New Vulnerability in GitHub Copilot and Cursor: How Hackers Can Weaponize Code Agents by Ziv Karliner](https://www.pillar.security/blog/new-vulnerability-in-github-copilot-and-cursor-how-hackers-can-weaponize-code-agents)
- (13.02.2025) [Chained commands (&&) bypass yolo mode “denylist” in Cursor by lukemmtt](https://forum.cursor.com/t/chained-commands-bypass-yolo-mode-denylist/50775)
- (18.06.2025) [The Model Context Protocol Security Reality Check](https://thenewstack.io/the-model-context-protocol-security-reality-check/)

## 🧑‍🚀 Tools and code

- [MCP Audit Extension - Audit and log all GitHub Copilot MCP tool calls in VSCode with ease](https://github.com/Agentity-com/mcp-audit-extension)
- [Secure MCP - Security auditing tool to detect MCP vulnerabilities and misconfigurations by makalin](https://github.com/makalin/SecureMCP)
- [mcp-context-protector - Security wrapper for MCP servers by trailofbits](https://github.com/trailofbits/mcp-context-protector)
- [AI-Infra-Guard by Tencent Zhuque Lab](https://github.com/Tencent/AI-Infra-Guard) - MCP Server Security Analysis Tool - a comprehensive, intelligent, easy-to-use, and lightweight AI Infrastructure Vulnerability Assessment.
- [MCP Guardian - Manage your LLM's access to MCP servers by eqtylab](https://github.com/eqtylab/mcp-guardian)
- [MCP Tool Poisoning Experiments by invariantlabs-ai](https://github.com/invariantlabs-ai/mcp-injection-experiments)
- [Google Security Operations and Threat Intelligence MCP Server - Access Google's security products and services](https://github.com/google/mcp-security)
- [MCP Watch - Vulnerability scanner for MCP servers](https://github.com/kapilduraphe/mcp-watch)
- [MCP Security Checklist: A Security Guide for the AI Tool Ecosystem by SlowMist](https://github.com/slowmist/MCP-Security-Checklist)
- [workers-mcp - Connect Cloudflare Workers with your MCP clients by Cloudflare](https://github.com/cloudflare/workers-mcp)
- [MCP Gateway - Acts as intermediary between LLMs and other MCP servers by lasso-security](https://github.com/lasso-security/mcp-gateway)
- [AWS Security MCP - Access AWS security tools by groovyBugify](https://github.com/groovyBugify/aws-security-mcp)]
- [MCPAuth: Gateway Authentication for Secure Enterprise MCP Integrations by Oide Brett](https://github.com/oidebrett/mcpauth)
- [mcpserverscanner.com by orgor](https://mcpserverscanner.com/)
- [mcpscan.ai](https://mcpscan.ai/)
- [Damn Vulnerable MCP Server by harishsg993010](https://github.com/harishsg993010/damn-vulnerable-MCP-server)
- [ToolHive - making MCP servers easy and secure by StacklokLabs](https://github.com/StacklokLabs/toolhive)
- [MCP-Shield – Detect security issues in MCP servers by riseandignite](https://github.com/riseandignite/mcp-shield)
- [mcp-scan by invariantlabs-ai](https://github.com/invariantlabs-ai/mcp-scan)
- [MCP Ethical Hacking by cmpxchg16](https://github.com/cmpxchg16/mcp-ethical-hacking)
- [mcp-injection-experiments by invariantlabs-ai](https://github.com/invariantlabs-ai/mcp-injection-experiments)
- [MCP Defender - Blocks malicious MCP traffic](https://github.com/MCP-Defender/MCP-Defender)
- [Octocode](https://github.com/bgauryy/octocode-mcp) - AI-powered developer assistant that enables advanced research, analysis and discovery across GitHub ecosystem. Allow smart search of security patterns across repositories.
- [Defenter](https://defenter.ai/) - Real-time semantic monitoring of AI coding agents and MCP server communication to protect from data leaks, context contamination, and malicious prompt injections.

## 💾 MCP Security Servers
- [Nuclei MCP Integration by addcontent](https://github.com/addcontent/nuclei-mcp) - Provides a standardized MCP interface for Nuclei, a fast and customizable vulnerabilty scanner, for performing scans and managing vulnerablity assessments
- [Illumio MCP Server by alexgoller](https://github.com/alexgoller/illumio-mcp-server) - MCP server for interacting with Illumio Policy Compute Engine for Illumio workload management, label operations, traffic flow analysis
- [TriageMCP by eversinc33](https://github.com/eversinc33/TriageMCP) - MCP server for doing basic static triage of Portable Executable (PE) files
- [RunReveal MCP Server](https://docs.runreveal.com/reference/model-context-protocol) - MCP server for RunReveal to query security logs at scale
- [Semgrep MCP Server](https://github.com/semgrep/mcp) - MCP server for using Semgrep to scan code for vulnerabilities
- [GhidraMCP by LaurieWired](https://github.com/LaurieWired/GhidraMCP) - MCP server for automatic reverse engineering in Ghidra, a software reverse engineering platform.
- [IDA-Pro-MCP by mrexodia](https://github.com/mrexodia/ida-pro-mcp) - MCP server for reverse engineering in IDA Pro, a tool for analyzing software and binary files.
- [binaryninja-mcp by MCPPhalanx](https://github.com/MCPPhalanx/binaryninja-mcp) - MCP server for Binary Ninja, a binary analysis tool.
- [Burp Suite MCP by PortSwigger](https://github.com/PortSwigger/mcp-server) - MCP integration for web security testing in Burp Suite, a security testing tool for web applications.
- [BloodHound-MCP-AI by MorDavid](https://github.com/MorDavid/BloodHound-MCP-AI) - MCP server integration for BloodHound, a tool for analyzing Active Directory domains.
- [RoadRecon MCP by atomicchonk](https://github.com/atomicchonk/roadrecon_mcp_server) - MCP server for Azure AD data analysis with ROADRecon, a tool for mapping Azure Active Directory environments.
- [Jadx MCP Plugin by mobilehackinglab](https://github.com/mobilehackinglab/jadx-mcp-plugin) - Jadx plugin for MCP server access via HTTP, used for decompiling Android apps.
- [VirusTotal MCP Server by BurtTheCoder](https://github.com/BurtTheCoder/mcp-virustotal) - MCP server for querying the VirusTotal API, a service for analyzing files and URLs for viruses.
- [Shodan MCP Server by BurtTheCoder](https://github.com/BurtTheCoder/mcp-shodan) - MCP server for querying the Shodan API, which provides data on Internet-connected devices.
- [DNStwist MCP Server by BurtTheCoder](https://github.com/BurtTheCoder/mcp-dnstwist) - MCP server for DNS fuzzing with dnstwist, a tool for detecting phishing and domain takeover threats.
- [Maigret MCP Server by BurtTheCoder](https://github.com/BurtTheCoder/mcp-maigret) - MCP server for OSINT data collection with Maigret, a tool that gathers user info from various sources.
- [pomerium/pomerium](https://github.com/pomerium/pomerium) - Identity-aware proxy with native support for Zero Trust access, now including MCP support.
  - Example implementations:
    - [pomerium/mcp-app-demo](https://github.com/pomerium/mcp-app-demo)
    - [pomerium/mcp-servers](https://github.com/pomerium/mcp-servers)
- [urldna/mcp](https://github.com/urldna/mcp) - urlDNA MCP server for phishing detection and URL analysis through advanced contextual scanning.

## 💻 Other Useful Resources

- [Awesome Cybersecurity Agentic AI](https://github.com/raphabot/awesome-cybersecurity-agentic-ai) - Collection of resources on using AI agents for security use cases
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
