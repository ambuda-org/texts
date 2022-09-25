GRETIL
======

All of the texts in this folder were downloaded from [GRETIL][gretil]. At the
time this document was written, all GRETIL texts in this folder were downloaded
on 2020-06-16 from the *Download All Sanskrit Texts* link on the GRETIL
homepage, which is listed under the the *Cumulative Download* section. At the
time of download, the GRETIL homepage said:

> Last Update: 10.09.2020


Data format
-----------

The GRETIL team mass-converted their corpus to TEI XML, so there are often
various small errors in the underlying text data or TEI markup. To make these
documents suitable for use on Ambuda, we have often made small manual
interventions to standardize the data format.

Our changes include:

- fixing underlying encoding errors (e.g. verses modeled as paragraphs)
- assigning each `<lg>` or `<p>` tag a valid `xml:id`
- moving metadata (such as the verse number) from the verse text to an element
  attribute

Generally, all of these files have received minor changes to standardize their
markup as described above. We try to update each text's `<teiHeader>` to
reflect these changes, but texts might slip through without specific changes to
the `<teiHeader>`. So for a full understanding of the changes we've made to
these files, we suggest running the `diff` command-line tool to compare our
files to the ones on GRETIL:

    diff gretil-file.xml ambuda-file.xml


License
-------

We release our manual changes to the public domain; all documents are
available under their original licenses.


[gretil]: http://gretil.sub.uni-goettingen.de/gretil.html
