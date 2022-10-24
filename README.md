# CYB333-
Complex Password Checker
import re

import string

password = input("Enter a password\n\nThe password must have at least 8 characters including upper case, lower case, and a number.\n")

if all([
    len(password) >= 8,
    any(character in password for character in string.ascii_lowercase),
    any(character in password for character in string.ascii_uppercase),
    any(character in password for character in string.digits),
]):
    print("Password is strong enough")
else:
    print("Password is not strong enough")
