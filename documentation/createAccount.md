# Use Case Description

## Create Account

## 1. Actors

- **Verified User**: Has the ability to create a new contract.

## 1.2. Preconditions

- The user should have a valid Solana wallet address.
- The user must have a verified account.
- The user must have $USDC or $SOL to put in the contract as collateral (payment).
- The receiver must have a valid Solana wallet address.

## 1.3. Main Flow

1. The user clicks the "create new contract" button.
2. The system prompts the user with a modal to enter the following data:
   - Contract title
   - Contract description (requirements for the contract to be fulfilled)
   - Receiver Solana wallet address
   - Currency of payment (SOL or USDC)
   - Amount of payment
   - Expiration date
3. If the data provided by the issuer is valid, the user clicks "create contract."
4. A sign popup appears in the user's wallet asking to sign the transaction and send the amount of payment in the selected currency.
5. The system creates the contract PDA that stores all the data and assets of the contract.
6. The system mints two cNFTs and sends one to the issuer and the other to the receiver with all the data related to the contract.
7. The contract creation modal closes.

## 1.4. Alternate Flows

- **The issuer doesn’t have funds to add to the contract**: The issuer can't create the contract.
- **The issuer adds invalid data to the contract creation**: The issuer can't create the contract.

## 1.5. Postconditions

- A contract is created with all the proper data.
- Two cNFTs with the contract details are minted and sent to the issuer and receiver, respectively.

## 2. Acceptance Criteria

- A contract with all the proper data is created.
- Two cNFTs with the contract data are created and sent to the issuer and receiver, respectively.

## 3. Appendices

- [Include any supplementary information, diagrams, or additional details that support this use case.]
