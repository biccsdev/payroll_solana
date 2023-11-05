# Use Case Description

## Sign Contract

## 1. Actors

- **Solana User**: Has a valid Solana wallet address.

## 1.2. Preconditions

- The user should have a valid Solana wallet address.
- The receiver (user) should have a cNFT of the contract that wants to sign.
- The contract's start date shouldn't occur yet.

## 1.3. Main Flow

1. The receiver heads to his profile.
2. The receiver clicks on the specific contract's "sign contract" button.
3. A new transaction pops up in the receiver's wallet.
4. The receiver signs the new transaction.
5. The system updates the receiver and issuer cNFTs with the receiver's signature and the new status "valid."
6. The contract becomes valid.
7. The system updates the UI with the valid contract data.

## 1.4. Alternate Flows

- **The receiver does not accept the contract details**:
  - The receiver goes to his profile and sees the contract.
  - The receiver clicks the "I don't agree with details" button.
  - The status of the cNFT updates from "pending" to "disagree."
  - A new message appears in the issuer's profile.
  - The issuer has to update the contract details.
  - The process starts over.

## 1.5. Postconditions

- The contract in question becomes valid.
- The issuer and receiver cNFTs are updated with the necessary data.

## 2. Acceptance Criteria

- The cNFTs must have a "valid" status.
- The cNFTs must have all involved wallets' signatures.
- The contract must hold the collateral assets of the agreement.

## 3. Appendices

- [Include any supplementary information, diagrams, or additional details that support this use case.]
