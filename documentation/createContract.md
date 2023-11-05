# Use Case Description

## Create Contract

## 1. Actors

- **Solana User**: Has the ability to create a new account based on his Solana wallet address.

## 1.2. Preconditions

- The user should have a valid Solana wallet address.
- The user needs to provide a valid phone number.
- The user needs to provide his real full name.
- The user needs to provide his email.
- The user needs to provide his birth date.

## 1.3. Main Flow

1. The user navigates to the home page.
2. The user clicks the login button.
3. If the Solana wallet address that the user clicks the login button with already has an account, it takes the user to his profile.
4. If it doesn't have an account yet, it takes the user to a create account page.
5. The user enters his personal data such as:
   - Phone number
   - Full name
   - Birth date
   - Email
6. The user clicks the create account button.
7. If all the data provided by the user is valid, a new account is created.
8. The account created will have the status "unverified."
9. The system will send an email to the user with a verification code.
10. The account with "unverified" status will not be able to create or sign contracts.
11. The system takes the user to his new profile page.
12. The system will show a box for the user to enter his verification code.
13. The system will show a "create new contract" button ONLY after the user is verified.

## 1.4. Alternate Flows

- **Invalid personal data**: If the user doesn't provide a valid email, phone number, or name, the system will not allow the user to create an account.
- **Invalid user age**: If the user's age is below 18, it will not allow him to create an account.
- **User entered a wrong email**: If the user loses access to his email before being able to verify his account, there will be a "change email" link, which will prompt a modal to the user to let him change the email provided and resend the verification code. Once the email is changed and the new verification code is sent, the old verification code previously sent will become inactive/useless.
- **User never verifies account**: If the user does not verify his account within 7 days of its creation, the system will automatically delete the account.

## 1.5. Postconditions

The user will have a valid account ready to create/sign contracts.

## 2. Acceptance Criteria

- The user must provide valid personal information.
- The user must verify the account via a verification code sent by email.
- The user must be 18+ years old.
- The user must have a valid Solana Wallet Address.

## 3. Appendices

- [Include any supplementary information, diagrams, or additional details that support this use case.]
