# dirty-password-generator
# this is a python script that generates an input number of passwords using random on the inputed characters.

import random

print('Welcome to the Dirty Password Generator')

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ1234567890!@#$%^&*()'

number = input('Amount of passwords to generate: ')
number = int(number)

length = input('Input your password lenth: ')
length = int(length)

print('\nhere are your passwords:')

for pwd in range(number):
    passwords = ''
    for c in range(length):
        passwords += random.choice(chars)
    print(passwords)
