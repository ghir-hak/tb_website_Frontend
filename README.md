<div align="center">
  <a href="https://discord.gg/KbN3KN7kpQ">
    <img src="images/discord-btn.png" alt="Join our Discord" height="30">
  </a>
  <a href="https://tau.how">
    <img src="images/docs-btn.png" alt="Read the Docs" height="30">
  </a>
  <a href="https://console.taubyte.com">
    <img src="images/sandbox-btn.png" alt="Try our Sandbox" height="30">
  </a>
</div>

<br/>

<div align="center">
  <a href="https://taubyte.com" target="_blank" rel="noopener noreferrer">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="images/logo-with-text-tau-white.png">
      <img width="160" src="images/logo-with-text-tau-black.png" alt="Tau Logo">
    </picture>
  </a>
  
  <br/>
  <br/>

  <a href="https://github.com/taubyte/tau/releases">
    <img src="https://img.shields.io/github/release/taubyte/tau.svg" alt="Release">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/github/license/taubyte/tau" alt="License">
  </a>
  <a href="https://goreportcard.com/report/github.com/taubyte/tau">
    <img src="https://goreportcard.com/badge/github.com/taubyte/tau" alt="Go Report Card">
  </a>

  <h1>Distributed Cloud Platform</h1>
  <p><strong>Self-hosted • Git-native • P2P architecture</strong></p>
</div>

<br/>

---

<br/>

<div align="center">
  <h2>What is Taubyte?</h2>
</div>

<p align="center">
Taubyte is a complete, self-hosted cloud platform that you deploy with a single binary.<br/>
It provides all the infrastructure components needed to build and run modern applications—<br/>
serverless functions, static hosting, databases, storage, messaging, and CI/CD—<br/>
without relying on third-party cloud providers.
</p>

<br/>

<div align="center">

### Key Differentiators

</div>

<table align="center">
<tr>
<td align="center" width="50%">

**🔄 Git-Native by Design**

Infrastructure is defined in Git repositories. Every commit triggers automatic deployment. No API calls, no infrastructure-as-code tools, no manual provisioning.

</td>
<td align="center" width="50%">

**🌐 Peer-to-Peer Architecture**

Built on libp2p, nodes automatically discover each other, handle failures, and distribute content. No central coordination, no single point of failure.

</td>
</tr>
<tr>
<td align="center" width="50%">

**⚡ WebAssembly Runtime**

Applications run in sandboxed WebAssembly environments with fast cold starts (~10ms) and near-native performance.

</td>
<td align="center" width="50%">

**🔐 Content-Addressed Storage**

Files are stored by cryptographic hash (IPFS), enabling automatic deduplication, parallel distribution, and integrity verification.

</td>
</tr>
<tr>
<td align="center" width="50%">

**💻 Local-to-Production Parity**

Development environments run the exact same services as production. No mocking, no simulation, no environmental drift.

</td>
<td align="center" width="50%">

**🚀 Zero Dependencies**

Single static binary with no external dependencies. No Kubernetes, no orchestration complexity, just one binary.

</td>
</tr>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>Core Features</h2>
</div>

<table>
<thead>
<tr>
<th>Feature</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Serverless Functions</strong></td>
<td>Event-driven compute with HTTP, pub/sub, and P2P triggers. Compiled to WebAssembly for security and portability.</td>
</tr>
<tr>
<td><strong>Static Hosting</strong></td>
<td>Serve websites with automatic HTTPS certificates via Let's Encrypt. Global edge distribution included.</td>
</tr>
<tr>
<td><strong>Databases</strong></td>
<td>Key-value stores with application or global scope. CRDT-based replication for conflict-free synchronization.</td>
</tr>
<tr>
<td><strong>Object Storage</strong></td>
<td>S3-compatible storage with content addressing. Automatic deduplication and multi-node distribution.</td>
</tr>
<tr>
<td><strong>Messaging</strong></td>
<td>Pub/sub channels using GossipSub protocol. Asynchronous communication between services and functions.</td>
</tr>
<tr>
<td><strong>Custom Domains</strong></td>
<td>Bring your own domain with automatic TLS provisioning. DNS and certificate management handled automatically.</td>
</tr>
<tr>
<td><strong>CI/CD Pipeline</strong></td>
<td>Git webhooks trigger builds in isolated Docker containers. Artifacts stored in content-addressed storage.</td>
</tr>
<tr>
<td><strong>Edge Distribution</strong></td>
<td>Geographic routing based on node location. Traffic automatically directed to nearest healthy instance.</td>
</tr>
<tr>
<td><strong>Plugin System</strong></td>
<td>Extend platform capabilities with Orbit plugins. Add integrations without modifying core services.</td>
</tr>
</tbody>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>Technology Highlights</h2>
  <p><em>Modern, proven technologies built into Taubyte</em></p>
</div>

<br/>

<table align="center">
<tr>
<td width="33%" valign="top">

<div align="center">

### WebAssembly & Runtime

</div>

- **[wazero](https://wazero.io/)** - Pure Go WebAssembly runtime with JIT compilation
- **WASI Support** - WebAssembly System Interface
- **~10ms cold starts** - Near-instant initialization

</td>
<td width="33%" valign="top">

<div align="center">

### Distributed Systems

</div>

- **[CRDT](https://github.com/ipfs/go-ds-crdt)** - Conflict-free replicated data types
- **[Pebble](https://github.com/cockroachdb/pebble)** - LSM-tree storage (RocksDB-style)
- **[Kademlia DHT](https://en.wikipedia.org/wiki/Kademlia)** - Distributed hash table

</td>
<td width="33%" valign="top">

<div align="center">

### P2P Networking

</div>

- **[libp2p](https://libp2p.io/)** - Modular P2P networking stack
- **GossipSub** - Efficient pub/sub messaging
- **Circuit Relay** - NAT traversal
- **[IPFS Lite](https://github.com/hsanjuan/ipfs-lite)** - Content-addressed storage

</td>
</tr>
<tr>
<td width="33%" valign="top">

<div align="center">

### Security & Certificates

</div>

- **[ACME Protocol](https://letsencrypt.org/)** - Automatic TLS via Let's Encrypt
- **WebAssembly Sandboxing** - Memory-safe execution

</td>
<td width="33%" valign="top">

<div align="center">

### Developer Tools

</div>

- **[Starlark](https://github.com/google/starlark-go)** - Python-like scripting
- **[MCP](https://modelcontextprotocol.io/)** - AI-assisted development
- **Taucorder** - Network debugging
- **Sensors** - Real-time metrics

</td>
<td width="33%" valign="top">

<div align="center">

### Build & CI/CD

</div>

- **Docker** - Isolated build environments
- **Git Webhooks** - Native GitHub integration
- **Content Addressing** - Immutable artifacts

</td>
</tr>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>Example Applications</h2>
  <p><em>See real-world applications built with Taubyte</em></p>
</div>

<br/>

<div align="center">

<!-- USER: Add YouTube video links here -->

**[Link to Video 1]** - [Description of application]

**[Link to Video 2]** - [Description of application]

**[Link to Video 3]** - [Description of application]

</div>

<br/>

---

<br/>

<div align="center">
  <h2>Getting Started</h2>
  <h3>Local Development with Dream</h3>
  <p>The recommended way to start with Taubyte is <strong>Dream</strong>—a complete cloud environment that runs on your local machine.</p>
</div>

<br/>

<table align="center">
<tr>
<td align="center" width="50%">

### Option 1: Dream Desktop
**Recommended**

Graphical interface for managing local cloud instances.

**Download:**
- Linux: [Download link]
- Windows: [Download link]
- macOS: [Download link]

</td>
<td align="center" width="50%">

### Option 2: Dream CLI
**For automation & CI/CD**

```bash
npm install -g @taubyte/dream
dream
```

</td>
</tr>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>Setup Instructions</h2>
</div>

<br/>

<details>
<summary><h3>Step 1: Configure Local DNS</h3></summary>

<br/>

Dream requires a DNS entry to function properly. Add the following to your system's hosts file:

<table>
<thead>
<tr>
<th>Operating System</th>
<th>File Path</th>
<th>Entry</th>
</tr>
</thead>
<tbody>
<tr>
<td>Linux / macOS</td>
<td><code>/etc/hosts</code></td>
<td><code>127.0.0.1 hal.computers.com</code></td>
</tr>
<tr>
<td>Windows</td>
<td><code>C:\Windows\System32\drivers\etc\hosts</code></td>
<td><code>127.0.0.1 hal.computers.com</code></td>
</tr>
</tbody>
</table>

<br/>

This allows Dream to handle requests as if it were a real cloud deployment.

</details>

<details>
<summary><h3>Step 2: Create a Universe</h3></summary>

<br/>

Launch Dream Desktop and create a new universe.

<div align="center">

**What is a Universe?**

A universe is an isolated Taubyte cloud instance running locally. It includes all platform services (Gateway, Substrate, Storage, Auth, Build services) and behaves identically to a production deployment.

</div>

<br/>

<table align="center">
<thead>
<tr>
<th>Type</th>
<th>Use Case</th>
<th>Persistence</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Ephemeral</strong></td>
<td>Quick testing, experimentation</td>
<td>Deleted on exit</td>
</tr>
<tr>
<td><strong>Persistent</strong></td>
<td>Active development, project work</td>
<td>Saved to disk</td>
</tr>
</tbody>
</table>

<br/>

Name your universe (e.g., "development") and click Create.

</details>

<details>
<summary><h3>Step 3: Connect to Web Console</h3></summary>

<br/>

<div align="center">

Navigate to **[console.taubyte.com](https://console.taubyte.com)** in your browser.

The console automatically detects your local Dream instance and establishes a connection.

</div>

</details>

<details>
<summary><h3>Step 4: Create a Project</h3></summary>

<br/>

In the console:

1. Click **New Project**
2. Enter a project name (e.g., "my-application")
3. Connect to a GitHub repository (or create a new one)
4. Click Create

The console generates a `.taubyte` directory in your repository with initial configuration.

</details>

<details>
<summary><h3>Step 5: Add Resources</h3></summary>

<br/>

<div align="center">

Taubyte organizes applications into composable resources.

</div>

<br/>

<table>
<thead>
<tr>
<th>Resource Type</th>
<th>Purpose</th>
<th>Scope</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Function</strong></td>
<td>Serverless compute with event triggers</td>
<td>Application</td>
</tr>
<tr>
<td><strong>Website</strong></td>
<td>Static file hosting with CDN</td>
<td>Application</td>
</tr>
<tr>
<td><strong>Database</strong></td>
<td>Key-value data storage</td>
<td>Application or Global</td>
</tr>
<tr>
<td><strong>Storage</strong></td>
<td>Object storage for files and assets</td>
<td>Application or Global</td>
</tr>
<tr>
<td><strong>Messaging</strong></td>
<td>Pub/sub channels for async communication</td>
<td>Application or Global</td>
</tr>
<tr>
<td><strong>Service</strong></td>
<td>Long-running background processes</td>
<td>Application</td>
</tr>
<tr>
<td><strong>Library</strong></td>
<td>Shared code modules</td>
<td>Application</td>
</tr>
<tr>
<td><strong>Domain</strong></td>
<td>Custom DNS with automatic TLS</td>
<td>Application or Global</td>
</tr>
<tr>
<td><strong>SmartOps</strong></td>
<td>Event-driven automation workflows</td>
<td>Application</td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

**Example: Creating a Function**

</div>

1. Select **Function** from resource types
2. Configure:
   - Name: `api`
   - Language: `Go` / `Rust` / `AssemblyScript`
   - Trigger: `HTTP`
   - Path: `/api/*`
   - Method: `GET, POST`
3. Click Create

The console generates a code template in your repository under `functions/api/`.

</details>

<details>
<summary><h3>Step 6: Deploy Your Application</h3></summary>

<br/>

Commit and push your changes:

```bash
git add .
git commit -m "Add API function"
git push origin main
```

<br/>

<div align="center">

**What happens next:**

</div>

1. GitHub sends a webhook to your Dream instance
2. Patrick (CI/CD service) receives the webhook and creates a build job
3. Monkey (build service) clones your repository and compiles code to WebAssembly
4. Hoarder (storage service) stores the compiled artifacts
5. TNS (configuration service) updates with the new deployment
6. Substrate (runtime service) loads and executes your function

<br/>

<div align="center">

Access your function at: `http://hal.computers.com/api/your-endpoint`

</div>

</details>

<br/>

---

<br/>

<div align="center">
  <h2>Production Deployment</h2>
</div>

<br/>

<div align="center">

### Using Spore Drive (Recommended)

Spore Drive automates Taubyte installation and configuration across multiple servers.

<!-- USER: I'll help you add this section later -->

**[Section to be added - Spore Drive installation and setup]**

</div>

<br/>

---

<br/>

<div align="center">

### Manual Installation

For manual deployment or custom configurations:

</div>

<br/>

```bash
# Install Taubyte binary
curl https://get.tau.link/tau | sh

# Generate node configuration
tau config generate \
  --name yourdomain.com \
  --services all \
  --ip <public-ip-address> \
  --swarm
```

<br/>

<div align="center">

**Configuration Options:**

</div>

<table align="center">
<thead>
<tr>
<th>Parameter</th>
<th>Description</th>
<th>Example</th>
</tr>
</thead>
<tbody>
<tr>
<td><code>--name</code></td>
<td>Your domain name</td>
<td><code>cloud.mycompany.com</code></td>
</tr>
<tr>
<td><code>--services</code></td>
<td>Services to run on this node</td>
<td><code>all</code> or <code>gateway,substrate</code></td>
</tr>
<tr>
<td><code>--ip</code></td>
<td>Public IP address</td>
<td><code>203.0.113.10</code></td>
</tr>
<tr>
<td><code>--swarm</code></td>
<td>Join P2P network</td>
<td>Flag (no value)</td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

**Start the node:**

</div>

```bash
tau start
```

<br/>

<div align="center">

### Multi-Node Architecture

For production deployments, distribute services across specialized nodes:

</div>

<table align="center">
<thead>
<tr>
<th>Node Type</th>
<th>Services</th>
<th>Purpose</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Edge</strong></td>
<td>Gateway, Substrate</td>
<td>Handle incoming traffic and execute functions</td>
</tr>
<tr>
<td><strong>Build</strong></td>
<td>Patrick, Monkey</td>
<td>Process CI/CD builds</td>
</tr>
<tr>
<td><strong>Storage</strong></td>
<td>Hoarder, TNS</td>
<td>Store content and configuration</td>
</tr>
<tr>
<td><strong>Discovery</strong></td>
<td>Seer, Auth</td>
<td>Service discovery and authentication</td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

Each node automatically discovers and communicates with others via libp2p.

</div>

<br/>

---

<br/>

<div align="center">
  <h2>Platform Architecture</h2>
  <h3>Core Services</h3>
</div>

<br/>

<table>
<thead>
<tr>
<th>Service</th>
<th>Role</th>
<th>Technology</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Gateway</strong></td>
<td>HTTP/HTTPS ingress, routing, load balancing</td>
<td>Go, ACME, L7 routing</td>
</tr>
<tr>
<td><strong>Substrate</strong></td>
<td>WebAssembly runtime, function execution</td>
<td>wazero, WASI</td>
</tr>
<tr>
<td><strong>Auth</strong></td>
<td>GitHub OAuth, webhook management, TLS certificates</td>
<td>Go, Let's Encrypt</td>
</tr>
<tr>
<td><strong>Patrick</strong></td>
<td>CI/CD orchestration, build job management</td>
<td>Go, PubSub</td>
</tr>
<tr>
<td><strong>Monkey</strong></td>
<td>Code compilation in isolated containers</td>
<td>Docker, Go</td>
</tr>
<tr>
<td><strong>TNS</strong></td>
<td>Configuration storage with CRDT replication</td>
<td>go-ds-crdt</td>
</tr>
<tr>
<td><strong>Seer</strong></td>
<td>Service discovery, geographic routing, DNS</td>
<td>Kademlia DHT</td>
</tr>
<tr>
<td><strong>Hoarder</strong></td>
<td>Content-addressed storage and distribution</td>
<td>IPFS, Bitswap</td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

**Supporting Components:**

- **Sensors**: Real-time metrics collection and load balancing
- **Orbit**: Plugin system for platform extensions
- **Starlark**: Policy engine for automation rules

</div>

<br/>

<div align="center">

### Communication Layer

All services communicate over **libp2p** streams with **CBOR-encoded** messages, enabling:

</div>

<br/>

<table align="center">
<tr>
<td align="center">

✅ Automatic peer discovery via Kademlia DHT

</td>
<td align="center">

✅ NAT traversal and relay capabilities (Circuit Relay)

</td>
</tr>
<tr>
<td align="center">

✅ Transport-agnostic connections (TCP, QUIC, WebSocket)

</td>
<td align="center">

✅ Pub/sub messaging via GossipSub protocol

</td>
</tr>
<tr>
<td align="center">

✅ Efficient binary serialization (CBOR)

</td>
<td align="center">

✅ Custom RPC protocol on `/serviceName/v1` paths

</td>
</tr>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>Technology Stack</h2>
</div>

<br/>

<div align="center">

### Core Technologies

</div>

<table>
<thead>
<tr>
<th>Component</th>
<th>Technology</th>
<th>Version</th>
<th>Purpose</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Language</strong></td>
<td><a href="https://go.dev/">Go</a></td>
<td>1.25+</td>
<td>Platform services (pure Go, no CGO)</td>
</tr>
<tr>
<td><strong>Networking</strong></td>
<td><a href="https://libp2p.io/">libp2p</a></td>
<td>0.42+</td>
<td>P2P networking (DHT, GossipSub, Relay)</td>
</tr>
<tr>
<td><strong>Runtime</strong></td>
<td><a href="https://wazero.io/">wazero</a></td>
<td>1.9+</td>
<td>WebAssembly JIT compilation</td>
</tr>
<tr>
<td><strong>Storage</strong></td>
<td><a href="https://github.com/hsanjuan/ipfs-lite">IPFS Lite</a></td>
<td>Latest</td>
<td>Content-addressed storage (Bitswap)</td>
</tr>
<tr>
<td><strong>Database</strong></td>
<td><a href="https://github.com/cockroachdb/pebble">Pebble</a></td>
<td>2.x</td>
<td>LSM-tree embedded KV store</td>
</tr>
<tr>
<td><strong>Replication</strong></td>
<td><a href="https://github.com/ipfs/go-ds-crdt">go-ds-crdt</a></td>
<td>Latest</td>
<td>CRDT-based conflict-free synchronization</td>
</tr>
<tr>
<td><strong>Containers</strong></td>
<td>Docker</td>
<td>Latest</td>
<td>Isolated build environments</td>
</tr>
<tr>
<td><strong>TLS</strong></td>
<td>ACME / Let's Encrypt</td>
<td>Latest</td>
<td>Automatic certificate provisioning</td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

### Supported Languages

</div>

<table align="center">
<thead>
<tr>
<th>Language</th>
<th>Compiler</th>
<th>Target</th>
</tr>
</thead>
<tbody>
<tr>
<td>Go</td>
<td>TinyGo</td>
<td>WebAssembly</td>
</tr>
<tr>
<td>Rust</td>
<td>rustc</td>
<td>WebAssembly</td>
</tr>
<tr>
<td>AssemblyScript</td>
<td>asc</td>
<td>WebAssembly</td>
</tr>
</tbody>
</table>

<br/>

---

<br/>

<div align="center">
  <h2>Learning Resources</h2>
</div>

<br/>

<div align="center">

### Official Documentation

</div>

<table>
<thead>
<tr>
<th>Resource</th>
<th>Description</th>
<th>Link</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Documentation</strong></td>
<td>Complete guides, API reference, tutorials</td>
<td><a href="https://tau.how">tau.how</a></td>
</tr>
<tr>
<td><strong>Quick Start</strong></td>
<td>Step-by-step deployment guide</td>
<td><a href="https://taubyte.com/blog/be-competitive-in-few-minutes/">Deploy Guide</a></td>
</tr>
<tr>
<td><strong>Architecture</strong></td>
<td>Deep dive into platform design</td>
<td><a href="https://taubyte.com/blog/introduction-to-taubyte/">Introduction</a></td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

### Community & Support

</div>

<table>
<thead>
<tr>
<th>Platform</th>
<th>Purpose</th>
<th>Link</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Discord</strong></td>
<td>Real-time chat, community support</td>
<td><a href="https://discord.gg/KbN3KN7kpQ">Join Discord</a></td>
</tr>
<tr>
<td><strong>YouTube</strong></td>
<td>Video tutorials, demos, walkthroughs</td>
<td><a href="https://youtube.com/@taubyte">Taubyte Channel</a></td>
</tr>
<tr>
<td><strong>GitHub Discussions</strong></td>
<td>Q&A, feature requests, ideas</td>
<td><a href="https://github.com/taubyte/tau/discussions">Discussions</a></td>
</tr>
<tr>
<td><strong>GitHub Issues</strong></td>
<td>Bug reports, issue tracking</td>
<td><a href="https://github.com/taubyte/tau/issues">Issues</a></td>
</tr>
</tbody>
</table>

<br/>

<div align="center">

### Additional Resources

- **[taubyte.com](https://taubyte.com)** - Official website and blog
- **[Example Projects](https://github.com/taubyte-test)** - Sample applications and templates
- **[API Reference](https://tau.how/api)** - Complete API documentation

</div>

<br/>

---

<br/>

<div align="center">
  <h2>Contributing</h2>
</div>

<br/>

<p align="center">
We welcome contributions from the community. To get started:
</p>

<br/>

<div align="center">

1. **Fork** the repository on GitHub
2. **Clone** your fork: `git clone https://github.com/YOUR_USERNAME/tau`
3. **Build** the project: `cd tau && go build`
4. **Test** changes using Dream
5. **Submit** a pull request with a clear description

</div>

<br/>

<p align="center">
See <a href="CONTRIBUTING.md">CONTRIBUTING.md</a> for detailed guidelines on code style, testing, and review process.
</p>

<br/>

---

<br/>

<div align="center">
  <h2>License</h2>
  <p>Taubyte is open source software released under the <a href="LICENSE">BSD 3-Clause License</a>.</p>
</div>

<br/>

---

<br/>

<div align="center">
  <h2>Built With</h2>
</div>

<br/>

<table align="center">
<thead>
<tr>
<th>Technology</th>
<th>Purpose</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://go.dev/">Go</a></td>
<td>Core platform implementation</td>
</tr>
<tr>
<td><a href="https://libp2p.io/">libp2p</a></td>
<td>Peer-to-peer networking</td>
</tr>
<tr>
<td><a href="https://wazero.io/">wazero</a></td>
<td>WebAssembly runtime</td>
</tr>
<tr>
<td><a href="https://ipfs.tech/">IPFS</a></td>
<td>Content-addressed storage</td>
</tr>
</tbody>
</table>

<br/>
<br/>

---

<br/>

<div align="center">
  <h2>Ready to get started?</h2>
  <br/>
  <a href="#getting-started">
    <img src="https://img.shields.io/badge/Download%20Dream%20Desktop-4A90E2?style=for-the-badge&logo=download&logoColor=white" alt="Download Dream Desktop">
  </a>
  &nbsp;&nbsp;
  <a href="https://tau.how">
    <img src="https://img.shields.io/badge/Read%20the%20Docs-00B4D8?style=for-the-badge&logo=read-the-docs&logoColor=white" alt="Read the Docs">
  </a>
  &nbsp;&nbsp;
  <a href="https://discord.gg/KbN3KN7kpQ">
    <img src="https://img.shields.io/badge/Join%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Join Discord">
  </a>
</div>

<br/>
<br/>
