# randomwordz

This package is used to get simple random words based on a particular part of speech. 

The data comes from the Brown Corpus, which was cleaned using a blacklist of words. In addition, 
names were added from the UNIX list of names.

### Installation:

```
$ python3 -m pip install randomwordz
```

### Usage:

```py
from randomwordz import WordGenerator

wg = WordGenerator()

print(wg.get_random("noun"))
# output: apple, etc
```

### Docs:

```py
wg.get_random(CODE)
# returns: "apple"
```
gets a random word of the class `CODE`

```py
wg.get_all(CODE)
# returns: ["apple", "orange", "human", ...]
```
gets a list of all the words of the class `CODE`

```py
wg.get_all_random(CODE)
# returns: ["human", "pear", "apple", ...]
```
gets a randomized list of all the words of the class `CODE`

#### Options:

```
'ADJ', 'ADP', 'CONJ', 'DET', 'NOUN', 'NUM', 'PRON', 'PRT', 'VERB', 'NAME'
```



