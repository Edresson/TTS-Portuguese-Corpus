# TTS-Portuguese Corpus
To create the dadaset was used public domain texts.Initially, the texts were extracted from Wikipedia articles displayed in the Highlights section. In a second phase, texts were also extracted from  [Chatterbot-corpus](https://github.com/gunthercox/chatterbot-corpus/tree/master/chatterbot\_corpus/data/portuguese), a corpus originally created for the construction of chatbots. We also used 20 sets of phonetically balanced phrases, each set containing 10 phrases proposed by [Seara (1994)](https://repositorio.ufsc.br/bitstream/handle/123456789/112119/98594.pdf?sequence=1). The total number of words is 71,358, with 13,311 distinct words.

The dataset developed in this work has approximately 10 hours and 28 minutes of speech from a single speaker, recorded at 48Khz, containing a total of 3,632 audio files in Wave format. Audio files range from 0.67 to 50.08 seconds.

Since the audios were not recorded in an acoustic studio, there is noise present in the audio files, so we chose to use a noise suppression library. For this purpose we used the library [RNNoise](https://github.com/xiph/rnnoise) . It is based on Recurrent Neural Networks, more specifically Gated Recurrent Unit (GRU)  and demonstrated good performance for noise suppression. The dataset is open source, and public available under the terms of the license Creative Commons Attribution 4.0 (CC BY 4.0).

Download this Dataset: 

[TTS-Portuguese Corpus 48Khz (as recorded)](https://huggingface.co/datasets/Edresson/TTS-Portuguese-Corpus/resolve/main/TTS-Portuguese-Corpus.zip)

[TTS-Portuguese Corpus 48Khz (as recorded) Dropbox](https://www.dropbox.com/s/ohpc7epowv9ct7o/TTS-Portuguese-Corpus.zip?dl=0)

Using [Wget](https://www.gnu.org/software/wget/): ```wget  https://huggingface.co/datasets/Edresson/TTS-Portuguese-Corpus/resolve/main/TTS-Portuguese-Corpus.zip```

**Audio samples** synthesized with best models: https://edresson.github.io/TTS-Portuguese-Corpus/

Models trained in this corpus:

| Model       |Colab Demo URL |
| ------------- |:------:|
| DCTTS model (Experiment 1) | https://drive.google.com/file/d/1tlmk4DCtYgvUUcJgOPHXPw9o2ysnbVbg/view  |
|TTS Mozilla model (Tacotron) |https://colab.research.google.com/drive/1b5Yo0sghajCrjftolN0LbArZzar7fd01?usp=sharing |

Synthesized samples of the best model with Griffin–Lim (1.wav) and WaveRNN (1-wavernn.wav) vocoder : [Link](https://soundcloud.com/user-797601460/sets/tts-mozilla-trained-in-tts-portuguese-corpus-with-wavernn-and-griffinlim-vocoders)



## NEW

| Model       |Colab Demo URL |
| ------------- |:------:|
|GlowTTS model + HiFi-GAN-FT |https://colab.research.google.com/drive/1sh96-f9J2BJcLm1rz5KBkwq3YP83bEr5?usp=sharing  |


**Cite this Dataset:**

Preprint:

```
@misc{casanova2020ttsportuguese,
    title={TTS-Portuguese Corpus: a corpus for speech synthesis in Brazilian Portuguese},
    author={Edresson Casanova and Arnaldo Candido Junior and Christopher Shulby and Frederico Santos de Oliveira and João Paulo Teixeira and Moacir Antonelli Ponti and Sandra Maria Aluisio},
    year={2020},
    eprint={2005.05144},
    archivePrefix={arXiv},
    primaryClass={eess.AS}
}

```

Full Paper:
```
@article{casanova2022tts,
  title={TTS-Portuguese Corpus: a corpus for speech synthesis in Brazilian Portuguese},
  author={Casanova, Edresson and Junior, Arnaldo Candido and Shulby, Christopher and Oliveira, Frederico Santos de and Teixeira, Jo{\~a}o Paulo and Ponti, Moacir Antonelli and Alu{\'\i}sio, Sandra},
  journal={Language Resources and Evaluation},
  pages={1--13},
  year={2022},
  publisher={Springer}
}


```
