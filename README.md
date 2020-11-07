# games-magazine-cryptogram-helper

Kappa Publishing's _Games Magazine_/_Games World of Puzzles_ often includes a cryptogram or cryptolist puzzle, where you're provided with some ciphertext and expected to work out the plaintext.  There are generally some hints (e.g., the cryptolists have some shared feature, except for one where you have to crack the code _and_ figure out the shared topic).

As of this writing, there are two scripts:

- `freqs`, which does a basic frequency analysis of a ciphertext and spits out a YAML guesses file.
- `dosubst`, which allows you to do substitution based on the guesses file.

Both take a single argument, the name of a file containing the ciphertext (which should be all caps, plus any punctuation included in the original).  `freqs` creates a YAML file, `_ciphertextfile_.guesses.yaml`, which you can also edit to change substitutions.  `dosubst` uses the ciphertext and the matching guesses file to do the substitutions.
