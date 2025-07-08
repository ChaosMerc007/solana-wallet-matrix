# 🧠 Solana Wallet Matrix & QR Compatibility Report

Status: Needs review
Submitted By:: Divine Mockors
For:: Superteam x Venta Bounty
Date: July 8, 2025

## 🔍 Project Goal

To compare leading Solana wallets by features and evaluate their support for **Solana Pay QR code payments**. This helps developers, merchants, and users choose the right wallet for payments, staking, NFT management, and overall UX.

## 📊 Wallet Feature Matrix

User research findings, competitor analysis, and design opportunities.

| Wallet | Platform(s) | Staking | NFTs | dApp Access | Multisig/Hardware | Solana Pay QR |
| --- | --- | --- | --- | --- | --- | --- |
| **Phantom** | Browser Extension, Mobile | ✅ | ✅ | ✅ | Ledger | ✅ |
| **Solflare** | Web, Extension, Mobile | ✅ | ✅ | ✅ | Ledger, Keystone | ✅ |
| **Slope** | Mobile | ⬜ | ✅ | ✅ | ❌ | ✅ |
| **Glow** | Mobile | ⬜ | ✅ | ✅ | ❌ | ✅ |
| **Exodus** | Desktop, Mobile | ✅ | ✅ | ❌ | Trezor | ✅ |
| **Trust Wallet** | Browser Extension, Mobile | ⬜ | ✅ | ✅ | ❌ | ✅ |
| **Ledger** | Hardware | ✅ | ✅ | ✅* | ✅ | ❌ |

## 🧪 Solana Pay QR Evaluation

I tested each wallet or researched for its ability to **scan and process QR payments** using Solana Pay. The flow, clarity, and experience were rated on a scale from 1 to 5 as represented below:

| Wallet | Solana Pay Flow Steps | UX Rating | Screenshots |
| --- | --- | --- | --- |
| **Phantom** | Open app → Tap QR → Scan → Approve | ⭐⭐⭐⭐⭐ | ✅ |
| **Solflare** | Open app → Scan → Review Tx → Confirm | ⭐⭐⭐⭐⭐ | ✅ |
| **Slope** | Camera scan → Opens app → Confirm | ⭐⭐⭐⭐ | ❌ |
| **Glow** | Scan via Safari → Redirect to app → Confirm | ⭐⭐⭐⭐ | ✅ |
| **Exodus** | Solana Pay tab → Scan → Approve | ⭐⭐⭐⭐ | ✅ |
| **Trust** | Use dApp browser → Scan QR → Confirm | ⭐⭐⭐ | ❌ |
| **Ledger** | Not supported | — | ❌ |

## 🖼 **Phantom Wallet**

![Phantom’s QR scanner interface before scanning Solana Pay code.](d2a2cbb7-e160-4c74-8ab8-4f613457a3cc.png)

Phantom’s QR scanner interface before scanning Solana Pay code.

![Phantom 2 QR Stage.jpg](2aa93291-a024-473f-97c5-88721f272493.png)

Phantom’s QR scanner interface before scanning Solana Pay code. 

![Phantom – Confirm screen showing 0.01744 SOL with address and fee.](71d42081-ddd8-4f68-b93b-3c2e000bce50.png)

Phantom – Confirm screen showing 0.01744 SOL with address and fee.

## 🖼 **Exodus Wallet**

![Exodus – Payment screen showing Solana Pay entry point.](840d8648-4305-48e2-8577-2660401cc5d1.png)

Exodus – Payment screen showing Solana Pay entry point.

![Exodus – Payment screen after Solana Pay QR scan.](14cc3623-4b3c-4e7e-8781-3d5e28157919.png)

Exodus – Payment screen after Solana Pay QR scan.

![Exodus – Payment screen after Solana Pay QR scan.](Exodus_Slide_to_Pay.jpg)

Exodus – Payment screen after Solana Pay QR scan.

## 🖼 Glow **Wallet**

![Glow 1.jpg](Glow_1.jpg)

Glow – Home screen showing Solana Pay entry point

![Glow – Payment screen showing Solana Pay with QR scanner option](Glow_2.jpg)

Glow – Payment screen showing Solana Pay with QR scanner option

![Glow – Payment confirmation ](6012416996051896872.jpg)

Glow – Payment confirmation 

## 🖼 Softlare **Wallet**

![Softlare’s Home screen. No instant QR scanner found](Softlare_1.jpg)

Softlare’s Home screen. No instant QR scanner found

![Softlare’s Payment Screen showing Solana Pay QR scan option](Softlare_2_pay_QR.jpg)

Softlare’s Payment Screen showing Solana Pay QR scan option

## 🔍 Key Observations

- **Phantom** is the best overall performer. It has the full features, excellent Solana Pay flow, strong mobile UX.
- **Exodus** is an underrated pick for mobile-first Solana Pay transactions.
- Softlare is a high performer too but it lacks instantly accessible QR scanner. And the gas fees are higher than other wallets
- **Glow** and **Slope** are lightweight and optimized for mobile but lack advanced config.
- **Ledger** prioritizes hardware security but doesn't natively support Solana Pay.

## 🏆 Wallet Recommendations

| Use Case | Recommended Wallet | Reason |
| --- | --- | --- |
| Best All-Round Experience | **Phantom** | Clean UI, strong dApp ecosystem, QR ready |
| Most Secure | **Solflare + Ledger** | Staking + multisig + hardware |
| Best for Mobile | **Glow** / **Slope** | Lightweight, snappy mobile-first designs |
| Merchant Friendly | **Exodus (Mobile)** | Built-in Solana Pay scanner & flow |

## 📎 Attached Files

- 🗂 **Solana Wallet Matrix Spreadsheet (.xlsx):**
    
    [Solana_Wallet_Feature_Matrix.xlsx](Solana_Wallet_Feature_Matrix.xlsx)
    
- 📸 **Screenshots Folder**
    
    [1izSH6JzFgbG4rtJoXu_lsz7gT-ZEkA03?usp=sharing](https://drive.google.com/drive/folders/1izSH6JzFgbG4rtJoXu_lsz7gT-ZEkA03?usp=sharing)
    

## Additional testing notes

### **Testing Methodology**

All wallets were tested using the latest available versions (as of July 2025) on both iOS and Android (where applicable). Solana Pay functionality was assessed by generating test QR codes linked to devnet payments and monitoring how wallets responded in terms of scan speed, transaction clarity, and ease of approval.

### General Findings:

- **Phantom and Solflare** immediately recognized and parsed Solana Pay QR codes without requiring a browser redirect. They offered clean transaction previews and quick confirmations.
- I noticed higher transaction fees with Softlare as seen in the screenshot where a transfer was made from Softlare to Glow
- **Glow** relied on Safari/iOS deep linking. It worked but introduced minor friction with app switching. It however works very smoothly on Android devices.
- **Trust Wallet** required users to manually open a dApp browser, making QR scanning less intuitive.
- **Exodus Mobile** was the most beginner-friendly for Solana Pay, with a dedicated section for QR payments. Also the easiest to setup.
- **Ledger** had no native Solana Pay support and requires pairing with another interface (e.g., Solflare or Phantom desktop).

### Issues Encountered:

- Some wallets (Glow, Slope) struggled to parse QR codes unless the camera was centered precisely.
- Phantom’s desktop extension version did not support camera QR scanning. Only the mobile app worked.
- Cross-app redirection behavior varied on Android vs iOS, particularly affecting Trust Wallet and Glow.

### Recommendations:

- Merchants should prefer **Phantom, Solflare, or Exodus** for smoother point-of-sale QR usage.
- Mobile-first wallets like **Slope and Glow** are promising but need UI polish for enterprise use.
- **Ledger users** should not rely on QR-based payments unless paired with a companion wallet.

These notes were compiled after 2 days of wallet usage, covering 7 wallets, 3 devices, and 15+ Solana Pay test scans.

## ✅ Submission Notes

This report was compiled through hands-on testing, personal research using the resources I could get, and wallet documentation. Designed to support both the Solana ecosystem and merchant onboarding efforts.