<div align="center">
 <p align="center">
  <a href="https://discord.gg/KbN3KN7kpQ">
    <img src="images/discord-btn.png" alt="Join our Discord" width="150">
  </a>
  &nbsp;&nbsp;
  <a href="https://tau.how">
    <img src="images/docs-btn.png" alt="Read the Docs" width="150">
  </a>
  &nbsp;&nbsp;
  <a href="https://console.taubyte.com">
    <img src="images/sandbox-btn.png" alt="Try our Sandbox" width="150">
  </a>
</p>

<p align="center">
  <img src="images/logo.png" alt="Tau Logo" width="100">
  &nbsp;&nbsp;
  <img src="images/logo.png" alt="Tau Logo" width="100">
</p>


[![Release](https://img.shields.io/github/v/release/taubyte/tau?style=flat-square)](https://github.com/taubyte/tau/releases/latest)
[![License](https://img.shields.io/github/license/taubyte/tau?style=flat-square)](LICENSE)
[![Go Report Card](https://goreportcard.com/badge/github.com/taubyte/tau)](https://goreportcard.com/report/github.com/taubyte/tau)

# Distributed Cloud Platform

**Self-hosted • Git-native • P2P architecture**

</div>

## What is Taubyte?

**Taubyte** is a complete, _self-hosted cloud platform_ that you can deploy with a **single binary**.

It provides all the infrastructure components needed to build and run modern applications, including:

- **Serverless functions**
- **Static hosting**
- **Databases**
- **Storage**
- **Messaging**
- **CI/CD pipelines**

All of this works _without relying on third-party cloud providers_, giving you full control over your deployments.

### Key Differentiators

<div align="center">

|                                                                                                                                                                         |                                                                                                                                                            |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Git-Native by Design**                                                                                                                                                | **Peer-to-Peer Architecture**                                                                                                                              |
| Infrastructure is defined in Git repositories.<br>Every commit triggers automatic deployment.<br>No API calls, no infrastructure-as-code tools, no manual provisioning. | Built on libp2p, nodes automatically discover each other, handle failures, and distribute content.<br>No central coordination, no single point of failure. |
| **WebAssembly Runtime**                                                                                                                                                 | **Content-Addressed Storage**                                                                                                                              |
| Applications run in sandboxed WebAssembly environments.<br>Fast cold starts (~10ms) and near-native performance.                                                        | Files are stored by cryptographic hash (IPFS).<br>Automatic deduplication, parallel distribution, and integrity verification.                              |
| **Local-to-Production Parity**                                                                                                                                          | **Zero Dependencies**                                                                                                                                      |
| Development environments run the exact same services as production.<br>No mocking, no simulation, no environmental drift.                                               | Single static binary with no external dependencies.<br>No Kubernetes, no orchestration complexity—just one binary.                                         |

</div>

## Core Features

**Serverless Functions**  
Event-driven compute with HTTP, pub/sub, and P2P triggers.  
Compiled to WebAssembly for security and portability.

**Static Hosting**  
Serve websites with automatic HTTPS certificates via Let's Encrypt.  
Global edge distribution included for fast access.

**Databases**  
Key-value stores with application or global scope.  
CRDT-based replication ensures conflict-free synchronization.

**Object Storage**  
S3-compatible storage with content addressing.  
Automatic deduplication and multi-node distribution.

**Messaging**  
Pub/sub channels using GossipSub protocol.  
Enables asynchronous communication between services and functions.

**Edge Distribution**  
Geographic routing based on node location.  
Traffic automatically directed to nearest healthy instance.

**Custom Domains**  
Bring your own domain with automatic TLS provisioning.  
DNS and certificate management handled automatically.

**CI/CD Pipeline**  
Git webhooks trigger builds in isolated Docker containers.  
Artifacts stored in content-addressed storage.

**Plugin System**  
Extend platform capabilities with Orbit plugins.  
Add integrations without modifying core services.

### Technology Highlights

_Modern, proven technologies built into Taubyte_

<div align="center">

|                                                                                                                                                                                                                                           |                                                                                                                                                                                                                                                                                                |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **WebAssembly & Runtime**                                                                                                                                                                                                                 | **Distributed Systems**                                                                                                                                                                                                                                                                        |
| • **[wazero](https://wazero.io/)** - Pure Go WebAssembly runtime with JIT compilation<br>• WASI Support - WebAssembly System Interface<br>• ~10ms cold starts for near-instant initialization                                             | • **[CRDT](https://github.com/ipfs/go-ds-crdt)** - Conflict-free replicated data types<br>• **[Pebble](https://github.com/cockroachdb/pebble)** - LSM-tree storage (RocksDB-style)<br>• **[Kademlia DHT](https://en.wikipedia.org/wiki/Kademlia)** - Distributed hash table for peer discovery |
| **P2P Networking**                                                                                                                                                                                                                        | **Additional Tools & Support**                                                                                                                                                                                                                                                                 |
| • **[libp2p](https://libp2p.io/)** - Modular P2P networking stack<br>• GossipSub - Efficient pub/sub messaging<br>• Circuit Relay - NAT traversal<br>• **[IPFS Lite](https://github.com/hsanjuan/ipfs-lite)** - Content-addressed storage | • Monitoring, metrics, and plugins for extending platform capabilities<br>• Built-in support for CI/CD pipelines and local-to-production parity<br>• Ensures reliable, high-performance deployments                                                                                            |

</div>

## Example Applications

_See real-world applications built with Taubyte_

<!-- TODO: Add real example applications with screenshots and links -->

## Getting Started

### Local Development with Dream

The recommended way to start with Taubyte is **Dream**—a complete cloud environment that runs on your local machine.

<div align="center">

|                                                                                                                                                                                                                                                                                                                                                                 |                                                                                                         |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **Option 1: Dream Desktop**<br>**Recommended**<br><br>Graphical interface for managing local cloud instances.<br><br>**Download:**<br>• Linux: [Download](https://github.com/taubyte/dream/releases/latest)<br>• Windows: [Download](https://github.com/taubyte/dream/releases/latest)<br>• macOS: [Download](https://github.com/taubyte/dream/releases/latest) | **Option 2: Dream CLI**<br>**For automation & CI/CD**<br><br>`npm install -g @taubyte/dream`<br>`dream` |

</div>

## Setup Instructions

<details>
<summary><h3>Step 1: Configure Local DNS</h3></summary>

Dream requires a DNS entry to function properly. Add the following to your system's hosts file:

<div align="center">

| Operating System | File Path                               | Entry                         |
| ---------------- | --------------------------------------- | ----------------------------- |
| Linux / macOS    | `/etc/hosts`                            | `127.0.0.1 hal.computers.com` |
| Windows          | `C:\Windows\System32\drivers\etc\hosts` | `127.0.0.1 hal.computers.com` |

</div>

This allows Dream to handle requests as if it were a real cloud deployment.

</details>

<details>
<summary><h3>Step 2: Create a Universe</h3></summary>

Launch Dream Desktop and create a new universe.

**What is a Universe?**  
A universe is an isolated Taubyte cloud instance running locally. It includes all platform services (Gateway, Substrate, Storage, Auth, Build services) and behaves identically to a production deployment.

<div align="center">

| Type           | Use Case                         | Persistence     |
| -------------- | -------------------------------- | --------------- |
| **Ephemeral**  | Quick testing, experimentation   | Deleted on exit |
| **Persistent** | Active development, project work | Saved to disk   |

</div>

Name your universe (e.g., "development") and click Create.

</details>

<details>
<summary><h3>Step 3: Connect to Web Console</h3></summary>

Navigate to **[console.taubyte.com](https://console.taubyte.com)** in your browser.

The console automatically detects your local Dream instance and establishes a connection.

</details>

<details>
<summary><h3>Step 4: Create a Project</h3></summary>

In the console:

- Click **New Project**
- Enter a project name (e.g., "my-application")
- Connect to a GitHub repository (or create a new one)
- Click Create

The console generates a `.taubyte` directory in your repository with initial configuration.

</details>

<details>
<summary><h3>Step 5: Add Resources</h3></summary>

Taubyte organizes applications into composable resources.

<div align="center">

| Resource Type | Purpose                                  | Scope                 |
| ------------- | ---------------------------------------- | --------------------- |
| **Function**  | Serverless compute with event triggers   | Application           |
| **Website**   | Static file hosting with CDN             | Application           |
| **Database**  | Key-value data storage                   | Application or Global |
| **Storage**   | Object storage for files and assets      | Application or Global |
| **Messaging** | Pub/sub channels for async communication | Application or Global |
| **Service**   | Long-running background processes        | Application           |
| **Library**   | Shared code modules                      | Application           |
| **Domain**    | Custom DNS with automatic TLS            | Application or Global |
| **SmartOps**  | Event-driven automation workflows        | Application           |

</div>

**Example: Creating a Function**

1. Select **Function** from resource types
2. Configure:
   - Name: `api`
   - Language: Go / Rust / AssemblyScript
   - Trigger: HTTP
   - Path: `/api/*`
   - Method: GET, POST
3. Click Create

The console generates a code template in your repository under `functions/api/`.

</details>

<details>
<summary><h3>Step 6: Deploy Your Application</h3></summary>

Commit and push your changes:

```bash
git add .
git commit -m "Add API function"
git push origin main
```

**What happens next:**

1. GitHub sends a webhook to your Dream instance
2. Patrick (CI/CD service) receives the webhook and creates a build job
3. Monkey (build service) clones your repository and compiles code to WebAssembly
4. Hoarder (storage service) stores the compiled artifacts
5. TNS (configuration service) updates with the new deployment
6. Substrate (runtime service) loads and executes your function

Access your function at: `http://hal.computers.com/api/your-endpoint`

</details>

## Production Deployment

### Using Spore Drive (Recommended)

Spore Drive automates Taubyte installation and configuration across multiple servers.

**[Section to be added - Spore Drive installation and setup]**

## Manual Installation

For manual deployment or custom configurations:

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

**Configuration Options:**

<div align="center">

| Parameter    | Description                  | Example                      |
| ------------ | ---------------------------- | ---------------------------- |
| `--name`     | Your domain name             | `cloud.mycompany.com`        |
| `--services` | Services to run on this node | `all` or `gateway,substrate` |
| `--ip`       | Public IP address            | `203.0.113.10`               |
| `--swarm`    | Join P2P network             | Flag (no value)              |

</div>

**Start the node:**

```bash
tau start
```

## Multi-Node Architecture

For production deployments, distribute services across specialized nodes:

<div align="center">

| Node Type     | Services           | Purpose                                       |
| ------------- | ------------------ | --------------------------------------------- |
| **Edge**      | Gateway, Substrate | Handle incoming traffic and execute functions |
| **Build**     | Patrick, Monkey    | Process CI/CD builds                          |
| **Storage**   | Hoarder, TNS       | Store content and configuration               |
| **Discovery** | Seer, Auth         | Service discovery and authentication          |

</div>

Each node automatically discovers and communicates with others via **libp2p**.

## Platform Architecture

### Core Services

<div align="center">

| Service       | Role                                               | Technology           |
| ------------- | -------------------------------------------------- | -------------------- |
| **Gateway**   | HTTP/HTTPS ingress, routing, load balancing        | Go, ACME, L7 routing |
| **Substrate** | WebAssembly runtime, function execution            | wazero, WASI         |
| **Auth**      | GitHub OAuth, webhook management, TLS certificates | Go, Let's Encrypt    |
| **Patrick**   | CI/CD orchestration, build job management          | Go, PubSub           |
| **Monkey**    | Code compilation in isolated containers            | Docker, Go           |
| **TNS**       | Configuration storage with CRDT replication        | go-ds-crdt           |
| **Seer**      | Service discovery, geographic routing, DNS         | Kademlia DHT         |
| **Hoarder**   | Content-addressed storage and distribution         | IPFS, Bitswap        |

</div>

**Supporting Components:**

- **Sensors**: Real-time metrics collection and load balancing
- **Orbit**: Plugin system for platform extensions
- **Starlark**: Policy engine for automation rules

### Communication Layer

All services communicate over **libp2p** streams with **CBOR-encoded** messages, enabling:

<div align="center">

|                                                          |                                                         |
| -------------------------------------------------------- | ------------------------------------------------------- |
| ✅ Automatic peer discovery via Kademlia DHT             | ✅ NAT traversal and relay capabilities (Circuit Relay) |
| ✅ Transport-agnostic connections (TCP, QUIC, WebSocket) | ✅ Pub/sub messaging via GossipSub protocol             |
| ✅ Efficient binary serialization (CBOR)                 | ✅ Custom RPC protocol on `/serviceName/v1` paths       |

</div>

## Technology Stack

### Core Technologies

<div align="center">

| Component       | Technology                                         | Version | Purpose                                  |
| --------------- | -------------------------------------------------- | ------- | ---------------------------------------- |
| **Language**    | [Go](https://go.dev/)                              | 1.25+   | Platform services (pure Go, no CGO)      |
| **Networking**  | [libp2p](https://libp2p.io/)                       | 0.42+   | P2P networking (DHT, GossipSub, Relay)   |
| **Runtime**     | [wazero](https://wazero.io/)                       | 1.9+    | WebAssembly JIT compilation              |
| **Storage**     | [IPFS Lite](https://github.com/hsanjuan/ipfs-lite) | Latest  | Content-addressed storage (Bitswap)      |
| **Database**    | [Pebble](https://github.com/cockroachdb/pebble)    | 2.x     | LSM-tree embedded KV store               |
| **Replication** | [go-ds-crdt](https://github.com/ipfs/go-ds-crdt)   | Latest  | CRDT-based conflict-free synchronization |
| **Containers**  | Docker                                             | Latest  | Isolated build environments              |
| **TLS**         | ACME / Let's Encrypt                               | Latest  | Automatic certificate provisioning       |

</div>

### Supported Languages

<div align="center">

| Language       | Compiler | Target      |
| -------------- | -------- | ----------- |
| Go             | TinyGo   | WebAssembly |
| Rust           | rustc    | WebAssembly |
| AssemblyScript | asc      | WebAssembly |

</div>

## Learning Resources

### Official Documentation

<div align="center">

| Resource          | Description                               | Link                                                                    |
| ----------------- | ----------------------------------------- | ----------------------------------------------------------------------- |
| **Documentation** | Complete guides, API reference, tutorials | [tau.how](https://tau.how)                                              |
| **Quick Start**   | Step-by-step deployment guide             | [Deploy Guide](https://taubyte.com/blog/be-competitive-in-few-minutes/) |
| **Architecture**  | Deep dive into platform design            | [Introduction](https://taubyte.com/blog/introduction-to-taubyte/)       |

</div>

### Community & Support

<div align="center">

| Platform               | Purpose                              | Link                                                      |
| ---------------------- | ------------------------------------ | --------------------------------------------------------- |
| **Discord**            | Real-time chat, community support    | [Join Discord](https://discord.gg/KbN3KN7kpQ)             |
| **YouTube**            | Video tutorials, demos, walkthroughs | [Taubyte Channel](https://youtube.com/@taubyte)           |
| **GitHub Discussions** | Q&A, feature requests, ideas         | [Discussions](https://github.com/taubyte/tau/discussions) |
| **GitHub Issues**      | Bug reports, issue tracking          | [Issues](https://github.com/taubyte/tau/issues)           |

</div>

### Additional Resources

- **[taubyte.com](https://taubyte.com)** - Official website and blog
- **[Example Projects](https://github.com/taubyte-test)** - Sample applications and templates
- **[API Reference](https://tau.how/api)** - Complete API documentation

## Contributing

We welcome contributions from the community. To get started:

1. Fork the repository on GitHub
2. Clone your fork: `git clone https://github.com/YOUR-USERNAME/tau`
3. Build the project: `cd tau && go build`
4. Test changes using Dream
5. Submit a pull request with a clear description

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

---

## License

Released under the [BSD 3-Clause License](LICENSE).

---

## Built With

<div align="center">

| Technology                   | Purpose                      |
| ---------------------------- | ---------------------------- |
| [Go](https://go.dev/)        | Core platform implementation |
| [libp2p](https://libp2p.io/) | Peer-to-peer networking      |
| [wazero](https://wazero.io/) | WebAssembly runtime          |
| [IPFS](https://ipfs.tech/)   | Content-addressed storage    |

</div>

## Get Started

[![Download Dream Desktop](https://img.shields.io/badge/Download%20Dream%20Desktop-4A90E2?style=for-the-badge&logo=download&logoColor=white)](https://github.com/taubyte/dream/releases/latest)
[![Read the Docs](https://img.shields.io/badge/Read%20the%20Docs-00B4D8?style=for-the-badge&logo=read-the-docs&logoColor=white)](https://tau.how)
[![Join Discord](https://img.shields.io/badge/Join%20Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/KbN3KN7kpQ)
