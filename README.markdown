# Internet-Drafts

This respository contains source code and building instructions for
my Internet-Draft documents.


## Requirements

- [mmark][]
- [xml2rfc](https://pypi.org/project/xml2rfc/)
- [GNU Make](https://www.gnu.org/software/make/)
- [xmllint](http://xmlsoft.org/)
- [xsltproc](http://xmlsoft.org/)

[mmark]: https://mmark.miek.nl/


## Organisation

Each file `foo.md` is the source of an Internet-Draft, in the
[mmark][] dialect.

To add `<displayreference>` elements, add them in
`foo-displayref.xml`.  This file is **required** for each markdown
source file, but may contain zero `<displayreference>` elements.


## Building

The build produces XML, HTML and plain text outputs for each input,
under the ``output/foo/`` subdirectory.  The XML file is ready for
submission to the IETF Datatracker.

```shell
make
```
