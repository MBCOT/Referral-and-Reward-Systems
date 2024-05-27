# Overview Document for Referral and Reward Systems

## Play to Earn with Gaming, Gambling, and User Interactions Systems or dApps

### Introduction

This document provides an in-depth overview of the referral and reward systems designed for a decentralized application (dApp) ecosystem, with a particular focus on gaming, gambling, and user interactions and activities based dApps. The referral system encourages user engagement by rewarding those who invite new users, while the reward system incentivizes participation through various activities within gaming and gambling platforms or any other system or dApp. These systems are independent but interact to enhance overall user benefits and system effectiveness.

### Referral System

#### Objectives

- Encourage users to invite friends to the dApp.
- Reward both the referrer and the referred user.
- Enhance user engagement in gaming and gambling dApps.

#### Key Features

- **Decentralization:** Options for full or partial decentralization.
- **Identity Tokens:** Serve as referral tokens containing user wallet addresses.
- **Smart Contracts:** Manage token issuance and reward distribution.

#### Implementation Approaches

1. **Fully Decentralized:**
   - All processes are handled via smart contracts on the blockchain.
   - Pros: High security, no central authority.
   - Cons: High complexity, increased development effort.

2. **Partially Decentralized:**
   - Central authority issues referral tokens.
   - Rewards are distributed through smart contracts.
   - Pros: Reduced complexity, easier to manage.
   - Cons: Slightly less secure, relies on central authority for initial token distribution.

#### Referral Process

1. **Token Creation and Distribution:**
   - Central authority or smart contract creates a large number of referral tokens.
   - Users obtain referral tokens from the central authority or buy them on a smart contract.

2. **Inviting Friends:**
   - User sends a referral link containing the Identity Token to friends.
   - Friend registers with the dApp and inputs the Identity Token.

3. **Verification and Reward:**
   - dApp verifies the referral token via archive nodes.
   - A percentage of the referred user’s winnings is sent to the referrer’s wallet.

#### Challenges and Solutions

1. **Cheating Prevention:**
   - Use Identity Tokens that are immutable and linked to user wallets.
   - Smart contracts validate and lock the referral tokens to prevent alteration.

2. **Initial Token Acquisition:**
   - Users claim initial tokens from a faucet or through a minimal transaction with the central authority.
   - Alternatively, use Maxima to request and receive tokens directly.

3. **Tracking Referrals:**
   - Identity Tokens track referrals on the state variables.
   - Archive nodes can get referral trees for complex reward distribution from the coin ID of an Identity Token.

## Reward System

#### Objectives

- Provide incentives for users to participate in the dApp.
- Ensure fair and secure reward distribution.
- Enhance engagement in gaming and gambling dApps.
- Enhance engagement in activity and tasks dApps.

#### Key Features

- **Reward Tokens:** Distributed based on user activities or game or gambling rules.
- **Smart Contracts:** Handle reward issuance and conditions for claiming rewards.

#### Implementation

1. **Token Issuance:**
   - A predefined number of reward tokens are created.
   - Tokens are distributed through dApp interactions, such as gameplay, gambling wins, or specific actions.

2. **Reward Distribution:**
   - Smart contracts manage the reward conditions and distribution.
   - Users earn rewards based on predefined criteria (e.g., gameplay success, referrals, gambling outcomes).

3. **Claiming Rewards:**
   - Users claim rewards through smart contracts, which verify conditions and authorize token transfer.

#### Challenges and Solutions

1. **Secure Distribution:**
   - Smart contracts ensure rewards are distributed based on verified activities.
   - Use cryptographic techniques to prevent tampering.

2. **Generic System Adaptation:**
   - Third-party dApps purchase reward tokens and implement custom logic for distribution.
   - Tokens can carry advertising metadata to support monetization.

3. **Ad Integration:**
   - Reward tokens can embed advertising information.
   - Users receive additional rewards for interacting with advertisements.

### Detailed Implementation Steps

#### Referral System Implementation

1. **Scenario Setup:**
   - A user wants to play a gaming or gambling dApp.
   - The user invites friends using a referral token (Identity Token).

2. **Referral Token Distribution:**
   - Central authority or smart contract issues trillions of referral tokens.
   - Users obtain tokens via smart contract or directly from a central authority.

3. **User Invitation:**
   - The user generates an invite link with the Identity Token.
   - Friends use the link to join the dApp and input the referral token.

4. **Verification Process:**
   - The dApp verifies the referral token using archive nodes.
   - The token’s coin ID and associated wallet address are checked.

5. **Reward Distribution:**
   - A percentage of the new user’s earnings from gaming or gambling is sent to the referrer’s wallet.
   - Smart contracts manage and automate this process.

#### Identity Token Management

1. **Initial Token Acquisition:**
   - New users request Identity Tokens from a faucet or central authority.
   - Alternatively, users can claim tokens via Maxima, a secure messaging system.

2. **Smart Contract Validation:**
   - Identity Tokens are immutable and linked to user wallets.
   - Smart contracts lock tokens to prevent tampering.

3. **Referral Tracking:**
   - Archive nodes can get referral chains from an Identity Token.
   - Referral trees can be created for complex reward distributions.

#### Example Scenario

1. **Initial Setup:**
   - User A obtains an Identity Token.
   - User A invites User B using the referral link.

2. **Verification:**
   - User B joins the dApp and inputs the referral token.
   - The dApp verifies the token via an archive node.

3. **Reward Distribution:**
   - User B engages in gaming or gambling activities and earns rewards.
   - A percentage of User B’s earnings is sent to User A’s wallet (just an example use case).

### Interaction Between Referral and Reward Systems

1. **Combined Incentives:**
   - Referral bonuses are a percentage of rewards earned by referred users.
   - Both systems use Identity Tokens to track and validate user activities.

2. **Reward Claims:**
   - Referral rewards are issued alongside regular rewards, incentivizing continuous user engagement.
   - Smart contracts ensure fair and transparent reward distribution.

### Conclusion

The referral and reward systems are designed to work both independently and synergistically to foster user engagement and ensure fair reward distribution. The decentralized approach enhances security and transparency, while the interaction between the systems maximizes user benefits and system efficiency. By leveraging blockchain technology and smart contracts, these systems provide a robust framework for incentivizing user participation in decentralized applications, particularly within gaming, gambling, and user tasks/activities dApps.

---
---

# Based on the next draft ideas document:

**From discussion over discord sharing ideas between @NEO and @Tiger and @Josua , the ideas has been refined in this draft documents exploring the use cases and the problems on how to do it and from this document chatgpt generated the full document based on the next document:**


---- Referral system ------ 

 - We want a system with kind of referrals mechanism that let the user who attract more users to play a game or whatever be rewarded based on some conditions.
 - How we do it ?

- fully decentralized (More complex to develop)
- Partially decentralized
  - Approach 1:
    - Create all trillions of reward tokens over the same tokenid.
    - The user who plays a game want some refferral tokens to invite his friends.
    - A central authority sell referral tokens to any user.
    - The user who plays the game get rewarded and his referral also with a % of winned ammount.
      - Where are the rewards tokens come from? 
      	- Into an smart contract ? 
      	- How does the game get the rewards without cheating ?
      	- Under what conditions can the rewards be claimed or authorized?
      	
      - If we want a generic system for everyone use the rewards tokens
      	- It seems quite complex to fit on a generic system.
      	- Every third party (dapp/game) should buy the rewards tokens on a DEX, faucet, smart contract.
      	- Every third party then should build his own logic game and an smart contract to reward the users with the tokens bought.
      	  - How does beneficit the third party from giving for free the rewards tokens ?
      	    - Setting adversting info on the game or app ?
      	      - If the player click on the avertising then got more rewards ?
      	    - Setting the adversting info on the rewards tokens when you buy them ?
      	      - If the reward token has not an script embedded, you cannot control the info that is set on the reward token by others.
      	      - When you got the rewards tokens you can modify them .....every unit ? 
      	        - Implies do a lot of tx.
      	        - Or set the publicity when you send the rewards tokens to the user.
      	          - How to force the user to watch the publicity on the rewards tokens received ? (A kind of simpler MDAE project)
      	    
 
...just a few thoughts.

Referral Mechanism.

To be developed only using Minima, Maxima, arhive nodes, MMR nodes, smart contracts.
To be generic and usable for anyone can be very complex, so first start with a simple use case scenario:
  - Scenario 1:
    - A user want to play a dapp game.
    - The user want to invite his friends with a referral token (Identity token)
    - The dapp detects that you have an Identity token and send the invite link to your friends.
  - - A friend open the dapp and set your referral (coinid of the Identity token).
    - The dapp check, with the help of archive nodes, the coinid of Identity token(referral) and get the wallet address.
    - The dapp/game does his logic and a % of user winnings is sent to the referral wallet, or any other token that suits for reward the referrals.

  - **Questions, implications...:** 
    - In order to avoid cheating, as the referral system should be generic and adaptable to any dapp that wants to use it, we must need an Identity token that would act as a referral, this **Identity token** should have the user's wallet on it with an smart contract that not let you change nor move the token, so the coinid will be always the same and the dapps can check it against archive nodes to get the referral to be payed.
    
    - How to get an Identity Token ?
      - We already have created all the tokens.
      - We put some tokens on smart contract so people can get one Identity Token.
      - **Problem:**
        - The first time users install Minima and a dapp, they don't have any minima nor any token, so in order to claim for them on smart contract or doing any tx they need at least one token of something to be set as an input of a TX.
          - We could use the rewards tokens but we have the same problem, we need some coin/token to claim for them.
          - We could claim for it over Maxima to the central authority, asking for Identity token and your wallet, and the central authority will send to us.
            - The central authority minima server should be prepared to receive a lot of incomming petitions and transactions to do.
            - The central authority instead of posting the tx could send the tx to the other user to post it over maxima, but also the coin itself should be exported and send it over maxima so that, the user can import it and post the tx to be successful and got his Identity Token. 
              This can also could be a lot of work to do for the minima server.
            - We could use an external web server that would act as a faucet as @DM did, so the dapp will get the first rewards from there and with that, the dapp will be able to claim an Idenity token from the smart contract directly without the Central authority being involved.
        
        - The second time the user wants another Idenity token maybe for another game, he already can get it from the smart contract using his Idenity Token or the rewards or minimas he has.
        
        - **How the user keeps track of all his referrals ?**
          - Once the game / app pays to a referral this could include the identity token of the user on his state variables, so when the referral user receive the payment que has the info of the referral user and can save it to a DB.
          
          - **How we chain or create a tree of the referrals ?**
            - If your claim the first time for an  Identity Token using your referral then this is setup on the state variables, and if the new user want to refferral his friend, then the new user will have on his identity token the refferal of his friend who invited him.
            This allows for more complex referrals system of payments, as with a given Token Identity, using the archive nodes we can get all the tree of refferrals to the root (the original source) so the dapps or games can use it to stablish any level of payments or any logic they want.
            
..... more thoughts.
              
            
