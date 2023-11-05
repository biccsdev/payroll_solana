# Use Case Description

## Edit Contract

## 1. Actors

- **Verified User**: Has the ability to create a new contract.

## 1.2. Preconditions

- The user should have a valid Solana wallet address.
- The contract must have the status "pending."
- The receiver must not have signed the contract yet.

## 1.3. Main Flow

1. The issuer navigates to his profile.
2. The issuer clicks the contract that wants to edit.
3. Clicks the "edit" button.
4. A modal with the contract info pops up.
5. The issuer modifies the desired data.
6. Clicks the "save changes" button.
7. Both cNFTs' data gets updated with the new contract data.

## 1.4. Alternate Flows

- **The issuer deletes the contract**:

  - The issuer clicks the "delete contract" button.
  - The cNFTs become invalid and change their status to "deleted contract" in the description and "invalid" in the status.

- **The issuer changes the receiver**:
  - The issuer changes the Solana wallet address of the receiver.
  - The current cNFT in the previous Solana wallet address becomes invalid. It updates its description to "redacted" and status to "invalid."
  - A new cNFT is minted with all the contract data and is sent to the new receiver's Solana wallet address.

## 1.5. Postconditions

- The cNFTs must get updated with the new contract data.
- The contract PDA must get updated with the new data.

## 2. Acceptance Criteria

- The cNFTs must get updated with the new contract data.
- The contract PDA must get updated with the new data.

## 3. Appendices

- [Include any supplementary information, diagrams, or additional details that support this use case.]
