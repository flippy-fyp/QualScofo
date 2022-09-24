# QualScofo

A **Qual**itative **Sco**re-**fo**llowing dataset.

See the [project report](https://arxiv.org/abs/2205.03247) for more information.

## Structure

```bash
|---<GROUP_ID>
    |---<PIECE_ID>
        |---<PIECE>.mid     # Score midi
            <PIECE>.mscz    # Score MuseScore file
            <PIECE>.mxl     # Score MusicXML file
            <PIECE>.pdf     # Score PDF file
            <PIECE>.wav     # Performance audio wave file
            |---raw
                # Contains raw files used to create the data in the parent directory (e.g. full preformance mp3, full MuseScore file, etc.)
```

Possible combinations of `<GROUP_ID>` and `<PIECE_ID>` are:

```bash
cello
|---suite1
octet
|---mendelssohn
orchestra
|---peer
    eine
    1812-1
    1812-2
piano
|---clair
    entertainer
    fugue
    gnossienne
    moonlight
    prelude
    turkish
    unsospiro
violin
|---chaconne-arp
    chaconne-front
```

## Sources

The scores and performance audio files are obtained from [MuseScore.com](https://musescore.com) and [YouTube](https://youtube.com) respectively. [Downloadasaur](https://www.downloadasaur.com) was used to obtain audio files from YouTube.

The URLs to the original source can be obtained by using the following URL format:
```
https://bit.ly/qualscofo-(musescore|youtube)-<GROUP_ID>-<PIECE_ID_PREDASH>
```

`<PIECE_ID_PREDASH>` denotes the Piece ID characters prior to the first occuring dash (`-`).

For instance, the YouTube URL for the `chaconne-arp` piece in the `violin` group is
```
https://bit.ly/qualscofo-youtube-violin-chaconne
```

Note that the performance audio of the pieces `prelude` and `fugue` in the `piano` group are not obtained from YouTube but from the [MAESTRO dataset](https://magenta.tensorflow.org/datasets/maestro).

## Copyright Disclaimer

Fair use: Research.

```
Under section 107 of the Copyright Act of 1976, allowance is made for "fair use" for purposes such as criticism, comment, news reporting, teaching, scholarship, education and research. Fair use is a use permitted by copyright statute that might otherwise be infringing.
```

## Citing

### BibTeX
```
@misc{https://doi.org/10.48550/arxiv.2205.03247,
  doi = {10.48550/ARXIV.2205.03247},
  url = {https://arxiv.org/abs/2205.03247},
  author = {Lee, Lin Hao},
  keywords = {Sound (cs.SD), Audio and Speech Processing (eess.AS), FOS: Computer and information sciences, FOS: Computer and information sciences, FOS: Electrical engineering, electronic engineering, information engineering, FOS: Electrical engineering, electronic engineering, information engineering},
  title = {Musical Score Following and Audio Alignment},
  publisher = {arXiv},
  year = {2022},
  copyright = {Creative Commons Attribution 4.0 International}
}
```
