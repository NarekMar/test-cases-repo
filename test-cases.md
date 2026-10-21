# Test Cases for login

## Assumptions
- Password must be at least 8 characters long.
- Email must contain "@".
- Passwords may contain special characters (!@#$%).

## TC-01: Login with valid data
Precondition: the user is registered (user@example.com / Test1234).
Steps:
1. Enter a valid email (for example, user@example.com).
2. Enter a valid password (for example, Test1234).
3. Click "Login".

Expected result: the user is logged in and sees their account page.

## TC-02: Login with wrong password
Precondition: the user is registered (user@example.com / Test1234).
Steps:
1. Enter a valid email (for example, user@example.com).
2. Enter a wrong password (for example, test1234).
3. Click "Login".

Expected result: the user is not logged in, an error message is shown.

## TC-03: Login with email without "@"
Precondition: the user is registered (user@example.com / Test1234).
Steps:
1. Enter an email without "@" (for example, test.mail.com).
2. Enter password "Test1234".
3. Click "Login".

Expected result: the user is not logged in, a message about invalid email is shown.

## TC-04: Login with password containing special characters
Precondition: the user is registered (user@example.com / Test!@34).
Steps:
1. Enter a valid email (for example, user@example.com).
2. Enter the password "Test!@34".
3. Click "Login".

Expected result: the user is logged in and sees their account page.

## TC-05: Login with empty fields 
Steps:
1. Leave the email and password fields empty. 
2. Click "Login".

Expected result: the user is not logged in, a message about empty fields

## TC-06: Login with a short password
Precondition: the user is registered (user@example.com / Test1234).
Steps:
1. Enter a valid email (for example, user@example.com).
2. Enter a short password (for example, Test12).
3. Click "Login"

Expected result: the user is not logged in, a message that password is less than 8 symbols
