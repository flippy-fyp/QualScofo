# QualScofo

A **Qual**itative **Sco**re-**fo**llowing dataset.

See the [project report](https://github.com/flippy-fyp/flippy-report/blob/main/main.pdf) for more information.

## Structure

```bash
|---<GROUP_ID>
    |---<PIECE_ID>
        |---<PIECE>.mid     # score midi
            <PIECE>.mscz    # MuseScore file
            <PIECE>.mxl     # MusicXML file
            <PIECE>.pdf     # PDF file
            <PIECE>.wav     # Performance wave file
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

The scores and performance audio are obtained from [MuseScore.com](https://musescore.com) and [YouTube](https://youtube.com) respectively.

The URLs to the original source can be obtained by using the following URL format:
```
https://bit.ly/qualscofo-(musescore|youtube)-<GROUP_ID>-<PIECE_ID>
```
For instance, the YouTube URL for the `suite1` piece in the `cello` group is 
```
https://bit.ly/qualscofo-youtube-cello-suite1
```

Note that the performance audio of the pieces `prelude` and `fugue` in the `piano` group are not obtained from YouTube but from the [MAESTRO dataset](https://magenta.tensorflow.org/datasets/maestro).

## Copyright Disclaimer

Fair use: Research.

```
Under section 107 of the Copyright Act of 1976, allowance is made for "fair use" for purposes such as criticism, comment, news reporting, teaching, scholarship, education and research. Fair use is a use permitted by copyright statute that might otherwise be infringing.
```

## Citing

TBA.
