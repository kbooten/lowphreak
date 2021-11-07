# Low Phreak

A creativity-support tool for poetry.

Low Phreak (**Low Freq**uency [**Pho**naskos](https://books.google.com/books?id=4QUIAQAAIAAJ&pg=PA193&lpg=PA193&dq=phonaskos&source=bl&ots=pQyyuyEqZz&sig=ACfU3U2ai2pLw0H0lhCoe1MrljKFd6s_3Q&hl=en&sa=X&ved=2ahUKEwjDj7-hi4L0AhWSdd8KHYQBDVQQ6AF6BAgSEAM#v=onepage&q=phonaskos&f=false)) discourages the poet from using common, high-frequency words.  It recommends alternatives---semantically-related low-frequency words.

---

The basis of Low Phreak is a word2vec model trained on pos-tagged sentences (e.g. `["the_DT", "dog_NN",...]`) extracted from Project Gutenberg text and Amazon product reviews.

Low Freak lives in this [Google Colab notebook](https://colab.research.google.com/drive/1rduI02KSUxuMMQmcN8pVrkFdXq_XFhQw?usp=sharing). The notebook uses `wget` to get raw data files from this repo, so anyone can try out Low Phreak in the browser simply by copying and running the Colab notebook (*File > Save copy in Drive* then *Runtime > Run all*). 

See also:

1. [`prepping_data_for_training.ipynb`](https://github.com/kbooten/lowphreak/blob/main/prepping_data_for_training.ipynb): tokenizing and pos-tagging sentences, counting tokens to identify low-frequency ones.
2. [`trainword2vecmodel.ipynb` (Google Colab)](https://colab.research.google.com/drive/1itCPb52Gnm6v_LpLWQi_R958WDZDu1Qd?usp=sharing): training the word2vec model on sentences from the previous notebook.
