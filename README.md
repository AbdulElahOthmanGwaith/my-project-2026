# NexusAI Platform - Open Source AI Orchestration Platform

<div align="center">
  <img src="docs/images/logo.png" alt="NexusAI Logo" width="200"/>
  
  **Interactive web platform for interacting with multiple AI models**
  
  [![GitHub Stars](https://img.shields.io/github/stars/nexus-ai/platform)](https://github.com/nexus-ai/platform/stargazers)
  [![GitHub Issues](https://img.shields.io/github/issues/nexus-ai/platform)](https://github.com/nexus-ai/platform/issues)
  [![License](https://img.shields.io/github/license/nexus-ai/platform)](https://github.com/nexus-ai/platform/blob/main/LICENSE)
  [![CI/CD Pipeline](https://img.shields.io/github/actions/workflow/status/nexus-ai/platform/ci-pipeline.yml)](https://github.com/nexus-ai/platform/actions)
</div>

## Key Features

### 🤖 Multi-AI Integration
- Full support for OpenAI GPT-4 and GPT-3.5
- Integration with Anthropic Claude
- Support for Hugging Face local and cloud models
- Unified interface for switching models during conversation

### 🔄 Fully Automated CI/CD System
- Automatic build on every code change
- Automated unit and integration tests
- Continuous security scanning for packages
- Automatic deployment on merge to main branch

### 💬 Modern Interactive Interface
- Eye-friendly dark design
- Markdown and rich text support
- Automatic code syntax highlighting
- Export conversations in multiple formats

### 🔐 Security and Privacy
- Encrypted stored API keys
- Multi-authentication support
- User data isolation
- Full transparency in source code

## Quick Start

### Requirements
- Docker and Docker Compose
- Git
- Required API keys (OpenAI, Anthropic)

### Installation in Three Steps

```bash
# 1. Clone the repository
git clone https://github.com/nexus-ai/platform.git
cd nexus-ai-platform

# 2. Copy environment file and edit it
cp .env.example .env
# Edit .env with your API keys

# 3. Run the platform
docker-compose up -d
```

After running, open your browser at `http://localhost:3000`

## Project Structure

```
nexus-ai-platform/
├── .github/
│   └── workflows/          # CI/CD files
│       ├── ci-pipeline.yml
│       └── cd-deploy.yml
├── client/                 # Frontend (Next.js)
│   ├── src/
│   │   ├── app/           # App Router
│   │   ├── components/    # Components
│   │   ├── lib/           # Utilities
│   │   └── hooks/         # React Hooks
│   ├── public/            # Static assets
│   └── Dockerfile
├── server/                 # Backend (FastAPI)
│   ├── app/
│   │   ├── api/          # Endpoints
│   │   ├── core/         # Core configurations
│   │   ├── models/       # Data models
│   │   ├── services/     # AI services
│   │   └── main.py       # Entry point
│   └── Dockerfile
├── infrastructure/         # Infra configurations
│   ├── docker-compose.yml
│   └── nginx.conf
├── docs/                   # Documentation
└── README.md
```

## Contributing

We welcome your contributions! Please read the [Contributing Guide](docs/CONTRIBUTING.md) to get started.

## License

MIT License - See [LICENSE](LICENSE) file for details.

## Support

- 📧 Email: support@nexus-ai.io
- 💬 Discord: [Join our community](https://discord.gg/nexus-ai)
- 📖 Documentation: [docs.nexus-ai.io](https://docs.nexus-ai.io)
