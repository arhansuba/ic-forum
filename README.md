# IC-Forum
IC-Forum is a decentralized forum platform powered by the ICP Chain Fusion, integrating with multiple smart contracts to provide a seamless and interactive user experience. The platform allows users to post questions, provide answers, upvote content, and swap tokens.

Table of Contents
Introduction
Features
Project Structure
Installation
Usage
Configuration
Contracts
Testing
Contributing
License
Introduction
IC-Forum aims to create a decentralized forum platform where users can interact, share knowledge, and participate in discussions securely and transparently. By leveraging ICP Chain Fusion and integrating various smart contracts, IC-Forum ensures a robust and scalable solution.

Features
Decentralized Forum: Users can post questions, answers, and upvote content.
Token Integration: Users can swap tokens and manage their balances.
Smart Contract Integration: Multiple contracts for various functionalities.
User-friendly Interface: Easy-to-use frontend for interacting with the platform.
Project Structure

ic-forum/
├── .devcontainer/
├── Front-end/
│   ├── components/
│   │   ├── Answer.tsx
│   │   ├── AnswerEditor.tsx
│   │   ├── Answers.tsx
│   │   ├── AuthButton.tsx
│   │   ├── BalanDetails.tsx
│   │   ├── Navbar.tsx
│   │   ├── Question.tsx
│   │   ├── QuestionEditor.tsx
│   │   ├── Questions.tsx
│   │   ├── TokenSwapper.tsx
│   │   ├── Upvote.tsx
│   │   ├── Username.tsx
│   ├── hooks/
│   │   ├── contracts/
│   │   │   ├── useAmmContract.ts
│   │   │   ├── useAmmDetails.ts
│   │   │   ├── useForumContract.ts
│   │   │   ├── useGoflowContract.ts
│   │   │   ├── useMaticContract.ts
│   │   │   ├── useSwap.ts
│   │   ├── useAddAnswer.ts
│   │   ├── useAddApprove.ts
│   │   ├── useAddMint.ts
│   │   ├── useAddQuestion.ts
│   │   ├── useAddUpvote.ts
│   │   ├── useAnswers.ts
│   │   ├── useBalance.ts
│   │   ├── useEvents.ts
│   │   ├── useQuestions.ts
│   │   ├── useUpvotes.ts
│   ├── lib/
│   │   ├── accounts.md
│   │   ├── number-utils.ts
│   ├── pages/
│   │   ├── question/
│   │   │   └── [id].tsx
│   │   ├── _app.tsx
│   │   ├── amm.tsx
│   │   ├── index.tsx
│   ├── public/
│   │   ├── favicon.ico
│   │   ├── polygon-logo.png
│   │   ├── vercel.svg
│   ├── styles/
│   │   ├── Home.module.css
│   │   └── globals.css
│   ├── .eslintrc.json
│   ├── .gitignore
│   ├── next-env.d.ts
│   ├── next.config.js
│   ├── package-lock.json
│   ├── package.json
│   ├── theme.ts
│   └── tsconfig.json
├── canisters/
├── contracts/
│   ├── Amm.sol
│   ├── Forum.sol
│   ├── Matic.sol
│   └── OurToken.sol
├── lib/
├── packages/
├── scripts/
│   ├── deploy-forum.ts
│   └── deploy-test-forum.ts
├── .gitignore
├── Caddyfile
├── Cargo.lock
├── Cargo.toml
├── README.md
├── deploy.sh
├── dfx.json
├── foundry.toml
Installation
To get started with IC-Forum, follow these steps:

Clone the repository:

git clone https://github.com/arhansuba/ic-forum.git
cd ic-forum
Install dependencies for the front-end:

cd Front-end
npm install
Usage
Running the Front-end
To run the front-end application:


cd Front-end
npm start
Configuration
The configuration for various hooks and contracts is stored in the hooks/contracts directory. Adjust the configurations as needed to match your setup.

Contracts
The smart contracts are located in the contracts directory. The main contracts include:

Amm.sol: Automated Market Maker contract.
Forum.sol: Core forum functionalities contract.
Matic.sol: Contract for Matic token integration.
OurToken.sol: Custom token contract for the forum.
Testing
To run tests for the contracts:


cd contracts
npm test
Contributing
We welcome contributions to IC-Forum! Please open an issue or submit a pull request on GitHub.

License
This project is licensed under the MIT License. See the LICENSE file for details.
