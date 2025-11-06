# Chess3 Discord Server Template

## 🚀 Quick Setup Guide

Discord templates can only include channels and categories. Roles, permissions, and bots must be configured manually. This guide makes it as fast as possible.

---

## Step 1: Create Server from Template

### Option A: Use This Template Link (After You Create It)

1. **Create your Discord server first** with basic structure
2. **Go to Server Settings** → **Server Template**
3. **Create Template** and share the link here
4. Others can use that link to clone your server structure

### Option B: Manual Quick Setup (15 minutes)

Follow the steps below to set up everything quickly.

---

## Step 2: Create Roles (5 minutes)

**Go to Server Settings → Roles → Create Role**

Copy-paste these role configurations:

### 1. 👑 Founder
```
Name: Founder
Color: #9945FF
Permissions: Administrator
Display separately: ✓
Allow anyone to mention: ✗
```

### 2. 🛡️ Moderator
```
Name: Moderator
Color: #14F195
Permissions: Manage Messages, Kick Members, Ban Members, Manage Nicknames, Timeout Members, View Audit Log
Display separately: ✓
Allow anyone to mention: ✓
```

### 3. 💎 Diamond Holder
```
Name: Diamond Holder (10+ NFTs)
Color: #00D4FF
Permissions: Default
Display separately: ✓
Allow anyone to mention: ✗
```

### 4. 🏆 Platinum Holder
```
Name: Platinum Holder (5-9 NFTs)
Color: #E5E4E2
Permissions: Default
Display separately: ✓
Allow anyone to mention: ✗
```

### 5. ♟️ Pawnz Holder
```
Name: Pawnz Holder (1-4 NFTs)
Color: #FFD700
Permissions: Default
Display separately: ✓
Allow anyone to mention: ✗
```

### 6. 🎨 Content Creator
```
Name: Content Creator
Color: #FF6B9D
Permissions: Embed Links, Attach Files, Use External Emojis
Display separately: ✓
Allow anyone to mention: ✗
```

### 7. 🌟 Ambassador
```
Name: Ambassador
Color: #FFA500
Permissions: Default
Display separately: ✓
Allow anyone to mention: ✗
```

### 8-12. Notification Roles (Don't display separately)
```
🔔 Announcements - #808080
📢 Mint Alerts - #808080
🎮 Tournament Alerts - #808080
🎁 Giveaway Alerts - #808080
📰 News - #808080
```

---

## Step 3: Create Channel Structure (5 minutes)

**Right-click server name → Create Category**

### Copy this structure exactly:

```
📌 WELCOME & INFO
├─ 📜 rules (text, read-only)
├─ 👋 welcome (text, read-only)
├─ 📢 announcements (announcement, read-only)
├─ 🎉 events (text, read-only)
├─ ❓ faq (text, read-only)
└─ 🔗 links (text, read-only)

💬 COMMUNITY
├─ 💭 general-chat (text)
├─ 🎨 media-share (text)
├─ 🤖 bot-commands (text)
├─ 🎮 gaming (text)
├─ 🎵 music-lounge (voice)
└─ 🗣️ general-voice (voice)

♟️ CHESS DISCUSSION
├─ 📊 chess-strategy (text)
├─ 🏆 tournaments (text)
├─ 📺 game-analysis (text)
└─ 🎯 chess-puzzles (text)

💎 NFT HOLDERS ONLY
├─ 🔐 verification (text)
├─ 💬 holder-chat (text, holders only)
├─ 📊 holder-announcements (announcement, holders only)
├─ 🗳️ governance (forum, holders only)
├─ 💰 staking-rewards (text, holders only)
├─ 🎁 holder-giveaways (text, holders only)
├─ 💎 diamond-lounge (text, diamond only)
└─ 🎤 holder-voice (voice, holders only)

🛠️ SUPPORT & HELP
├─ 🆘 support (forum)
├─ 🐛 bug-reports (forum)
├─ 💡 suggestions (forum)
└─ 📝 feedback (text)

🎨 CREATORS & COMMUNITY
├─ 🖼️ fan-art (text)
├─ 📹 content-creators (text, creator role only)
├─ 🌟 ambassador-chat (text, ambassador role only)
└─ 🤝 partnerships (text, read-only)

🎯 ENGAGEMENT
├─ 🎁 giveaways (text, read-only)
├─ 🎲 games (text)
├─ 📊 polls (text, read-only)
└─ 🏅 leaderboard (text, read-only)

🔧 STAFF ONLY
├─ 🛡️ mod-chat (text, mods only)
├─ 📋 mod-logs (text, mods only)
├─ 👑 admin-chat (text, founders only)
└─ 📊 analytics (text, founders only)
```

---

## Step 4: Set Channel Permissions (3 minutes)

### Quick Permission Settings:

**For Read-Only Channels** (rules, welcome, announcements, etc.):
```
@everyone: View Channel ✓, Send Messages ✗
Moderator: View Channel ✓, Send Messages ✓
```

**For Holder-Only Channels** (holder-chat, governance, etc.):
```
@everyone: View Channel ✗
Pawnz Holder: View Channel ✓, Send Messages ✓
Platinum Holder: View Channel ✓, Send Messages ✓
Diamond Holder: View Channel ✓, Send Messages ✓
```

**For Diamond Lounge**:
```
@everyone: View Channel ✗
Diamond Holder: View Channel ✓, Send Messages ✓
```

**For Staff Channels**:
```
@everyone: View Channel ✗
Moderator: View Channel ✓, Send Messages ✓
Founder: View Channel ✓, Send Messages ✓
```

---

## Step 5: Install Bots (2 minutes)

Click these links and add to your server:

1. **MEE6** (Leveling): https://mee6.xyz/
2. **Collab.Land** (NFT Verification): https://collab.land/
3. **Dyno** (Moderation): https://dyno.gg/
4. **Carl-bot** (Reaction Roles): https://carl.gg/

---

## Step 6: Configure Bots

### MEE6 Setup
1. Go to https://mee6.xyz/dashboard
2. Select your server
3. **Levels**: Enable XP system
4. **Moderation**: Enable auto-mod (spam, caps, links)
5. **Welcome**: Set welcome message in #welcome

### Collab.Land Setup
1. Type `/collabland-config` in any channel
2. Select "Token Gating"
3. **Blockchain**: Solana
4. **Contract Address**: [Your Candy Machine ID]
5. **Role Mapping**:
   - 1-4 NFTs → Pawnz Holder
   - 5-9 NFTs → Platinum Holder
   - 10+ NFTs → Diamond Holder

### Carl-bot Setup (Reaction Roles)
1. Go to https://carl.gg/dashboard
2. Select your server
3. **Reaction Roles** → Create new
4. Create in #roles channel:
   - 🔔 → Announcements
   - 📢 → Mint Alerts
   - 🎮 → Tournament Alerts
   - 🎁 → Giveaway Alerts
   - 📰 → News

---

## Step 7: Add Content to Key Channels

### #rules
```markdown
# 📜 Server Rules

Welcome to Chess3 Official! Please read and follow these rules:

**1. Be Respectful**
Treat everyone with respect. No harassment, hate speech, or discrimination.

**2. No Spam**
Don't spam messages, links, or mentions. Use #bot-commands for bot spam.

**3. No Scams or Phishing**
Never share suspicious links. We'll never DM you asking for wallet info.

**4. English Only in Main Channels**
Keep main channels in English. Use DMs for other languages.

**5. No NSFW Content**
Keep all content safe for work.

**6. Follow Discord ToS**
All Discord Terms of Service apply: https://discord.com/terms

**7. Listen to Moderators**
Moderator decisions are final.

**Violations may result in warnings, timeouts, or permanent bans.**

React with ✅ to accept the rules and gain access to the server!
```

### #welcome
```markdown
# 👋 Welcome to Chess3 Official!

We're building the next 3volution of competitive chess on Solana.

## 🎯 Quick Start:
1️⃣ Read <#rules> and react to accept
2️⃣ Check out <#faq> for common questions
3️⃣ Verify your NFTs in <#verification> (if you're a holder)
4️⃣ Choose notification roles in <#roles>
5️⃣ Say hi in <#general-chat>!

## 📚 Important Links:
🌐 **Website**: https://chessalienz.vercel.app
📖 **Whitepaper**: https://chess3-1.gitbook.io/chess3/
🐦 **Twitter**: https://x.com/CHESSALIENZ
♟️ **Mint**: https://chessalienz.vercel.app/mint.html
🔍 **Collection**: [Magic Eden link when live]

## 💎 NFT Holders:
Head to <#verification> to verify your Chessalienz: Pawnz NFTs and unlock exclusive channels!

Let's revolutionize chess together! ♟️🚀
```

### #links
```markdown
# 🔗 Official Links

## 🌐 Website & Mint
**Website**: https://chessalienz.vercel.app
**Mint Page**: https://chessalienz.vercel.app/mint.html

## 📖 Documentation
**Whitepaper**: https://chess3-1.gitbook.io/chess3/
**How to Mint Guide**: https://chess3-1.gitbook.io/chess3/community/how-to-mint-guide

## 🐦 Social Media
**Twitter/X**: https://x.com/CHESSALIENZ
**Discord**: [This server]

## 🛒 Marketplaces
**Magic Eden**: [Link when live]
**Tensor**: [Link when live]

## 🔍 Blockchain
**Solscan**: [Collection link when live]
**Solana Explorer**: https://explorer.solana.com

## 💼 Wallets
**Phantom**: https://phantom.app
**Solflare**: https://solflare.com
**Backpack**: https://backpack.app
**Magic Eden Wallet**: https://wallet.magiceden.io

⚠️ **Always verify URLs before connecting your wallet!**
```

### #verification
```markdown
# 🔐 NFT Verification

Verify your Chessalienz: Pawnz NFTs to unlock holder-exclusive channels!

## How to Verify:

1️⃣ Click the **"Let's go!"** button below (from Collab.Land bot)
2️⃣ Connect your Solana wallet (Phantom, Solflare, etc.)
3️⃣ Sign the verification message
4️⃣ Your role will be automatically assigned!

## Holder Tiers:
💎 **Diamond Holder** (10+ NFTs) - All holder perks + Diamond Lounge
🏆 **Platinum Holder** (5-9 NFTs) - All holder perks
♟️ **Pawnz Holder** (1-4 NFTs) - Holder perks

## What You Get:
✅ Access to <#holder-chat>
✅ Exclusive <#holder-announcements>
✅ <#governance> voting rights
✅ <#staking-rewards> access
✅ Holder-only <#holder-giveaways>
✅ Priority support

**Need help?** Ask in <#support>

---

*Your wallet address is never stored. Verification is secure and private.*
```

### #faq
```markdown
# ❓ Frequently Asked Questions

## General

**Q: What is Chess3?**
A: Chess3 is a play-to-earn chess platform built on Solana, starting with the Chessalienz: Pawnz NFT collection.

**Q: When is the mint?**
A: Mint date TBA. Follow <#announcements> and Twitter for updates!

**Q: What's the mint price?**
A: Starting at 3 SOL with a reverse auction (decreases 0.03 SOL every 60 seconds with no mint).

**Q: How many can I mint?**
A: Maximum 10 per wallet.

## NFT Questions

**Q: How many NFTs in the collection?**
A: 5,000 unique Chessalienz: Pawnz NFTs.

**Q: What are the character roles?**
A: 21 unique roles! See the full list: https://chess3-1.gitbook.io/chess3/nft-collection/character-roles

**Q: What utility do NFTs have?**
A: Platform access, tournaments, governance, staking, reduced fees, and more!

## Technical

**Q: Which blockchain?**
A: Solana

**Q: Which wallets are supported?**
A: Phantom, Solflare, Backpack, Magic Eden Wallet

**Q: How do I verify my NFT in Discord?**
A: Go to <#verification> and follow the instructions!

**Q: Where can I trade after mint?**
A: Magic Eden and Tensor (links in <#links>)

## Platform

**Q: When does the platform launch?**
A: Q4 2025 for beta. See roadmap: https://chess3-1.gitbook.io/chess3/roadmap/development-phases

**Q: What is $GBTZ?**
A: The Chess3 platform token (Gambitz). Details: https://chess3-1.gitbook.io/chess3/economics/tokenomics

**More questions?** Ask in <#general-chat> or <#support>!
```

---

## Step 8: Server Settings

**Server Settings → Overview**:
- **Verification Level**: Medium (verified email required)
- **Explicit Content Filter**: Scan messages from all members
- **DM Settings**: Disable DMs from server members

**Server Settings → Moderation**:
- **2FA Requirement**: Required for moderators

**Server Settings → Community**:
- Enable Community Server
- Set rules channel: #rules
- Set updates channel: #announcements

---

## Step 9: Create Server Template

Once everything is set up:

1. **Server Settings** → **Server Template**
2. Click **"Create Template"**
3. Name: "Chess3 Official Server"
4. Description: "Complete server setup for Chess3 NFT project"
5. **Generate Template Link**
6. Share the link with your team or save for future use

---

## 🎉 You're Done!

Your Chess3 Discord server is now fully set up!

### Final Checklist:
- [ ] All roles created with correct colors
- [ ] All channels and categories created
- [ ] Permissions set for holder channels
- [ ] Bots installed and configured
- [ ] Welcome message posted
- [ ] Rules posted
- [ ] FAQ posted
- [ ] Links posted
- [ ] Verification working
- [ ] Test with a secondary account

### Next Steps:
1. Invite your team (badt0shi, broccoly)
2. Assign Founder roles
3. Test verification with a holder wallet
4. Announce Discord on Twitter
5. Add Discord link to website
6. Start engaging with your community!

---

**Need help? Refer back to DISCORD-SETUP.md for detailed explanations of each feature.**
