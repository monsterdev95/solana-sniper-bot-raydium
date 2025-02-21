# Solana GRPC Ultra-Fast raydium sniper bot

This is a unmaintained and dirty PoC of using GRPC to detect newly launched tokens on Raydium and snipe them with the goal of being the first buy. Please feel free to use this in your own code. 

This bot buy tokens which only specific poolsize set on .env file and sell at specific pool size.
By default, this bot buy tokens whose mint address ends with 'pump' and has poolsize between 170 and 200 sol because such tokens are very safe and profitable.
![image](https://github.com/bigj-SVS/grpc-sniper/assets/173855326/1f4f4f54-d2fc-438e-a603-6aba1b641e1b)


# Requirements
This bot use the corvus's great grpc and rpc , so you don't need to purchase any expensive grpc or rpc service.

# Instructions
- Using the Solana CLI, generate a public-bundles.json keypair using the following command
`solana-keygen new --outfile ./public-bundles.json`(There is already this file exists)
![image](https://github.com/bigj-SVS/grpc-sniper/assets/173855326/a6624c17-4397-48f4-82ab-9b1940990b89)
- Move this file to your cloned grpc-sniper repo in the top-level parent directory
- Rename `.env.example` to `.env`
- Add your private key in base64 format which can be exported from either Phantom or derived from your JSON keypair for your wallet.

# Commands
- npm i
- npm run start
