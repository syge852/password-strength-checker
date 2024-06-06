# password_strength_checker.py

import re

def check_password_strength(password):
    if len(password) < 8:
        return "Weak: Password must be at least 8 characters long"
    if not re.search(r"[A-Z]", password):
        return "Weak: Password must contain at least one uppercase letter"
    if not re.search(r"[a-z]", password):
        return "Weak: Password must contain at least one lowercase letter"
    if not re.search(r"\d", password):
        return "Weak: Password must contain at least one digit"
    if not re.search(r"[!@#$%^&*(),.?\":{}|<>]", password):
        return "Weak: Password must contain at least one special character"
    return "Strong password"

def main():
    password = input("Enter a password to check its strength: ")
    strength = check_password_strength(password)
    print(strength)

if __name__ == "__main__":
    main()
