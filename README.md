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
- Generate unique and original beats on command
  - We’d probably provide a repository of samples (e.g. hi-hats, snares, 808s)
  - Program would follow basic rhythmic structure and layout samples in an
    artistic way
- Generate comprehensible lyrics
  - Lots of [existing research](https://arxiv.org/pdf/1611.00379.pdf)
- Combine lyrics (via text-to-speech) and beat
  - Text-to-speech program dictates generated lyrics to the given beat (
    following the same rhythmic structure used to generate the beat)
- Do all of that in under a minute and create a website to make the program
  publicly available

### Current Status

Currently, I'm working on combining [Malmi et
al.](https://www.kdd.org/kdd2016/papers/files/adf0399-malmiA.pdf)'s program with
a voice synthesizer to rap machine generated lyrics over existing beats.

### Existing Research

Included in this repository are select papers and patents (in PDF form) to
provide an idea of the existing research within the field of machine creativity
as it relates to music generation.
- [DopeLearning: A Computational Approach to Rap Lyrics
  Generation](https://www.kdd.org/kdd2016/papers/files/adf0399-malmiA.pdf)
  - Malmi et al. contribute a prediction model to identify the next line of
    existing lyrics from a set of candidate next lines.
  - They use this model to combine lines from existing songs, producing lyrics
    with rhyme and meaning.
- [Automatic Music Generating Method and
  Device](https://patentimages.storage.googleapis.com/d5/f7/de/e87de2c3729421/US6506969.pdf)
- [Apparatus for Automatically Composing Music
  Piece](https://patentimages.storage.googleapis.com/1e/7e/12/f97c11fdcb08b1/US4399731.pdf)
