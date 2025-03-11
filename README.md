# cmppdf

This is a small bash script to visually compare two PDF files. It can be used with

```
cmppdf path/to/file1.pdf path/to/file2.pdf
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

This software is distributed under the [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license (Attribution-ShareAlike 4.0 International). The graphical compare code was originally posted by `linguisticturn` on [StackOverflow](https://stackoverflow.com/a/71011009/11241626) (License CC BY-SA 4.0) and later improved by Jim Avera [in the same thread](https://stackoverflow.com/a/75703176/11241626), who posted it [on his personal website](https://abhweb.org/jima/cmppdf). I (Emmanuel Dervieux) only posted it on GitHub for the sake of continuation, bug tracking, and possible further improvements if need be.