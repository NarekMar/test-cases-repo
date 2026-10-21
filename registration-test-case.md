# Test Cases for registration

## Assumptions
- Password must be 8 to 20 characters long.

## TC-R01: Registration with password of 7 characters (below minimum)
Precondition: the registration page is open, email user2@example.com is not registered.
Steps:
1. Enter "user2@example.com" in the email field.
2. Enter "Test123" (7 characters) in the password field.
3. Click "Register".

Expected result: the account is not created, a message says the password must be at least 8 characters.

## TC-R02: Registration with password of 8 characters (minimum)
Precondition: the registration page is open, email user3@example.com is not registered.
Steps:
1. Enter "user3@example.com" in the email field.
2. Enter "Test1234" (8 characters) in the password field.
3. Click "Register".

Expected result: the account is created, the user sees a confirmation message or their account page.

## TC-R03: Registration with password of 20 characters (maximum)
Precondition: the registration page is open, email user4@example.com is not registered.
Steps:
1. Enter "user4@example.com" in the email field.
2. Enter "Test1234Test1234Test" (20 characters) in the password field.
3. Click "Register".

Expected result: the account is created, the user sees a confirmation message or their account page.

## TC-R04: Registration with password of 21 characters (above maximum)
Precondition: the registration page is open, email user5@example.com is not registered.
Steps:
1. Enter "user5@example.com" in the email field.
2. Enter "Test1234Test1234Test1" (21 characters) in the password field.
3. Click "Register".

Expected result: the account is not created, a message says the password must be maximum 20 characters. 