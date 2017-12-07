# Optional Reading before the Workshop
[Amy Earhart, "The Digital Edition and the Digital Humanities," Textual Cultures 7.1 (2012)](link)

# What are Digital Editions and Digitized Corpora?

What are digital editions and digitized text corpora?  This tutorial will generate a discussion about the research purposes of digitized corpora and the how those research methods guide the structure and formation of different corpora.  

## Explore two digital corpora commonly used by scholars of antiquity and late antiquity

Spend 5 minutes exploring one of the following two digital corpora:
  * [Perseus Digital Library Greek and Roman Collection](http://www.perseus.tufts.edu/hopper/collection?collection=Perseus:collection:Greco-Roman) 
    * Scroll down to Basil for some early Christian texts and click on his Epistles
    * Run a search in the box on the right
    * Click on a word -- what happens?
  * [Papyri.info text navigator](http://papyri.info/search)
    * Try filtering using the metadata fields
    * Try changing your font to Coptic and typing in a Coptic word in the search box
    * Try changing your font back to American English and searching for a word in the translation.

As you are exploring, ask yourself:
  * What texts are here, what texts aren’t here -- what is the corpus?
  * What else besides “text” is in this corpus?  What other information can I find?
  * What kind of research could I/would I do with this text corpus?
  * Can I tell how the text has been digitized?

If you have time, check out an [aligned digital Hexapla](http://textalign.net/output/new-testament-hexapla.html) of digitized editions of the New Testament in six languages created by Joel Kalvesmaki as part of his [Text Alignment Network project](http://textalign.net/).

## Coptic SCRIPTORIUM Digital Editions

Our project publishes digital editions of literary Coptic texts.

Visit [data.copticscriptorium.org](http://data.copticscriptorium.org).  (Go directly to this link, or go to our main site at http://copticscriptorium.org and click on Corpora in the menu.)  This is our web-based repository designed for reading, browsing, retrieving digital editions of Coptic literary texts.  Use the menu to filter for texts.
  * Click on Corpus
  * Select a corpus, like the Apophthegmata Patrum
    * The "Normalized" button will give you a digital edition of the normalized text. 
    * The "Analytic" button will show you an edition of an aligned normalized text, English translation (when available), and part of speech tagging for each word.
    * The "Diplomatic" button will provide a digital edition of a diplomatic manuscript transcription
  * If you're looking at any of these digital editions, scroll down to see the document's _metadata_ (or information about the document).
  
Play around with the filtering and browse through the editions.  Consider:
  * Hover over the text with your cursor. Does anything pop up?
  * Can you click on anything?  What does it do?
  * What texts are here, what texts aren’t here -- what are the corpora?
  * What else besides “text” is in this corpus?  What other information can I find?
  * What kind of research could I/would I do with these text corpora?
  
Want to come back to a text later or cite it?  Make a note of its CTS URN.  A URN is a uniform resource name (a kind of unique identifier).  Our URN's were created using a system called the [Canonical Text Services URNs](http://www.homermultitext.org/hmt-doc/cite/texts/ctsoverview.html).  For example:
  * urn:cts:copticLit:ap is the CTS URN for the Coptic Apophthegmata Patrum corpus
  * urn:cts:copticLit:ap.2 is the CTS URN for the saying in the Coptic AP numbered 2 under Chaîne's numbering system.
  * urn:cts:copticLit:ap.2.monbeg is the CTS URN for saying 2 in the Coptic AP as it appears in the manuscript witness known as codex MONB.EG 
  * You can find the URNs in each document's metadata and in the "Cite this Document" section on the document's page at http://data.copticscriptorium.org
  * **Try it out:** What happens when you type urn:cts:copticLit:shenoute in the box that says "Enter URN" at the top of the screen?  What happens when you type urn:cts:copticLit:shenoute.abraham?  What happens when you click on this link: http://data.copticscriptorium.org/urn:cts:copticLit:shenoute.abraham ?
  
After you've played around, here's a review key features:
  * Normalized editions: English translation (if available) pops up on hover; words linked to the online [Coptic Dictionary](https://corpling.uis.georgetown.edu/coptic-dictionary/) ("Chapter view" for biblical books.)
  * Diplomatic editions: manuscript page number pops up on hover
  * Analytic editions are aligned Coptic/English (if available)/Greek (in Mark and 1 Cor corpora)/part of speech)
  * You can filter using the menu.
  * You can reference and retrieve documents, text groups, and corpora using their CTS URNs.
  * All a document's metadata is underneath the edition.
  * You can search for a string of characters on any document page using the usual command-f command on your computer
  * You can select and copy text, save the html page to your computer, print to pdf just as you do on any other website.
  
If you want to cite a document or visualization in a publication, see the Citation information after each document's metadata.  Also, see our [Citation Guidelines](http://copticscriptorium.org/citation-guidelines.html) page.  **Always make a note of your document URN and relevant metadata, especially the version number and date of the document. You might also want to save the visualization for your own records by saving the webpage or printing to pdf.**

All the editions you see are visualizations generated from text that has been encoded and annotated according to disciplinary standards.  The project releases digitized and annotated text in these formats:
  * Text Encoding Initiative Extensible Markup Language (TEI-XML) files
  * PAULA XML files
  * The online installation of the files in the search and visualization tool (or database) we use (called ANNIS)
  * The raw files used in the ANNIS installation (relANNIS files)

The following buttons will take you to those data files:

![screenshot of buttons](https://github.com/CopticScriptorium/NAPS2017/raw/master/images/buttons.png)

Perseus and Papyri.info also use TEI XML encoding for their digital editions.  Coptic Scriptorium is a multi-disciplinary project; we also release our corpora in PAULA XML files, since the PAULA format is used for linguistic research.

If you're creating your own digital corpus, Consider: 
  * What kinds of things do you want to digitize and why?  
  * What makes that a "corpus"?  
  * Do you need to annotate your text in any way?  In our corpus architecture, even spelling normalization is an annotation.  What annotations do you need?  Why and how?  
  * What kind of metadata do you need to provide?  
  * What kind of access will you allow others to have to your corpus?  (Consider a license for your corpus and data.)
  
If you're interested in aligning texts and translations, here are some tools:
  * [Alpheios Text Alignment App](http://www.perseids.org/apps/alignment) (allows you to export XML files of your alignment; created in collaboration with Perseus)
  * [Text Alignment Network](http://textalign.net/)
  * [Ugarit text alignment](http://ugarit.ialigner.com/)

If you're interested in Coptic New Testament and Old Testament editions, check out these projects in Germany:
  * [New Testament Virtual Manuscript Room](http://ntvmr.uni-muenster.de/) which includes Coptic
  * [Coptic Old Testament Project](http://coptot.manuscriptroom.com/)
