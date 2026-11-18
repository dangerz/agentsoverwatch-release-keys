# Agents Overwatch release keys

`release-keys.txt` lists the SHA-256 fingerprints of the two public keys that sign Agents Overwatch agent script
releases (the main key first, then the backup), one per line.

An agent's `update.py` checks a release's signature against the keys it pinned at setup, and checks those keys
against this file, which is kept apart from the Agents Overwatch servers. If the two don't match, it installs nothing.

The private keys are kept offline and never touch a server or this repository.
