# French Kaldi Profile

A [Rhasspy](https://github.com/rhasspy/rhasspy) profile for French (`fr`).

Includes:

* A [Kaldi nnet3](https://kaldi-asr.org/doc/dnn3.html) speech to text model
    * See files in `acoustic_model/`
    * Recipe created with [ipa2kaldi](https://github.com/rhasspy/ipa2kaldi)
    * Trained on:
        * [Common Voice](https://commonvoice.mozilla.org) (549 hours)
        * [M-AILabs](https://www.caito.de/2019/01/the-m-ailabs-speech-dataset/) (190 hours)
        * [Voxforge](http://voxforge.org/fr) (37 hours)
        * [SIWIS](https://datashare.is.ed.ac.uk/handle/10283/2353) (10 hours)
* An [IPA](https://en.wikipedia.org/wiki/International_Phonetic_Alphabet) pronunciation lexicon based on [Paul Guyot's lexicon](https://github.com/pguyot/zamia-speech/releases)
    * See `base_dictionary.txt.gz`
* A [phonetisaurus](https://github.com/AdolfVonKleist/Phonetisaurus) grapheme to phoneme model for predicting word pronunciations
    * See `g2p.fst.gz`
    * Trained on `base_dictionary.txt.gz`
* A tri-gram [ARPA language model](https://cmusphinx.github.io/wiki/arpaformat/)
    * See `base_language_model.txt.gz`
    * Text from audio transcriptions, [Common Voice](https://github.com/mozilla/common-voice/tree/master/server/data/fr), and [Universal Dependencies](https://universaldependencies.org/)
