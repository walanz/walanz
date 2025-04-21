<p align="center">
  <img src="./public/logo-128.png" width="128" height="128" alt="Walanz Logo">
</p>

<h1 align="center">Walanz</h1>

<p align="center">Multi-chain Ethereum Balance Checker</p>

<div align="center">
  <a href="#features">Features</a> •
  <a href="#components">Components</a> •
  <a href="#getting-started">Getting Started</a> •
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#license">License</a> •
  <a href="./README-zh.md">中文文档</a>
</div>

<img src="./public/1400x560-banner.png" width="100%" alt="Walanz Banner">

---

## Features

- ✅ **Multi-chain Support**: Query ETH balances across numerous Ethereum-compatible chains
- ✅ **Batch Address Queries**: Check multiple wallet addresses simultaneously 
- ✅ **Real-time Price Conversion**: Automatic conversion to USD and CNY
- ✅ **Multiple Platforms**: Browser extension and API service available
- ✅ **Block Explorer Integration**: Direct links to block explorers for detailed information

## Components

### 🧩 Extension

Chrome extension for quick balance checks directly from your browser.

- Single & batch address queries
- Flexible blockchain selection
- Intuitive interface with clear balance display
- Real-time price conversions

[Extension Guide →](./extension/README.md)

### 🚀 Service

RESTful API service for programmatic balance checking.

- Multiple chain support via viem
- Serverless architecture optimized for Vercel
- Complete API with Swagger documentation
- Batch operations for efficiency

[Service Documentation →](./service/README.md)

## Getting Started

### Extension Installation

1. Download from Chrome Web Store or build from source
2. Click the Walanz icon in your browser toolbar
3. Enter Ethereum addresses and select chains to query

### API Usage

```bash
# Example API call to check balances
curl -X POST https://walanz.vercel.app/addresses/balances \
  -H "Content-Type: application/json" \
  -d '{"addresses":["0x123..."], "chains":["ethereum", "optimism"]}'
```

## Tech Stack

- **Frontend**: React, TypeScript, TailwindCSS
- **Backend**: NestJS, TypeScript
- **Blockchain**: Viem for multi-chain interactions
- **Deployment**: Vercel for serverless hosting

## License

[MIT License](LICENSE)