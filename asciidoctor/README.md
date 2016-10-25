= asciidoctor = 

== Usage ==

To create a HTML version:
`docker run -it -w /opt/ -v $(pwd):/opt/ --rm alexsuch/asciidoctor asciidoctor my-asciidoctor-file.adoc`

To create a PDF version:
`docker run -it -w /opt/ -v $(pwd):/opt/ --rm alexsuch/asciidoctor asciidoctor-pdf my-asciidoctor-file.adoc`

To create an EPUB version:
`docker run -it -w /opt/ -v $(pwd):/opt/ --rm alexsuch/asciidoctor asciidoctor-epub3 my-asciidoctor-file.adoc`
