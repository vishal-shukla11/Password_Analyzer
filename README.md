Functions

has_upper:

Checks if the password contains at least one uppercase letter.
Iterates through each character of the password.
Returns 1 if an uppercase letter is found, otherwise returns 0.

has_lower:

Checks if the password contains at least one lowercase letter.
Iterates through each character of the password.
Returns 1 if a lowercase letter is found, otherwise returns 0.

has_digit:

Checks if the password contains at least one digit.
Iterates through each character of the password.
Returns 1 if a digit is found, otherwise returns 0.

has_special:

Checks if the password contains at least one special character (non-alphanumeric, excluding space and underscore).
Iterates through each character of the password.
Returns 1 if a special character is found, otherwise returns 0.

Main Logic

evaluate_password:

Determines the strength of the password based on its length and the presence of different types of characters.
Strong Password:
Length is at least 8 characters.
Contains at least one uppercase letter, one lowercase letter, one digit, and one special character.
Moderate Password:
Length is at least 6 characters.
Contains at least one uppercase letter, one lowercase letter, and one digit.
Weak Password:
Does not meet the criteria for strong or moderate passwords.

main:

Prompts the user to enter a password.
Reads the input using fgets to avoid buffer overflow and handle spaces.
Removes the newline character added by fgets.
Calls evaluate_password to determine and print the strength of the entered password.
