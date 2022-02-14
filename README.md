# Overview: Singing Voice Transcription

**Jiarui Hai**

## Singing Melody Transcription

### Frame-level

- [Multiple F0 estimation in vocal ensembles using convolutional neural networks](https://arxiv.org/pdf/2009.04172.pdf)
  - ISMIR 2020
  - multiple f0 extraction: addressed the f0 estimation challenge for harmony
- [Joint singing pitch estimation and voice separation based on a neural harmonic structure renderer](https://ieeexplore.ieee.org/abstract/document/8937135/?casa_token=nRG-pPmxE4QAAAAA:JwFl-dNmyYUl8nCE3US3hOuE0VNgc5OOu5ob768JKjTxvtOnh2UN-yT_XM8QCj3gKQbWIZF-TeM)
  - WASPAA 2019
  - multi-task model: vocal accompaniment separation + f0 estimation
- [CNN based two-stage multi-resolution end-to-end model for singing melody extraction](https://ieeexplore.ieee.org/abstract/document/8683630/?casa_token=TLZDOLK22tEAAAAA:dpd-UXLx5YY7xVMqtIm8Xt7WuPZHI-kAoI1ncwAIiUWHxW_FWmqVakGjaGjWyEcDvC6ZERilt3Y)
  - ICASSP 2019
  - neural spectrogram encoder + feature extractors → pitch
- [Vocal melody extraction using patch-based CNN](https://ieeexplore.ieee.org/abstract/document/8462420/?casa_token=3qXFXh0arZEAAAAA:kagkmBVktjywvn3F2oIPlL_V8UoMjhfTpNJ-AzWFKKRX-dI0isi6Z6zHzCLYCa61pkP9tGuypFY)
  - ICASSP 2018
  - end-to-end vocal f0 estimation for polyphonic music
- [Singing Voice Melody Transcription Using Deep Neural Networks](https://wp.nyu.edu/ismir2016/wp-content/uploads/sites/2294/2016/07/163_Paper.pdf)
  - ISMIR 2016
  - f0 estimation for polyphonic music
- [CREPE: A CONVOLUTIONAL REPRESENTATION FOR PITCH ESTIMATION](https://arxiv.org/pdf/1802.06182.pdf) 
  - ICASSP 2018
  - independent temporal smoothness: 10ms hop size (default)
  - addressed harmony
- [PYIN: A fundamental frequency estimator using probabilistic threshold distributions](https://ieeexplore.ieee.org/document/6853678)
  - ICASSP 2014
  - statistical model

### Note-level

- [Omnizart: A general toolbox for automatic music transcription](https://arxiv.org/pdf/2106.00497.pdf)
  - arxiv 2021
  - python library
  - including VOCANO

- [VOCANO: A note transcription framework for singing voice in polyphonic music](https://archives.ismir.net/ismir2021/paper/000036.pdf)
  - ISMIR 2021
  - singing voice separation → monophonic singing
  - frame-level pitch extraction → note segmentation
- [Bayesian singing transcription based on a hierarchical generative model of keys, musical notes, and F0 trajectories](https://eita-nakamura.github.io/articles/Nishikimi_etal_BayesianSingingTranscription_2020.pdf)
  - TASLP 2020
  - statistical method for f0 estimation
  - time-frequency quantization
  - musical score model: f0 +  time units → musical notes

- [Hierarchical Classification Networks for Singing Voice Segmentation and Transcription](https://archives.ismir.net/ismir2019/paper/000111.pdf)
  - ISMIR 2019
  - monophonic singing voice
  - note segmentation model + pitch contour → note-level transcription 
- [Automatic singing transcription based on encoder-decoder recurrent neural networks with a weakly-supervised attention mechanism](https://ieeexplore.ieee.org/abstract/document/8683024/?casa_token=FCeIuK9eKt0AAAAA:sI_ex_8Iwqm6uEXYn2S1xkwYWwQ30BRnAqclNqe1KfohrwRS23cjSxDaTyRKlM_xexD-IcCFC2I)
  - ICASSP 2019
  - monophonic singing
  - attention-based encoder-decoder model: spectrogram → E → D → pitch + note

- [Probabilistic transcription of sung melody using a pitch dynamic model](http://jblsmith.github.io/documents/yang2017-icassp-transcription_sung_melody.pdf)
  - ICASSP 2017
  - pYin + statistical method for note-level vocal melody estimation
- [Musical note estimation for F0 trajectories of singing voices based on a Bayesian semi-beat-synchronous HMM](https://wp.nyu.edu/ismir2016/wp-content/uploads/sites/2294/2016/07/004_Paper.pdf)
  - ISMIR 2016
  - statistical music note estimation from a temporal trajectory of vocal F0s （beat tracking）

### Others

- [Computer-aided melody note transcription using the tony software: Accuracy and efficiency](http://tenor2015.tenor-conference.org/papers/04-Mauch-Tony.pdf)
  - SMC 2015
  - interactive software for note-level vocal melody annotation
- [DALI: a large dataset of synchronized audio, lyrics and notes, automatically created using teacher-student machine learning paradigm](https://arxiv.org/pdf/1906.10606.pdf)
  - ISMIR 2018
  - dataset: audio, time-aligned vocal melody notes, time-aligned lyric
- [Medleydb: A multitrack dataset for annotation-intensive mir research](https://www.researchgate.net/profile/Justin-Salamon/publication/265508421_MedleyDB_A_Multitrack_Dataset_for_Annotation-Intensive_MIR_Research/links/54106cc70cf2f2b29a4109ff/MedleyDB-A-Multitrack-Dataset-for-Annotation-Intensive-MIR-Research.pdf)
  - ISMIR 2014
  - dataset

## Singing Lyrics Transcription

### Singing Recognition

- [MSTRE-Net: Multistreaming Acoustic Modeling for Automatic Lyrics Transcription](https://arxiv.org/abs/2108.02625)
  - ISMIR 2021
  - both polyphonic and monophonic recordings
  - new test set
  - a compact variant of [MTDNN](https://ieeexplore.ieee.org/abstract/document/9003730/?casa_token=I7y5OWnfieIAAAAA:t_0IPvto8K3HmdnxMmseBOS9gEz5ISXjdT19zMziYombswhoQgObaXnrp4bhmA5YNRDYypXXEA)
- [Automatic lyrics transcription using dilated convolutional neural networks with self-attention](https://ieeexplore.ieee.org/abstract/document/9207052/?casa_token=Zee-eWreAr0AAAAA:IxD64t159W6EwqecWEMT2yqASGbmp4MMV5O6iT1knxsVEAM3k8I2GF_9bCDJolW2fvMm9PHP7lo)
  - IJCNN 2020
  - monophonic singing
- [Automatic Lyric Transcription from Karaoke Vocal Tracks: Resources and a Baseline System](https://www.researchgate.net/publication/335724627_Automatic_Lyric_Transcription_from_Karaoke_Vocal_Tracks_Resources_and_a_Baseline_System)
  - Interspeech 2019
  - baseline

### Lyrics Alignment

- [Low Resource Audio-to-Lyrics Alignment From Polyphonic Music Recordings](https://ieeexplore.ieee.org/abstract/document/9414395/?casa_token=t6XA5T0AliYAAAAA:p8znY79wgiMXcC_-jLcbzonqubGbcIm1erMVWyESrEY-gIPxeTmW5ZFItGcWPC64QJu8aVNOguM)
  - ICASSP 2021
  - extending the pronunciation dictionary
  - rule-based method: vocal segmentation → (acoustic model + extended language model) biased decoding → anchor selection → audio-to-lyrics segmentation
  - lower computational
- [Multilingual lyrics-to-audio alignment](https://program.ismir2020.net/static/final_papers/101.pdf)
  - ISMIR 2020
  - singing voice separation → acoustic model (CTC-based model for multilingual speech recognition) → posterio-gram (+lyrics) → predict alignment annotations
- [End-to-end lyrics alignment for polyphonic music using an audio-to-character recognition model](https://ieeexplore.ieee.org/abstract/document/8683470/?casa_token=mu2FCHctms4AAAAA:Qfi8iq_1R071UzYpyHZRmZjmrfkdN5IQbTPDrNb8Yqs7_udTrkiUSGkzirzIBkZFJcWBNCHsC30)
  - ICASSP 2019
  - viterbi training for lyrics alignment
- [Semi-supervised Lyrics and Solo-singing Alignment](https://ismir2018.ismir.net/doc/pdfs/30_Paper.pdf)
  - ISMIR 2018
  - Singing-Adapted Acoustic Model
  - monophonic singing voice → segmentation → ASR → match lyrics → anchor or non-anchor

