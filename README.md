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

## Citing

TBA.
