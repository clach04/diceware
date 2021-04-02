#!/usr/bin/env python
# Diceware password generator in Python
# (words file is https://www.eff.org/files/2016/07/18/eff_large_wordlist.txt)
# Because I have no dice:

try:
    from secrets import choice
except ImportError:
    import random
    choice = random.SystemRandom().choice
import string
import sys


def stupid_extra_stuff():
    """return a random upper case letter, digit and "special character" which some password policies now require
    returns them in order (not yet randomized, may never be....)
    """
    special_characters = []
    special_characters.append(choice(string.ascii_uppercase))
    special_characters.append(choice(string.digits))
    special_characters.append(choice(string.punctuation))
    return ''.join(special_characters)


try:
    num_words = int(sys.argv[1])
except (IndexError, ValueError):
    num_words = 5
w = [s.split()[1] for s in open(sys.path[0]+'/words')]
passphrase = '-'.join(choice(w) for i in range(num_words))
print(passphrase)
print(passphrase+stupid_extra_stuff())
