# Password-Generator
**Purpose of the Code:**

The purpose of this Python code is to generate a random password based on the user's desired length. It uses a set of characters that include uppercase and lowercase letters, digits, and special characters. The code shuffles these characters and selects a random set of characters to create a password of the specified length.

**How the Code Works:**

1. The code begins by importing the `string` and `random` modules. `string` is used to access predefined character sets like lowercase letters, uppercase letters, and digits, while `random` is used for shuffling and selecting characters randomly.

2. A list called `char` is created, which contains all the characters that can be used to generate the password. It includes lowercase and uppercase letters, digits, and some special characters like "!@#$%^&*()_".

3. The `gen_random_pass` function is defined to generate the random password. It takes the desired length of the password as input from the user.

4. The `random.shuffle(char)` line shuffles the characters in the `char` list. This step ensures that the characters used in the password are selected randomly.

5. An empty list called `password` is created to store the randomly selected characters.

6. Using a loop that runs for the specified length of the password, characters are randomly selected from the shuffled `char` list using `random.choice(char)`. These characters are appended to the `password` list.

7. After the loop is complete, the `password` list contains the randomly selected characters for the password.

8. `random.shuffle(password)` shuffles the characters within the `password` list to ensure that the characters are in a random order.

9. Finally, the characters in the `password` list are joined together into a single string using `"".join(password)`, and the generated password is printed to the console.

10. The `gen_random_pass()` function is invoked to execute the password generation process.

The result is a random password of the specified length, containing a mix of uppercase and lowercase letters, digits, and special characters, with the order of characters also being randomized.
