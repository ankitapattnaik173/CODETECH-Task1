###Name:ANKITA PATTNAIK
Company:CODETECH IT SOLUTIONS
ID:CT8CSEH1196
Domain:"CYBER SECURITY&ETHICAL HACKING"
Duration:JUNE 20th to AUGUST 20th,2024.
Mentor:###

## Overview of the Project

### Project: Password Strength Checker

This repository contains a Python script for checking the strength of a password. The script evaluates the password based on various criteria and provides feedback on its strength. It also checks if the password is among common passwords, which can make it more vulnerable to attacks.

## Features

- **Character Class Check**: Ensures the password contains at least one uppercase letter, one lowercase letter, one digit, and one special character.
- **Length Check**: Evaluates the password based on its length, giving higher scores to longer passwords.
- **Common Password Check**: Compares the password against a list of common passwords to ensure it is not easily guessable.

## Usage

### Prerequisites

- Python 3.x

### Setup

1. Clone the repository or download the script files.
2. Ensure you have a file named `common.txt` in the same directory as the script. This file should contain a list of common passwords, one per line.

### Running the Script

1. Open a terminal or command prompt.
2. Navigate to the directory containing the script and the `common.txt` file.
3. Run the script using the following command:
   ```terminal
   python password_strength_checker.py
   ```

### Example

When you run the script, you will be prompted to enter a password. The script will then evaluate the password and print a message indicating its strength.

```plaintext
Enter password: P@ssw0rd123
Password is not that strong.
```

### Detailed Feedback

- If the password is too common, the script will immediately indicate that the password strength is 0.
- The script will evaluate the password based on character classes and length, and provide feedback accordingly.
- If the password does not meet the minimum requirements (at least one uppercase letter, one lowercase letter, one digit, and one special character), the script will suggest improvements.

## Code Overview

### `check_password_strength(password: str) -> int`

This function takes a password as input and returns a score indicating its strength. The score is based on the presence of different character classes and the length of the password.

### `check_password(password: str) -> None`

This function checks the password against a list of common passwords and then evaluates its strength using the `check_password_strength` function. It prints messages indicating the strength of the password and suggests improvements if necessary.

## Example `common.txt` File

The `common.txt` file should contain a list of common passwords. Here is an example of what the file might look like:

```plaintext
123456
password
123456789
12345678
12345
1234567
password1
```

Make sure the `common.txt` file is placed in the same directory as the script.

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, feel free to open an issue or submit a pull request.

