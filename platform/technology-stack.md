# Technology Stack

## Overview

Chessalienz Pawnz is built on a modern, scalable, and secure technology stack leveraging the Solana blockchain and industry-leading web technologies.

**Production Status**: ✅ **LIVE ON MAGIC EDEN** (December 2025)

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
- **Vite 5.0.0**: Modern build tool and development server
- **Vanilla JavaScript**: Pure JS implementation (no React framework)
- **CSS3**: Custom styling with animations
- **HTML5**: Semantic markup structure

### **Build Tools**
- **vite-plugin-node-polyfills**: Node.js API browser compatibility
- **Browser Polyfills**: crypto, buffer, stream, assert for Solana integration

### **Solana Integration**
- **Browser-based wallet connection**: Direct wallet adapter integration
- **Client-side signing**: All transaction signing in browser
- **Magic Eden compatibility**: Optimized for marketplace integration

### **Storage**
- **Irys (Arweave)**: Permanent NFT metadata storage
- **IPFS**: Decentralized image hosting
- **Pinata**: IPFS pinning service

---

## 🖥️ Backend Stack

### **Runtime & Framework**
- **Magic Block**: Primary development platform
- **Magic Block Solana SDK**: Blockchain integration
- **Sugar CLI**: Candy machine deployment tool
- **Node.js 20**: Development environment
- **TypeScript**: Configuration & scripts

### **Solana Libraries**
- **@solana/web3.js**: Blockchain interactions
- **@solana/spl-token**: Token transfers & management
- **Borsh 2.0.0**: Binary serialization
- **Magic Block APIs**: Backend services integration

### **Security & Middleware**
- **express-rate-limit**: Rate limiting (10 req/min)
- **cors**: Cross-origin resource sharing
- **dotenv**: Environment variable management
- **Magic Block Auth**: Authentication & authorization

### **API Endpoints**
```
N/A - Deployed via Magic Eden Marketplace
Direct candy machine interaction through Magic Eden
Application APIs hosted on Magic Block infrastructure
```

---

## 🚀 Infrastructure & Deployment

### **Marketplace & Minting**
- **Primary Marketplace**: Magic Eden
- **Minting Protocol**: Magic Eden Launchpad
- **Collection Management**: Magic Eden Creator Tools
- **Secondary Trading**: Magic Eden Marketplace
- **Analytics**: Magic Eden Insights Dashboard

### **Application Development**
- **Development Platform**: Magic Block
- **Framework**: Magic Block Solana SDK
- **Deployment**: Magic Block Infrastructure
- **Backend Services**: Magic Block Compute
- **Database**: Magic Block Storage Solutions

### **Frontend Hosting**
- **Platform**: Vercel
- **CDN**: Global edge network
- **SSL**: Automatic HTTPS
- **Deployment**: Git-based CI/CD
- **Environment**: Production + Preview branches

---

## 🔐 Security Stack

### **Candy Machine Security**
- **Metaplex Candy Machine V3**: Battle-tested minting protocol
- **Hidden Settings**: Art protection until reveal
- **Authority Control**: Creator wallet management
- **Immutable Supply**: Fixed 8,888 NFT collection

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
- **Local Testing**: Development environment validation
- **Sugar Validation**: Pre-deployment checks
- **Solana Explorer**: Transaction monitoring
- **Magic Eden Analytics**: Marketplace performance

---

## 🔄 Data Flow Architecture

### **Minting Flow**
```
User Wallet → Magic Eden → Candy Machine → Solana RPC → Blockchain
     ↓              ↓              ↓              ↓
Wallet Adapter   Marketplace   Transaction   Confirmation
     ↓              ↓              ↓              ↓
Select NFT       Sign TX        On-Chain      Success/Error
```

### **Application Flow**
```
User Interface → Magic Block → Solana RPC → Blockchain
       ↓             ↓              ↓           ↓
   Frontend App   Backend API   Transaction   State Update
       ↓             ↓              ↓           ↓
   User Action   Compute Logic  On-Chain     Real-time UI
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

### **Frontend (6 packages)**
```json
{
  "vite": "^5.0.0",
  "assert": "^2.1.0",
  "buffer": "^6.0.3",
  "crypto-browserify": "^3.12.0",
  "stream-browserify": "^3.0.0",
  "vite-plugin-node-polyfills": "^0.19.0"
}
```

### **Backend (Magic Block + Sugar CLI)**
```json
{
  "@magic-block/solana-sdk": "latest",
  "@metaplex-foundation/sugar": "latest",
  "@solana/web3.js": "^1.98.4",
  "typescript": "latest"
}
```

---

## 📚 Technical Documentation

### **Public Repositories**
- **NFT Collection**: [github.com/chess3official/chessalienz-pawnz-nft-collection](https://github.com/chess3official/chessalienz-pawnz-nft-collection)
- **Whitepaper**: [gitbook.com/chess3/whitepaper](https://gitbook.com/chess3/whitepaper)

### **Documentation**
- [Candy Machine Deployment Guide](https://developers.metaplex.com/candy-machine)
- [Magic Eden Creator Guide](https://docs.magiceden.io)
- [Magic Block Developer Docs](https://docs.magicblock.io)
- [Solana NFT Standards](https://docs.solana.com/nfts)

---

**Last Updated**: December 8, 2025
