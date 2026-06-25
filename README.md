# slashmark-password-project
# Password Generator

import random
import string

print("=== PASSWORD GENERATOR ===")

# Ask user for password length
length = int(input("Enter password length: "))

# Characters to use in password
characters = string.ascii_letters + string.digits + string.punctuation

password = ""

# Generate password
for i in range(length):
    password += random.choice(characters)

print("Generated Password:", password)
