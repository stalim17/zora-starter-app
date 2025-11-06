# Base Onboarding Checklist for Zora Starter App

Deploying the Zora Starter App on Base is straightforward if you keep a few key details in mind.  
This short checklist covers everything new builders should verify before shipping live.

---

### 1. Environment Setup
- Use the latest **Node LTS (v18+)** and **Next.js 14+** for compatibility.  
- Set `NEXT_PUBLIC_CHAIN_ID=8453` for Base mainnet, or `84532` for Base Sepolia testnet.  
- Add your RPC endpoint (Alchemy or QuickNode) as `NEXT_PUBLIC_RPC_URL`.

---

### 2. Wallet Integration
- Test with Coinbase Smart Wallet or MetaMask first.  
- Ensure `wagmi` or `rainbowkit` versions support Base network IDs.  
- Check the default chain switching logic; Base is often missing from initial configs.

---

### 3. Contract Deployment
- For local testing, deploy with `hardhat` using `--network base-sepolia`.  
- Verify contracts on **BaseScan** after deployment.  
- Always keep your collection’s metadata hosted on IPFS or Arweave.

---

### 4. UI Customization
- Update site title and favicon to reflect your project identity.  
- Replace the default mint function text (`"Mint NFT"`) with a clear call-to-action.  
- Add Base’s signature color `#0052FF` for brand consistency.

---

### 5. Pre-Launch Checklist
- ✅ RPC connection successful  
- ✅ Wallet connects + switch to Base automatically  
- ✅ Mint flow tested end-to-end  
- ✅ Metadata resolves onchain  
- ✅ Deployment verified on BaseScan  

---

### Final Note
The Starter App already lowers the barrier for creative builders.  
This checklist just helps make Base deployment smoother and repeatable for the next wave of creators.

> Build once, mint everywhere — but start on Base.
