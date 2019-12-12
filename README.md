# AAR

### Advanced Authentic Research

The [Advanced Authentic Research (AAR) Program](https://aar.pausd.org) is a
unique opportunity for students in grades 10-12 where it is designed for
students with interest, passion, curiosity, and perseverance to investigate an
authentic topic of their choosing. Students are paired with mentors in the
particular field of research who will support and facilitate each students' work
in their own laboratories, offices, and other settings. The student research
will be supported by the process-oriented curriculum developed by the AAR Team.
The recursive nature of the research process allows students to go back and
forth between the different stages of inquiry as they encounter new information.
The expectation is that students will spend about 60 hours per semester (about
4 hours per week) on their project. The AAR program earns 5 career and technical
education credits per semester.

## My Project

To what extent can we use machine learning techniques to automatically generate
music (namely hip-hop songs)?

### Generating Hip-Hop with Machine Learning

Create a program that can generate an original, 3min song (beat, lyricism,
vocals) given a word or phrase
- Train a GAN to generate unique and original beats on command
  - We’d probably provide a repository of samples (e.g. hi-hats, snares, 808s)
  - Program would follow basic rhythmic structure and layout samples in an
    artistic way
- Generate comprehensible lyrics
  - Lots of [existing research](https://arxiv.org/pdf/1611.00379.pdf) (see below
    list for more)
- Combine lyrics (via text-to-speech) and beat
  - Text-to-speech program dictates generated lyrics to the given beat (
    following the same rhythmic structure used to generate the beat)
- Do all of that in under a minute and create a website to make the program
  publicly available

### Existing Research

Included in this repository are select papers and patents (in PDF form) to
provide an idea of the existing research within the field of machine creativity
as it relates to music generation.

#### Repositories

- [Music Generation with Deep
  Learning](https://github.com/umbrellabeach/music-generation-with-DL)
  - Repository of related papers, conferences, and links to existing projects
    and useful libraries.
- [MuseGAN](https://github.com/salu133445/musegan)
  - Project on music generation. In a nutshell, we aim to generate polyphonic
    music of multiple tracks (instruments). The proposed models are able to
    generate music either from scratch, or by accompanying a track given a
    priori by the user.
  - We train the model with training data collected from
    [Lakh Pianoroll Dataset](https://salu133445.github.io/lakh-pianoroll-dataset/)
    to generate pop song phrases consisting of bass, drums, guitar, piano and
    strings tracks.
  - Sample results are available [here](https://salu133445.github.io/musegan/results).
  - An extension of this project using binary neurons can be found at this
    [repository](https://github.com/salu133445/bmusegan) and on this
    [website](https://salu133445.github.io/bmusegan/).
- [Magenta](https://github.com/tensorflow/magenta)
  - Tensorflow library for creating art and music. Relevant music models
    include:
    - [**MelodyRNN**](https://github.com/tensorflow/magenta/tree/master/magenta/models/melody_rnn) -
      you give it a NoteSequence, and it continues it in the style of your original NoteSequence.
    - [**MusicVAE**](https://github.com/tensorflow/magenta/tree/master/magenta/models/music_vae) -
      generates brand new NoteSequences or interpolates between two sequences.
    - [**Onsets and Frames**](https://github.com/tensorflow/magenta/tree/master/magenta/models/onsets_frames_transcription) -
      transcribes piano audio
  - Magenta is a research project exploring the role of machine learning in the
    process of creating art and music. Primarily this involves developing new
    deep learning and reinforcement learning algorithms for generating songs,
    images, drawings, and other materials. But it's also an exploration in
    building smart tools and interfaces that allow artists and musicians to
    extend (not replace!) their processes using these models. Magenta was
    started by some researchers and engineers from the Google Brain team, but
    many others have contributed significantly to the project. We use TensorFlow
    and release our models and tools in open source on this GitHub. If you’d
    like to learn more about Magenta, check out our blog, where we post
    technical details. You can also join our discussion group.
- [Torchaudio](https://github.com/pytorch/audio)
  - PyTorch library that makes processing and working with audio signals in
    machine learning manageable.

#### Datasets

- [Million Song Dataset](http://millionsongdataset.com/)
  - The **Million Song Dataset** is a freely-available collection of audio features
    and metadata for a million contemporary popular music tracks.
  - Its purposes are:
    - To encourage research on algorithms that scale to commercial sizes
    - To provide a reference dataset for evaluating research
    - As a shortcut alternative to creating a large dataset with APIs (e.g. The Echo Nest's)
    - To help new researchers get started in the MIR field
  - The core of the dataset is the feature analysis and metadata for one million
    songs, provided by The Echo Nest. The dataset does not include any audio,
    only the derived features. Note, however, that sample audio can be fetched
    from services like 7digital, using code we provide.
- [Lakh MIDI Dataset](https://colinraffel.com/projects/lmd/)
  - Collection of 176,581 unique MIDI files, 45,129 of which have been matched
    and aligned to entries in the Million Song Dataset.
  - Created as part of [this paper](https://academiccommons.columbia.edu/doi/10.7916/D8N58MHV)
- [Lakh Pianoroll Dataset](https://salu133445.github.io/lakh-pianoroll-dataset/)
  - Generated by combining MIDIs from the [Lakh MIDI Dataset](https://colinraffel.com/projects/lmd/)
    to create polyphonic pianorolls.
  - Created as part of Dong et al.'s MuseGAN [project](https://github.com/salu133445/musegan)

#### Papers

- [Music Generation using RNNs](https://github.com/unnati-xyz/music-generation)
  - Another experiment for algorithmic music generation using recurrent neural
    networks.
- [DopeLearning: A Computational Approach to Rap Lyrics
  Generation](https://www.kdd.org/kdd2016/papers/files/adf0399-malmiA.pdf)
  - Malmi et al. contribute a prediction model to identify the next line of
    existing lyrics from a set of candidate next lines.
  - They use this model to combine lines from existing songs, producing lyrics
    with rhyme and meaning.
- [Convolutional Generative Adversarial Networks With Binary Neurons for
  Polyphonic Music
  Generation](https://salu133445.github.io/bmusegan/pdf/bmusegan-ismir2018-paper.pdf)
    - Dong et al. contributes a [python project](https://github.com/salu133445/musegan)
      to automatically generate polyphonic pop song phrases (phrases consisting
      of multiple instruments).
- [The Beat Spectrum: A New Approach to Rhythm
  Analysis](http://rotorbrain.com/foote/papers/icme2001.pdf)
  - Foote et al. introduces the *beat spectrum* and *beat spectrogram* to
    automatically characterize and represent the rhythm and tempo of music and
    audio.
- [Query-By-Beat-Boxing: Music Retrieval for the
  DJ](http://rotorbrain.com/foote/papers/icme2001.pdf)
  - Kapur et al. explores a novel method of retrieving automatically classified
    music through the analysis of user created *BeatBoxing*.
  - Describes how the individual *BeatBoxing* sounds can be automatically
    identified and contributes a method of tempo extraction.
- [MySong: Automatic Accompaniment Generation for Vocal
  Melodies](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/mysongchi2008.pdf)
- [Automatic Music Generating Method and
  Device](https://patentimages.storage.googleapis.com/d5/f7/de/e87de2c3729421/US6506969.pdf)
- [Apparatus for Automatically Composing Music
  Piece](https://patentimages.storage.googleapis.com/1e/7e/12/f97c11fdcb08b1/US4399731.pdf)
- [Interactive Music Composition and Performance
  System](https://patentimages.storage.googleapis.com/9b/03/70/5aacca6472b19c/US4526078.pdf)
