# pdftk

> Docker Image packaging for PDFtk

## Supported tags

- [`latest` (*latest/Dockerfile*)](ubuntu/Dockerfile)

What is PDFtk?

PDFtk is a command-line tool for working with PDFs. It is commonly used for
client-side scripting or server-side processing of PDFs.

PDFtk can:

- Merge PDF Documents or Collate PDF Page Scans;
- Split PDF Pages into a New Document;
- Rotate PDF Documents or Pages;
- Decrypt Input as Necessary (Password Required);
- Encrypt Output as Desired;
- Fill PDF Forms with X/FDF Data and/or Flatten Forms;
- Generate FDF Data Stencils from PDF Forms;
- Apply a Background Watermark or a Foreground Stamp;
- Report PDF Metrics, Bookmarks and Metadata;
- Add/Update PDF Bookmarks or Metadata;
- Attach Files to PDF Pages or the PDF Document;
- Unpack PDF Attachments;
- Burst a PDF Document into Single Pages;
- Uncompress and Re-Compress Page Streams;
- Repair Corrupted PDF (Where Possible).

See the [PDFtk](https://www.pdflabs.com/tools/pdftk-server) tool home page for
further information.

The pdftk package available on Ubuntu and Debian images is actually a port to
java. See the source code [GitLab](https://gitlab.com/pdftk-java/pdftkrepository)
repository.

## How to use this image

For many simple tasks, you can map a volume with your PDFs to work and run the
PDFtk Docker image directly:

```bash
$ docker run -it --rm \
    --name pdftk \
    --user $UID \
    --volume "$PWD/pdftk:/pdftk" \
    --workdir /pdftk \
    pequy/pdftk
```

