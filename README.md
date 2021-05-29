# nltk

import nltk
nltk.download()

story = """Package that provides Jupyter kernels for use with the consoles of Spyder, the Scientific Python Development Environment.

These kernels can launched either through Spyder itself or in an independent Python session, and allow for interactive or file-based execution of Python code inside Spyder.

To learn about creating, connecting to and using these kernels with the Spyder console, please read our"""
# finding all the sentences
sentences = nltk.sent_tokenize(story)
# find all the words
words = nltk.word_tokenize(story)

# stemming find coommon characters in words (includes words not in dictionary)
# [history, historical] = histor
# library "porterstemmer"

from nltk.corpus import stopwords # mostly noun, pron, prepositions etc
from nltk.stem import PorterStemmer

stopwords.words('english')

# convert paragraph or sentences or words into stemming
# for i in range(len(sentences)):
    
# lemmitization find coommon characters in words (does not includes words not in dictionary)
# [history, historical] = history
# library "porterstemmer"

# uni gram - 1 word per dimension ['my', 'name', 'is', 'sam']
# bi gram - 2 words per dimension ['my name', 'name is', 'is sam', 'sam']
# tri gram - 3 words per dimension
# n gram - n words per dimension
