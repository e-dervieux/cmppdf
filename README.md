# cmppdf

This is a bash script to visually or textually compare two PDF files. 
It can be used with

```
cmppdf FILE1 FILE2                        # compare appearance
cmppdf --text FILE1 FILE2                 # compare text

cmppdf -o OUTPREFIX FILE1 FILE2           # save difference jpegs
cmppdf --text -o - FILE1 FILE2 >diffs.txt # capture diffs

cmppdf -pw COMMON_PASSWORD ... FILE1 FILE2 # handle passwords
cmppdf -pw1 PASS1 -pw2 PASS2 ... FILE1 FILE2

cmppdf --help  # full documentation
```

## Dependencies

This script requires:

  - basic PDF tools such as `pdftotext` and `pdftoppm`
    - `apt-get install poppler-utils` on Linux or
    - `brew install poppler` on MacOS
  - `pdftk`
    - `apt-get install pdftk` on Linux or
    - `brew install  pdftk-java` on MacOS
  - ImageMagick
    - `apt-get install imagemagick` on Linux or
    - `brew install imagemagick ` on MacOS)
  - Core GNU utils such as `b2sum`, which are included in most Linux distribution but may require to be installed on MacOS using `brew install coreutils`

## Authorship and License

This software is distributed under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license (Attribution-ShareAlike 4.0 International). The graphical compare code was originally posted by `linguisticturn` on [StackOverflow](https://stackoverflow.com/a/71011009/11241626) (License CC BY-SA 4.0) and later improved by Jim Avera [in the same thread](https://stackoverflow.com/a/75703176/11241626), who keeps his latest version [on his personal website](https://abhweb.org/jima/cmppdf). I (Emmanuel Dervieux) only posted it on GitHub for the sake of continuation, bug tracking, and possible further improvements if need be.
