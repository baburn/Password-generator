# Password Generator

## Overview

This Python script is a simple password generator that generates random passwords based on user-specified lengths. The generated passwords include a mix of lowercase letters, uppercase letters, and numbers.

## Usage

### Prerequisites

Ensure that you have Python installed on your system.

### Running the Script

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/password-generator.git
   ```

2. Navigate to the project directory:

   ```bash
   cd password-generator
   ```

3. Run the script:

   ```bash
   python password_generator.py
   ```

4. Follow the prompts to specify the number of passwords and their respective lengths.

## Code Explanation

The script consists of several functions:

### `generatePassword(pwlength)`

- Input: `pwlength` - a list of integers representing the desired lengths of passwords to be generated.
- Output: A list of randomly generated passwords.

This function generates passwords by randomly selecting lowercase letters and then replacing some characters with numbers and uppercase letters using the helper functions `replaceWithNumber` and `replaceWithUppercaseLetter`.

### `replaceWithNumber(pword)`

- Input: `pword` - a string representing a password.
- Output: The password with some randomly chosen characters replaced by numbers.

This function randomly replaces a character in the first half of the password with a numeric digit.

### `replaceWithUppercaseLetter(pword)`

- Input: `pword` - a string representing a password.
- Output: The password with some randomly chosen characters replaced by uppercase letters.

This function randomly replaces a character in the second half of the password with its uppercase equivalent.

### `main()`

This is the main function responsible for interacting with the user. It prompts the user for the number of passwords to generate and their respective lengths. It then calls `generatePassword` to generate and display the passwords.

## Example

```bash
How many passwords do you want to generate? 2
Generating 2 passwords
Minimum length of password should be 3
Enter the length of Password #1: 8
Enter the length of Password #2: 6
Password #1 = ab1CdeFg
Password #2 = abc2De
```

## Note

- The minimum length of a password is set to 3.
- The script ensures that the user-specified length is at least 3 for each password.

Feel free to customize and enhance the script according to your specific requirements.
