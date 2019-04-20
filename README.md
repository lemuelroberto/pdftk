# pdftk

> Docker Image packaging for PDFtk

pdftk port to java a Handy Tool for Manipulating PDF Documents.

Application source code repository: https://gitlab.com/pdftk-java/pdftk.

PDFtk tool home page: https://www.pdflabs.com/tools/pdftk-server.

## How to run

For many simple tasks, you can map a volume with your PDFs to work and run the
PDFtk Docker image directly:

```bash
$ docker run -it --rm --name pdftk -v "$PWD/pdftk:/pdftk" -u 1000 -w /pdftk pequy/pdftk
```

