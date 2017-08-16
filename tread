# tokenize with double newline  but not single newline

import re
from nltk.tokenize import sent_tokenize
# file = 'foo.txt'

def tread(s):
    tread = open(s, 'r').read()
    while '  ' in tread: # reduce whitespace
        tread = tread.replace('  ', ' ')
    tread = re.split('\\\n\\\n|\\\n\\ \\\n',tread) # treats string between double newline \n\n as a standalone sentence
    lst=[]
    for each in tread:
        lst.extend(tokenizer.tokenize(each))
    tread = map( lambda x: " ".join(x.replace('\n', " ").split()),lst) # new line is not treated as a new sentence
    return tread
