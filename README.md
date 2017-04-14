### DICEWARE

Diceware is a method for generating long, secure passphrases that are difficult to guess, but easier to remember.

This project defaults to the [Electronic Frontier Foundation (EFF) wordlist](https://www.eff.org/deeplinks/2016/07/new-wordlists-random-passphrases).

For questions about the Diceware method, please visit the [official Diceware page](http://diceware.com) and [Diceware FAQ](http://world.std.com/%7Ereinhold/dicewarefaq.html).

This project was inspired and forked from [Stephen Washington's Diceware project](https://github.com/stephenwashington/diceware).

### PRNG Disclaimer

This implementation of Diceware passphrase generation has an auto-generate option that uses a [Cryptographically Secure PRNG](https://en.wikipedia.org/wiki/Cryptographically_secure_pseudorandom_number_generator) (CSPRNG) to simulate dice rolls. These types of pesudo-random number generators are better than most because, even if an attacker has access to a series of previous rolls, he cannot reliably predict the next roll. Despite this improvement, CSPRNGs are not truly random. The Offical Diceware page strongly recommends you use physical dice when generating passphrases.

### Dependencies

The webpage uses HTML, CSS, and built-in Javascript functions (no jQuery, etc.). In addition, it uses [random.js](https://github.com/ckknight/random-js) to generate random numbers. All dependencies are locally loaded, so no calls to any other servers are made.
