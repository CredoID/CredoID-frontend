

# CredoID-frontend

OVERVIEW

CredoID is a decentralized identity and KYC reuse protocol built on the Stellar ecosystem. This frontend application provides users with a secure and intuitive interface to manage their digital identity, complete KYC verification once, and reuse that verification across multiple applications without resubmitting personal documents.
The frontend serves as the Identity Wallet and Verifier Dashboard, allowing users to upload identity documents, receive verifiable credentials, manage identity NFTs, and share proof of verification with trusted applications.
It also enables KYC providers and integrators to interact with the platform through a transparent and decentralized interface powered by Soroban smart contracts and decentralized storage using IPFS.
The application is designed to support users, KYC verifiers, fintech applications, and DeFi protocols while ensuring privacy, security, and interoperability across the ecosystem.


Key Features
 Decentralized Identity Wallet
   Users can create and manage a decentralized identity linked to their Stellar wallet.
 KYC Document Upload
    Users upload identity documents (PDF or images) to be verified by trusted KYC providers.
Verifiable Credential Management
 After verification, users receive a reusable digital credential stored off-chain and anchored on-chain.
Identity NFT Management
  A proof-of-verification NFT is minted to represent successful identity verification.
Verifier Dashboard
 Trusted KYC providers can review documents, approve identities, and issue credentials.
App Integration Verification
  External applications can request identity verification from the user's wallet.
Secure Wallet Authentication
 Authentication is performed via non-custodial wallet signatures.
Real-Time Status Updates
 Users can track the status of verification requests and credentials.
Privacy-Preserving Identity Sharing
 Apps can verify a user’s status without accessing raw documents.
Responsive and Accessible Design
 Optimized for desktop and mobile devices.


  Tech Stack
 Framework-Next.js (App Router)
Language -TypeScript
Styling -Tailwind CSS
State Management-React Hooks and Context API
Blockchain - Stellar wallet integrations
Smart Contracts- Soroban
Decentralized Storage-IPFS

 📁 Project Structure
 
.
├── public/ 
│   ├── images/
│   └── icons/
│

├── src/
│   ├── app/                    
│   │   ├── dashboard/
│   │   ├── wallet/
│   │   ├── verifier/
│   │   └── api/
│   │
│   ├── components/            
│   │   ├── wallet/
│   │   ├── identity/
│   │   ├── verifier/
│   │   ├── forms/
│   │   └── layout/
│   │
│   ├── data/                  
│   │
│   ├── hooks/               
│   │   ├── useWallet.ts
│   │   ├── useIdentity.ts
│   │   └── useCredential.ts
│   │
│   ├── lib/                    
│   │   ├── stellar.ts
│   │   ├── ipfs.ts
│   │   ├── api.ts
│   │   └── helpers.ts
│   │
│   ├── context/                
│   │
│   ├── services/              
│   │   ├── identityService.ts
│   │   ├── credentialService.ts
│   │   └── verifierService.ts
│   │
│   ├── styles/                 
│   │
│   ├── types/                  
│   │
│   └── App.css                 
│
├── middleware.ts               
├── .gitignore
├── CONTRIBUTING.md
├── README.md
├── components.json             
├── eslint.config.mjs
├── next.config.ts
├── package.json
├── package-lock.json
└── LICENSE

 Installation & Setup Prerequisites
Before running the project, ensure the following tools are installed:
* Node.js 18+
* npm or yarn
* Stellar wallet (Freighter recommended)


   Testing
This project includes unit tests, integration tests, and end-to-end tests to ensure reliability and security.
Run all tests: npm test
Run tests with coverage report: npm run test:coverage
Run tests in watch mode:npm run test:watch


  Quick Setup
Install dependencies and pre-commit hooks:
npm install
npm run prepare

Run CI checks locally:
npm run lint
npm run test
npm run build

   Useful Links
Stellar Development Foundation Developer Docs
[https://developers.stellar.org](https://developers.stellar.org)

Soroban Smart Contract Docs
[https://soroban.stellar.org/docs](https://soroban.stellar.org/docs)

Next.js Documentation
[https://nextjs.org/docs](https://nextjs.org/docs)

IPFS Documentation
[https://docs.ipfs.tech](https://docs.ipfs.tech)



 Security Considerations
The frontend follows best practices for decentralized identity systems:
* No personal documents are stored on-chain
* Identity credentials are stored on IPFS
* Only hashes are anchored on Stellar
* Wallet-based authentication prevents centralized login risks
* Verifier registry prevents unauthorized KYC issuers


Contributions are welcome 🚀
1. Fork the repository
2. Create a new feature branch- git checkout -b feature/my-feature
3. Commit your changes with descriptive messages- git commit -m "Add credential wallet UI"
4. Push your branch: git push origin feature/my-feature
5. Open a Pull Request


 


