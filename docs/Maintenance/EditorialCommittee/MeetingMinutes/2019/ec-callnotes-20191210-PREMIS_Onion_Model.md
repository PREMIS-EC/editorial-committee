**EC PREMIS Subgroup call: “PREMIS Onion Model”**

**2019-12-10 17:00 CET**

**Participants:**

Bertrand Caron

Sara Romkey

Karin Bredenberg

Jack O’Sullivan

Micky Lindlar

Lina Bountouri

Eld Zierau

Betrand walks us through the presentation again. First step was to
extract information about compound / compressed objects from the data
dictionary. Bertrand considered compressed and encrypted descriptions to
be related, at times even competing against each other.

Two possibilities to describe compound objects:

1.  **“Onion model”**

-   Has different composition levels (expects integer value, indicating
    > number of actions you have to perform to access content)

1.  Filestream / BItstream model

-   In addition to the onion model

**Decision tree:**

-   Is the file compressed or encrypted?

    -   If no → no composition level / composition level 0

    -   If yes → 2 composition levels 0 (compressed) and 1 (file after
        > decompression)y

-   Further decision based on number of files contained within

    -   If yes & &lt;= 1 file contained, onion model can be used, but
        > doesn’t have to be

    -   If used, it results in n + 1 PREMIS Files w/ 1
        > objectCharacteristics each

        -   1 file for the container, compositionLevel = 0

        -   n Files for the contained fielstreams, compostionLevel=1

**Example 2: gzipped WARC contained multiple files**

-   2 levels of composition

    -   Gzip file

    -   WARC file

-   PDF file within WARC is considered a separate file

-   Question from Micky: why is the PDF not part of File1 as well?

-   Eld: the relation is captured in the relationship container, what I
    > am missing there is composition level 3 as an information there

-   Bertrand: yes, there appears to be something missing here.
    > Certainly, file2 would need to have compositionLevel 2 or not be
    > there at all.

-   Micky / Eld: it would be good to have the compositionLevel at the
    > relationship level as well, especially as FIle2 is an integral
    > part of File1

**Example 3: a ZIP file compressing 3 PDF files**

-   FIle1 is the ZIP file with a relationshipType derivation

-   File2 (and File3, File4) are the PDF files

**Example 4: 3 PDF files extracted from the ZIP file containing them
(stored in the Repo alongside the original file)**

-   File1 is the ZIP file

-   Every PDF extracted file would have different information about
    > storage and contentLocation (as opposed to example3, where they
    > shared storage and contentInformation with File1/the zip)

-   Micky: File2 is the file contained within file1, not the extracted
    > file, as in this case the compositionLevel would have to be 0

-   Jack: there must be a separate conceptual file we are currently not
    > seeing?

-   Bertrand: yes, it seems that in this example there would be 7 PREMIS
    > files, but it is a pretty theoretical example

**Ontology**

-   In the ontology, there is no objectCharacteristics class (so there
    > is no way to distinguish the “onion model” from the Filestream
    > case, where two files are described)

    -   However, there is a premis:compositionLevel entity that can be
        > applied to the file

**Questions:**

-   Are examples and tree relevant / a reasonable interpretation of how
    > PREMIS handles compound Objects?

-   If we need to interpret the DD, is there some documentation missing
    > about describing compound Objects?

    -   Also: do we need both models? Onion model AND
        > filestream/bitstream model? Should we, e.g. eliminate one
        > during the next DD revision

-   Is maintaining the two solutions (DD/XML and ontology) acceptable or
    > do we need to reconcile them somehow (either by eliminating the
    > objectCharacteristics level in the DD or by adding a class with
    > the same name in the ontology)?

-   BnF example: often packages (ZIP files, ISO images, etc.) are
    > created precisely for not having to manage / describe its content
    > at the file level

    -   Describe WARC GZIP files with the onion model for the top two
        > levels (0 = GZIP, 1 = WARC)

    -   Then use in-house metadata format containerMD: [<span
        > class="underline">http://bibnum.bnf.fr/containerMD-v1\_1/index.html</span>](http://bibnum.bnf.fr/containerMD-v1_1/indexhtml)
        > which allows to describe globally packaged files as entries
        > grouped by format

Next step:  
- everybody look at this during christmas break

-   Will discuss in January meeting, deciding if / how we will move
    > forward with this
