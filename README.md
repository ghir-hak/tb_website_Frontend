<div align="center">

[![Release](https://img.shields.io/github/release/taubyte/tau.svg?color=blue)](https://github.com/taubyte/tau/releases)
[![License](https://img.shields.io/github/license/taubyte/tau?color=blue)](LICENSE)

</div>

<div align="center">
  <img src="images/gifs/banner.png" width="100%">
</div>

<div align="center">
  <a href="https://taubyte.com/doc"><img src="images/gifs/documentation.png" width="32%"></a>
  <a href="https://discord.gg/KbN3KN7kpQ"><img src="images/gifs/discord.png" width="32%"></a>
  <a href="https://taubyte.com/book-a-demo"><img src="images/gifs/demo.png" width="32%"></a>
</div>

Tau is an open-source, Git-native platform-as-a-service that empowers development teams to build, deploy, and scale applications with full infrastructure autonomy. With built-in AI capabilities, Tau seamlessly integrates intelligent features into your development workflow. Unlike traditional cloud providers, Tau is fully self-hosted while providing the same capabilities as Vercel, Netlify, Cloudflare, and other major platforms—now enhanced with AI-powered development and deployment tools.

<div align="center">

| Development Environment                                                                                                                                                                                                                        |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <div align="center"><img src="images/gifs/dreamcli.gif" width="32%" ><img src="images/gifs/5px.png"><img src="images/gifs/dreamdesktop.gif" width="32%" ><img src="images/gifs/5px.png"><img src="images/gifs/connect.gif" width="32%" ></div> |

</div>

<div align="center">

| Build Your Application                                                                                                                                                                                                                          |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <div align="center"><img src="images/gifs/newproject.gif" width="32%" ><img src="images/gifs/5px.png"><img src="images/gifs/newfunction.gif" width="32%" ><img src="images/gifs/5px.png"><img src="images/gifs/pushall.gif" width="32%" ></div> |

</div>

<div align="center">

| Deploy and Run                                                                                                                                                                                                                                  |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <div align="center"><img src="images/gifs/builds.gif" width="32%" ><img src="images/gifs/5px.png"><img src="images/gifs/runfunction.gif" width="32%" ><img src="images/gifs/5px.png"><img src="images/gifs/spore-drive.gif" width="32%" ></div> |

</div>

### Example Projects

<div align="center">
  <a href="https://youtu.be/RIdwJQB3Tk0"><img src="images/gifs/pixel.png" width="48%" style="border-radius: 15px; margin: 5px;"></a>
  <a href="https://youtu.be/gMTYh-gQLgA"><img src="images/gifs/tower.png" width="48%" style="border-radius: 15px; margin: 5px;"></a>
</div>

### The Hitchhiker's Guide To Taubyte

A fast paced video series to get you from 0 to hero in ono time.

<div align="center">
  <a href="https://www.youtube.com/watch?v=8FO1KiTE0FE"><img src="images/gifs/vid1.png" width="32%"></a>
  <a href="https://www.youtube.com/watch?v=ajdcUGd2SeE"><img src="images/gifs/vid2.png" width="32%"></a>
  <a href="https://www.youtube.com/watch?v=YyZHCBkjCOU"><img src="images/gifs/vid3.png" width="32%"></a>
</div>

<div align="center">
  <a href="https://www.youtube.com/watch?v=IDUI7a96gSw&t=10s"><img src="images/gifs/vid4.png" width="32%"></a>
  <a href="https://www.youtube.com/playlist?list=PLLKNB3tJrL9Y4nl0JnBhU2wHS4iWldUfh"><img src="images/gifs/vid5.png" width="32%"></a>
  <a href="https://www.youtube.com/playlist?list=PLLKNB3tJrL9Y4nl0JnBhU2wHS4iWldUfh"><img src="images/gifs/vid6.png" width="32%"></a>
</div>

### Core Features

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         CURRENT ARCHITECTURE                            │
└─────────────────────────────────────────────────────────────────────────┘

    ┌──────────────────────────────────────────────────────────────────┐
    │                    APPLICATION LAYER                             │
    │  • Serverless Functions  • Web Hosting  • Databases              │
    │  • Storage (IPFS)        • Messaging (MQTT)                      │
    └───────────────────────────────┬──────────────────────────────────┘
                                    │
    ┌───────────────────────────────┴───────────────────────────────────┐
    │                    DISTRIBUTED SERVICES                           │
    ├───────────────────────────────┬───────────────────────────────────┤
    │    DISTRIBUTED CORE           │      NETWORK LAYER                │
    │  • Seer (DNS)                 │  • P2P (libp2p)                   │
    │  • Gateway (Load Balancer)    │  • NAT Traversal                  │
    │  • Hoarder (Replication)      │  • Circuit Relay                  │
    │                               │  • Multi-Transport                │
    └───────────────────────────────┴───────────────────────────────────┘
                                    │
    ┌───────────────────────────────▼───────────────────────────────────┐
    │                    PLATFORM FOUNDATION                            │
    │  • Single Binary, Zero Dependencies  • Auto TLS/SSL               │
    │  • Minimal Configuration              • Orbit Plugin System       │
    │  • WebAssembly Runtime                                            │
    └───────────────────────────────────────────────────────────────────┘

    ┌──────────────────────────────────────────────────────────────────┐
    │                    DEVELOPER TOOLS                               │
    │  • Git-Native Infrastructure  • Local = Production               │
    │  • CI/CD Pipeline             • E2E Testing                      │
    │  • Spore Drive                                                   │
    └──────────────────────────────────────────────────────────────────┘
```

**Application Layer**

- [x] **Serverless Functions** - WebAssembly runtime supporting Rust, Go, and AssemblyScript with instant cold starts
- [x] **Web Hosting** - Deploy websites and SPAs with automatic routing and custom domains
- [x] **Databases** - Key-value store with encryption, regex matching, and configurable limits
- [x] **Storage** - Object storage with versioning, IPFS-backed content-addressed storage with deduplication
- [x] **Messaging** - Real-time pub/sub via MQTT and WebSocket protocols

**Developer Tools**

- [x] **Git-Native Infrastructure** - All infrastructure defined in Git as code, no API calls needed
- [x] **Local Equals Production** - Dream framework creates local cloud environments matching production
- [x] **CI/CD Pipeline** - Git-native workflow with automatic builds on commit/push
- [x] **E2E Testing** - Dream framework enables end-to-end testing of Tau projects
- [x] **Easy Deployment** - Spore Drive provides simple, automated deployment framework

**Distributed Core**

- [x] **Seer** - Distributed DNS service for automatic service discovery
- [x] **Gateway** - Intelligent load balancing and request routing
- [x] **Hoarder** - Automatic replication for databases and object storage

**Network Layer**

- [x] **Peer-to-Peer Networking** - Built on libp2p with automatic node discovery, self-healing networks, and dynamic routing
- [x] **NAT Traversal & Circuit Relay** - Nodes behind firewalls can join the cloud
- [x] **Transport Independent** - Support for TCP/IP, WebSocket, QUIC, and more

**Platform Foundation**

- [x] **Single Binary, Zero Dependencies** - One executable file, deploy anywhere
- [x] **Auto TLS/SSL** - Automatic certificate provisioning and renewal
- [x] **Minimal Configuration** - Built-in auto-discovery for nodes, services, and routing
- [x] **Extensible Platform** - Orbit plugin system for adding custom capabilities
- [x] **Portable Computing** - WebAssembly runtime enabling true portability and sandboxing

## Features Timeline

### Technical Achievements

- **Distributed Services Architecture** - Seer (DNS), Gateway (load balancing), Hoarder (replication)
- **Advanced Networking** - NAT traversal, circuit relay, and transport-independent protocols (TCP/IP, WebSocket, QUIC)
- **Content-Addressed Storage** - IPFS-backed distributed storage with automatic deduplication and parallel downloads
- **Portable Computing** - WebAssembly runtime enabling true portability and sandboxing

### Coming Soon

```
┌─────────────────────────────────────────────────────────────────────────┐
│                         UPCOMING FEATURES                               │
└─────────────────────────────────────────────────────────────────────────┘

    ┌──────────────────────────────────────────────────────────────────┐
    │              COMPUTING ENHANCEMENTS                              │
    │  • Container Support  • VM Support                               │
    └──────────────────────────────────────────────────────────────────┘

    ┌──────────────────────────────────────────────────────────────────┐
    │              APPLICATION ENHANCEMENTS                            │
    │  • GraphQL Gateway  • Enhanced AI Integration                    │
    └──────────────────────────────────────────────────────────────────┘

    ┌──────────────────────────────────────────────────────────────────┐
    │              CROSS-CUTTING ENHANCEMENTS                          │
    │  • Advanced Monitoring & Observability                           │
    │  • Zero-Trust Networking  • Advanced Encryption                  │
    └──────────────────────────────────────────────────────────────────┘

    ┌──────────────────────────────────────────────────────────────────┐
    │              DEPLOYMENT & WORKFLOW                               │
    │  • Multi-Cloud Orchestration  • Real-time Collaboration          │
    │  • Advanced CI/CD  • Edge Computing Enhancements                 │
    └──────────────────────────────────────────────────────────────────┘
```

**Computing Layer**

- **Container Support** - Native container runtime for computing workloads
- **Virtual Machine Support** - VM-based computing with portability guarantees

**AI & Integration**

- **Enhanced AI Integration** - Deeper AI capabilities built into the platform
- **GraphQL Support** - Native GraphQL API gateway and schema management

**Observability**

- **Advanced Monitoring & Observability** - Comprehensive metrics, tracing, and logging

**Security & Edge**

- **Enhanced Security Features** - Advanced encryption, zero-trust networking, and security policies
- **Edge Computing Enhancements** - Improved edge deployment and data locality

**Orchestration & Workflow**

- **Multi-Cloud Orchestration** - Deploy and manage across multiple cloud providers
- **Real-time Collaboration** - Multi-developer workflows and live collaboration tools
- **Advanced CI/CD Features** - Enhanced pipeline capabilities and deployment strategies

---

## Connect With Us

- **Instagram**: [@dtaubyte](https://instagram.com/dtaubyte)
- **X (Twitter)**: [@dtaubyte](https://x.com/dtaubyte)
- **YouTube**: [Taubyte](https://youtube.com/@taubyte)
- **Discord**: [Join our community](https://discord.gg/KbN3KN7kpQ)
- **Documentation**: [taubyte.com/doc](https://taubyte.com/doc)

---

<div align="center">
  <p>Built with ❤️ by the Taubyte team</p>
  <p>Star us on <a href="https://github.com/taubyte/tau">GitHub</a> if you find Tau useful!</p>
</div>
