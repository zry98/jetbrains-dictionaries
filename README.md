# JetBrains Dictionaries
Dictionaries of other languages for JetBrains IDEs

## Generate dictionaries of other languages

For example, on Ubuntu:
```bash
$ sudo apt search aspell-* | grep -B 1 Spanish  # search for a Spanish dictionary
...
aspell-es/bionic 1.11-14 all
  Spanish dictionary for aspell
$ sudo apt install aspell-es  # install it
...
$ aspell --lang es dump master | aspell --lang es expand | tr ' ' '\n' > es.dic  # convert it for JetBrains IDEs
...
```