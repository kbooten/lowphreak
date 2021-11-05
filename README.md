# Low Phreak

A creativity-support tool for poetry.

Low Phreak (**Low Freq**uency [**Pho**naskos](https://books.google.com/books?id=4QUIAQAAIAAJ&pg=PA193&lpg=PA193&dq=phonaskos&source=bl&ots=pQyyuyEqZz&sig=ACfU3U2ai2pLw0H0lhCoe1MrljKFd6s_3Q&hl=en&sa=X&ved=2ahUKEwjDj7-hi4L0AhWSdd8KHYQBDVQQ6AF6BAgSEAM#v=onepage&q=phonaskos&f=false)) discourages the poet from using common, high-frequency words.  It recommends alternatives---semantically-related low-frequency words.

---

The basis of Low Phreak is a word2vec model trained on pos-tagged sentences (e.g. `["the_cc", "dog_nn",...]`) extracted from Project Gutenberg text and Amazon rproduct reviews.  This repo consists of three notebooks:

1. Tokenizing and pos-tagging sentences.
2. Training the word2vec model.
3. The interface itself

