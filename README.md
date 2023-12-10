# Event Token Smart Contract 

## Overview

The Event Token smart contract, named Event_Token, serves as the backbone for managing tokens on an event platform. Developed in Solidity, it leverages the OpenZeppelin library for ERC20 implementation and introduces features such as token minting, burning, ticket redemption for different chambers, and token transfers.

## Key Features

1. **Token Minting**
   - The contract owner can create new Event Tokens and allocate them to specific addresses, providing flexibility in token distribution.

2. **Token Burning**
   - Users have the ability to burn a portion of their own tokens, reducing their token balance.

3. **Ticket Redemption**
   - Users can exchange Event Tokens for event tickets, each associated with a specific chamber: SILVER, GOLD, or DIAMOND. Each chamber has a unique cost in terms of tokens.

4. **Token Transfer**
   - Users can transfer their Event Tokens to other addresses, facilitating peer-to-peer transactions.

5. **Chamber Enumeration**
   - The contract defines an enumeration type, "Chamber," which represents the different tiers of event participation: SILVER, GOLD, and DIAMOND.

6. **Event Ticket Redeemed Event**
   - An event is emitted when a user successfully redeems a ticket, providing essential information such as the user's address, the chosen chamber, and the associated ticket cost.

7. **Get Ticket Cost Function**
   - Users can query the cost of a ticket for a specific chamber without executing any transactions.

## Usage Guidelines

1. **Deploying the Contract**
   - Deploy the Event_Token contract on the Ethereum blockchain, specifying the initial owner's address.

2. **Minting Tokens**
   - The contract owner can generate new Event Tokens and assign them to specific addresses, managing the token supply.

3. **Burning Tokens**
   - Users can reduce their token balance by burning a certain amount of their own tokens.

4. **Redeeming Tickets**
   - Users can participate in different event chambers by redeeming tickets using their Event Tokens. The cost varies based on the selected chamber.

5. **Transferring Tokens**
   - Token holders can transfer their Event Tokens to other addresses, enabling seamless transactions.

6. **Accessing Ticket Cost**
   - Users can retrieve the cost of a ticket for a specific chamber without executing any transactions, providing transparency.

## Security Considerations

1. **Ownership**
   - Be mindful of the centralized control held by the contract owner. Ensure secure key management practices to mitigate potential security risks.

2. **Ticket Redemption**
   - Implement robust validation in the ticket redemption function to prevent unintended behavior or exploitation.

3. **Token Transfer**
   - Enforce access controls and thorough validation to prevent unauthorized token transfers and maintain the security of the token ecosystem.

## License

This smart contract operates under the MIT License, with details available in the SPDX-License-Identifier within the source code.

## Author

Vignesh

s82167500@gmail.com
