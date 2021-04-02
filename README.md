# Diceware password generator

Diceware password generator in Python. Because I have no dice. Uses [EFF's Long Wordlist][wordlist].

Consider https://github.com/ulif/diceware/ instead, it has more features.
This script has less features but is really tiny so faster to code review.

```bash
git clone https://github.com/clach04/diceware.git
cd diceware
./passphrase
```

For example:

```
$ ./passphrase
panoramic-nectar-precut-smith-banana

$ py -3 passphrase 7
evacuate-skinhead-superman-uselessly-affecting-moneyless-scurvy
evacuate-skinhead-superman-uselessly-affecting-moneyless-scurvyN1+
```

### Links

* [Diceware passphrase home page](http://www.diceware.com)
* [EFF Dice-Generated Passphrases](https://www.eff.org/dice) ([deep dive](https://www.eff.org/deeplinks/2016/07/new-wordlists-random-passphrases), [word list][wordlist])

[wordlist]: https://www.eff.org/files/2016/07/18/eff_large_wordlist.txt
