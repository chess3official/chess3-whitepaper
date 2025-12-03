# Technology Stack

## Overview

Chessalienz Pawnz is built on a modern, scalable, and secure technology stack leveraging the Solana blockchain and industry-leading web technologies.

**Status**: ✅ **PRODUCTION READY** (December 2025)

---

## ⛓️ Blockchain Layer

### **Solana**
- **Network**: Solana Mainnet-Beta
- **RPC Provider**: Helius (Dedicated endpoint)
- **Token Standard**: SPL Token (Fungible & Non-Fungible)
- **Transaction Speed**: ~400ms confirmation time
- **Cost**: ~$0.00025 per transaction

### **Why Solana?**
- ✅ High throughput (65,000+ TPS)
- ✅ Low transaction costs
- ✅ Fast finality
- ✅ Proven NFT ecosystem
- ✅ Battle-tested security

---

## 🎨 Frontend Stack

### **Framework & Libraries**
- **Next.js 16.0.7**: React framework with server components
- **React 19.2.1**: UI library with latest features
- **TypeScript**: Type-safe development
- **Tailwind CSS 3.4**: Utility-first styling

### **Solana Integration**
- **@solana/web3.js 1.98.4**: Core Solana library
- **@solana/spl-token 0.4.14**: Token operations
- **@solana/wallet-adapter-react 0.15.39**: Wallet connectivity
- **@solana/wallet-adapter-wallets 0.19.37**: Multi-wallet support

### **Metaplex Integration**
- **@metaplex-foundation/js 0.20.1**: NFT metadata & minting
- **@metaplex-foundation/mpl-candy-machine 6.1.0**: Candy Machine v3
- **@metaplex-foundation/mpl-token-metadata 3.4.0**: NFT metadata standard
- **@metaplex-foundation/umi 1.4.1**: Unified Metaplex interface

### **Wallet Support**
- **Phantom**: Primary wallet (99% of users)
- **Solflare**: Alternative wallet
- **Backpack**: Gaming-focused wallet
- **Torus**: Web2-style onboarding (disabled due to security)
- **WalletConnect**: Cross-chain support (disabled due to security)

### **Storage**
- **Irys (Arweave)**: Permanent NFT metadata storage
- **IPFS**: Decentralized image hosting
- **NFT.Storage**: Backup storage solution

---

## 🖥️ Backend Stack

### **Runtime & Framework**
- **Node.js 20**: LTS runtime
- **Express.js**: Web server framework
- **TypeScript**: Type-safe backend code

### **Solana Libraries**
- **@solana/web3.js**: Blockchain interactions
- **@solana/spl-token**: Token transfers & management
- **Borsh 2.0.0**: Binary serialization

### **Security & Middleware**
- **express-rate-limit**: Rate limiting (10 req/min)
- **cors**: Cross-origin resource sharing
- **dotenv**: Environment variable management

### **API Endpoints**
```
GET  /health                    - Health check
POST /api/presale/buy          - Purchase presale pass
GET  /api/presale/recovery     - Admin recovery
GET  /api/presale/stats        - Presale statistics
GET  /api/mint-status          - Mint status
POST /api/check-eligibility    - Check mint eligibility
POST /api/mint                 - Mint NFT
```

---

## 🚀 Infrastructure & Deployment

### **Frontend Hosting**
- **Platform**: Vercel
- **CDN**: Global edge network
- **SSL**: Automatic HTTPS
- **Deployment**: Git-based CI/CD
- **Environment**: Production + Preview branches

### **Backend Hosting**
- **Platform**: Railway
- **Runtime**: Node.js 20 (Nixpacks)
- **Scaling**: Automatic horizontal scaling
- **WAF**: Web Application Firewall
- **Monitoring**: Built-in metrics & logs

### **Domain & DNS**
- **DNS Provider**: Cloudflare
- **SSL/TLS**: Full encryption
- **DDoS Protection**: Enterprise-grade

---

## 🔐 Security Stack

### **Automated Security Scanning**
- **Snyk**: Dependency vulnerability scanning
- **CodeQL**: Static application security testing
- **OSSF Scorecard**: Security health metrics
- **Dependabot**: Automated dependency updates

### **CI/CD Security**
- **GitHub Actions**: Automated workflows
- **Security scans**: On every push
- **Weekly audits**: Comprehensive scans
- **Automated alerts**: Real-time notifications

### **Infrastructure Security**
- **Railway WAF**: Request filtering & blocking
- **Environment isolation**: Secure secrets management
- **HTTPS only**: Encrypted traffic
- **Rate limiting**: DDoS mitigation

---

## 📊 Development Tools

### **Version Control**
- **Git**: Source control
- **GitHub**: Repository hosting
- **Branch Protection**: Required reviews

### **Package Management**
- **npm**: Node package manager
- **package-lock.json**: Dependency locking
- **Automated updates**: Dependabot

### **Code Quality**
- **ESLint**: JavaScript linting
- **Prettier**: Code formatting
- **TypeScript**: Type checking

### **Testing & Monitoring**
- **Manual testing**: Pre-deployment checks
- **Error tracking**: Runtime error monitoring
- **Transaction logs**: Recovery & debugging

---

## 🔄 Data Flow Architecture

### **Minting Flow**
```
User Wallet → Frontend UI → Backend API → Solana RPC → Blockchain
                ↓              ↓              ↓
           Wallet Adapter   Validation   Transaction
                ↓              ↓              ↓
           Sign TX        Rate Limit    Confirmation
                ↓              ↓              ↓
           Submit         Recovery Log   Success/Error
```

### **Metadata Flow**
```
NFT Metadata → Irys/Arweave → Permanent Storage
     ↓              ↓                ↓
  JSON File    Upload API      IPFS Hash
     ↓              ↓                ↓
  Images       Verification    On-Chain Link
```

---

## 🌐 Network Configuration

### **RPC Endpoints**
- **Primary**: Helius Mainnet (Dedicated)
- **Fallback**: Public Solana RPC
- **Rate Limits**: 100 req/sec (Helius)

### **Blockchain Networks**
- **Production**: Solana Mainnet-Beta
- **Development**: Solana Devnet
- **Testing**: Local validator

---

## 📦 Key Dependencies

### **Frontend (44 packages)**
```json
{
  "next": "^16.0.7",
  "react": "^19.2.1",
  "@solana/web3.js": "^1.98.4",
  "@metaplex-foundation/js": "^0.20.1",
  "tailwindcss": "^3.4.1"
}
```

### **Backend (15 packages)**
```json
{
  "express": "latest",
  "@solana/web3.js": "^1.98.4",
  "@solana/spl-token": "^0.4.14",
  "express-rate-limit": "latest",
  "cors": "latest"
}
```

---

## 🔮 Future Enhancements

### **Planned Upgrades**
- [ ] WebSocket support for real-time updates
- [ ] Advanced caching layer
- [ ] GraphQL API
- [ ] Mobile app (React Native)
- [ ] Enhanced analytics dashboard

### **Blockchain Improvements**
- [ ] Compressed NFTs (cNFTs)
- [ ] State compression
- [ ] Cross-program invocations (CPI)
- [ ] Token-2022 standard

---

## 📚 Technical Documentation

### **Public Repositories**
- **Frontend**: [github.com/chess3official/pawnz-mint-ui](https://github.com/chess3official/pawnz-mint-ui)
- **Backend**: [github.com/chess3official/chessalienz-pawnz-mint](https://github.com/chess3official/chessalienz-pawnz-mint)

### **Documentation**
- [Security Audit Report](https://github.com/chess3official/chessalienz-pawnz-mint/blob/main/SECURITY-AUDIT-REPORT.md)
- [Snyk Findings](https://github.com/chess3official/pawnz-mint-ui/blob/main/SNYK-FINDINGS.md)
- [Setup Guide](https://github.com/chess3official/chessalienz-pawnz-mint/blob/main/THIRD-PARTY-AUDIT-SETUP.md)

---

## 🎯 Performance Metrics

### **Frontend**
- **First Contentful Paint**: < 1.5s
- **Time to Interactive**: < 3.0s
- **Lighthouse Score**: 90+

### **Backend**
- **API Response Time**: < 200ms
- **Transaction Processing**: < 500ms
- **Uptime**: 99.9%

### **Blockchain**
- **Transaction Confirmation**: ~400ms
- **Success Rate**: 99%+
- **Cost per Mint**: ~0.002 SOL

---

**Last Updated**: December 3, 2025
