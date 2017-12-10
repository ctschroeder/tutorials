# Digital Editions and Lexicons

## Optional Reading before the Workshop
[Amy Earhart, "The Digital Edition and the Digital Humanities," Textual Cultures 7.1 (2012)](https://github.com/ctschroeder/tutorials/blob/master/basel/files/earhart.pdf)

## Fonts 
Best practices are to use Unicode characters for languages with non-Latin charactersets.  Computational work in particular is difficult with legacy fonts that use the Latin alphabet characters visualized as foreign language characters.  Sharing of data is also easier using the Unicode characterset.

Most systems have Greek installed. For Coptic, [download the Antinoou font + keyboard](https://www.evertype.com/fonts/coptic/). 
You need both the font (to visualize the characters) and 
(add embedded webfont discussion later)

## What are Digital Editions and Digitized Corpora?

What are digital editions and digitized text corpora?  This tutorial will generate a discussion about the research purposes of digitized corpora and the how those research methods guide the structure and formation of different corpora.  

### Explore two digital corpora commonly used by scholars of antiquity and late antiquity

Spend some time exploring one or more of the following digital corpora:
  * [Perseus Digital Library Greek and Roman Collection](http://www.perseus.tufts.edu/hopper/collection?collection=Perseus:collection:Greco-Roman) 
    * Scroll down and click on a set of texts
    * Run a search in the box on the right
    * Click on a word -- what happens?
  * [Papyri.info text navigator](http://papyri.info/search)
    * Try filtering using the metadata fields
    * Try changing your font to Coptic and typing in a Coptic word in the search box
    * Try changing your font back to American English and searching for a word in the translation.
  * [Corpus Corporum](http://www.mlat.uzh.ch/MLS/)
    * Click on one of the corpora on the left and explore
    * If you want more guidance, try clicking on the [Patrologia Latina](http://mlat.uzh.ch/MLS/xanfang.php?corpus=2&lang=0)
      * What kind of information does the site tell you about the corpus?
      * Try searching for a Latin word in the lower left. (Let's say "ascesis".) 
        * Search "Verses only"
        * Try a "lemmatized search" -- are the results different?
        * Try "Dictionary display" (note: on my Mac, I needed to hold "command" (not "control") and hit enter)
As you are exploring, ask yourself:
  * What texts are here, what texts aren’t here -- what is the corpus?
  * What else besides “text” is in this corpus?  What other information can I find?
  * What kind of research could I/would I do with this text corpus?
  * Can I tell how the text has been digitized?

If you have time, check out an [aligned digital Hexapla](http://textalign.net/output/new-testament-hexapla.html) of digitized editions of the New Testament in six languages created by Joel Kalvesmaki as part of his [Text Alignment Network project](http://textalign.net/).

### Coptic SCRIPTORIUM Digital Editions

Coptic Scriptorium publishes digital editions of literary Coptic texts.

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
  
After you've played around, here's a review of key features:
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

## Discussion of creating corpora

If you're creating your own digital corpus, Consider: 
  * What kinds of things do you want to digitize and why?  
  * What makes that a "corpus"?  
  * Do you need to annotate your text in any way?  In our corpus architecture, even spelling normalization is an annotation.  What annotations do you need?  Why and how?  
  * What kind of metadata do you need to provide?  
  * What kind of access will you allow others to have to your corpus?  (Consider a license for your corpus and data.)
  
## Text alignment

If you're interested in aligning texts and translations, here are some tools:
  * [Alpheios Text Alignment App](http://www.perseids.org/apps/alignment) (allows you to export XML files of your alignment; created in collaboration with Perseus)
  * [Text Alignment Network](http://textalign.net/)
  * [Ugarit text alignment](http://ugarit.ialigner.com/) (multi-language, not for Ugaritic!)

## Other edition projects

There are many many other edition projects for ancient texts.  I'm sure you know of some you can recommend to the group!! Here are a couple interesting ones.

[Open Greek and Latin](http://www.dh.uni-leipzig.de/wo/projects/open-greek-and-latin-project/) at Leipzig has released a bunch of texts in TEI-XML on [their GitHub site](https://github.com/OpenGreekAndLatin)

If you're interested in New Testament and Old Testament editions, check out these projects in Germany:
  * [New Testament Virtual Manuscript Room](http://ntvmr.uni-muenster.de/) which includes Coptic
  * [Coptic Old Testament Project](http://coptot.manuscriptroom.com/)
  
[Monastica](http://monastica.ht.lu.se/) is technically a database, but it does provide digitized text for the Apophthegmata Patrum in multiple languages, as well.

## Dictionaries and Lexicons

### Greek and Latin

Navigate back to the [Perseus homepage](http://www.perseus.tufts.edu/).  Click on "all search options".  
  * Play around with the dictionary and lexical searches. 
  * What can you find?  What can't you find?
  * Play around with the word study tool -- enter a term, what happens?
  * Are there reusable resources for another project you might wish to create?
  * Can you tell how the text and lexical resources are structured as data?
  * How might you use these results for your research?
  * Can you easily LINK to the lexicon entries from other projects?


Visit [Corpus Corporum](http://www.mlat.uzh.ch/MLS/) again
  * Try searching for a Latin word in the lower left using "Dictionary display" (note: on my Mac, I needed to hold "command" (not "control") and hit enter)
  * Next, go directly to their Latin lexicon at http://www.comphistsem.org/manual_lexicon.html .  Search for some terms.
  * Questions for discussion:
    * How do they get their lemmatized text?
    * Where do they get the dictionary entries from?
    * Can you tell how the text and lexical resources are structured as data?
    * How might you use these results for your research?
    * Can you easily LINK to the lexicon entries from other projects?
  
Note:  integrating lexical files, lemmatized text, or using the Perseus natural language processing tools into your own project is beyond the scope of the bootcamp. However, now that you know more about what's available, you can plot out your own possibilities.

### Coptic Dictionary Online

This part of the tutorial will introduce you to the basic functionality of the [Coptic Dictionary Online](https://corpling.uis.georgetown.edu/coptic-dictionary), created by the KELLIA project.  The KELLIA project is a collaboration between German and US researchers working in Coptic Digital Humanities, funded by the National Endowment for the Humanities and the Deutsche Forschungsgemeinschaft. ([more information](https://corpling.uis.georgetown.edu/coptic-dictionary/about.cgi))

First simply type the search window a Coptic word (in utf-8/unicode Coptic characters).  You can control for dialect and part of speech (N=noun, V=Verb, etc.) or you can leave those options blank.

**Be sure to check out the search tips on [the Help page](https://corpling.uis.georgetown.edu/coptic-dictionary/help.cgi).** Play around with searches for words containing particular suffixes, prefixes, or character strings.

You can even search translations.  Forget what the Coptic word for "river" is?  
  * Try typing "river" into the quick search bar on the top of the screen
  * Or go to the Dictionary home page and try typing "river" into the Translation box.
  * You can search translations in English, French, and German
  
Try searching for a word, such as ϣⲏⲣⲉ ("child, son").  
  * Click on the word ϣⲏⲣⲉ to see the entry
  * Click on the little plant icon.  This is the icon for the search tool for our digital corpus (ANNIS).  You will get the results for all the matching lemmas for ϣⲏⲣⲉ in our corpora.  Take a look.
  
  ![dictionary to Annis image](http://blog.copticscriptorium.org/wp-content/uploads/2016/07/lexicon-to-ANNIS.png)

Questions for discussion:
  * How do they get their lemmatized text?
  * Where do they get the dictionary entries from?
  * Can you tell how the text and lexical resources are structured as data?
  * How might you use these results for your research?
  * Can you easily LINK to the lexicon entries from other projects?
  
Visit the dictionary's [GitHub page](https://github.com/KELLIA/dictionary/) to see the original TEI XML lexicon files and other resources put in to the creation of this program.

## Creating your own digital edition

There are *many* things to consider when creating a digital edition or corpus for research.  First, consider what you want to do with your editions/corpus?
  * What kind of research do you want to do: computational? close reading?
  * In what state is your source text:  manuscripts, out of copyright print editions, copyright print editions, digitized editions (such as Perseus)?
    * If digitized, what is digitized already and how?  Will it suit your needs?  
      * For example, some digital editions are edited, either as critical editions or as editions with normalized spelling/orthography. Is previously edited or "corrected" text suitable for your research?
      * Some digital editions/corpora have been created using OCR (optical character recognition). What is your tolerance for error?  
  * Does your research use plain text corpora or do you need annotations (such as lemmas, that you could link to a lexicon, or geographic entities you could link to gazetteers)? 
      
### Digitizing text

Weigh the pros (speed of creating large corpora) and cons (error rates) of OCR vs manual transcription. Remember that manual transcription and annotation also have error rates.

#### OCR

OCR typically works by training a tool using a set of training texts and then applying the trained program to new documents.  Keep in mind marginalia, footnotes, and other paratexts when OCR'ing.  Preparing your documents for OCR often involves dealing with paratext, sharpening text detail, etc.  There is a wealth of research on OCR; this section provides only an overview of basic tools and considerations.

  * Tools 
    * Tesseract: example of online OCR for Greek/Latin using Tesseract is [Antigrapheus](https://dcthree.github.io/antigrapheus/)
    * Other projects are finding more success with [Ocropus](https://github.com/tmbdev/ocropy), which has a more robust language modeling program

Other resources and projects:
    * UCL has a handwriting recognition project, [Transcriptorium](http://transcriptorium.eu/) for manuscripts in Spanish, German, English, and Dutch. (NOTE the alphabets!)  To my knowledge, no OCR/text recognition project exists for manuscripts in other languages.
    * The [Kitab project](http://kitab-project.org/corpus/) has been working on OCR for Arabic; they would be a good project to consult for anyone interested in non-Latin OCR projects
    
Some projects outsource OCR + annotation for text structure (page, chapter, verse, etc.) and metadata (author, title, date, etc.) to third-party, commercial companies that contract these services.

#### Transcribing and annotating (case study)

Many of you may be familiar with [Papyri.info](http://papyri.info/)'s Papyrological Editor, their transcription + annotation interface

Today in groups, we will transcribe a short Coptic text.  Ideally, one person in your group knows Coptic.  If not, knowledge of Greek should be fine.  Please select someone who has a Coptic keyboard to be your group's primary "scribe." Each group will transcribe a text and provide basic paleographic/manuscript encoding. *Please identify the primary "scribe" to me and I will make that person an account in our transcription program.*

For more detailed documentation on Coptic Scriptorium's transcription practices, visit our [wiki](http://wiki.copticscriptorium.org/doku.php?id=gitdox_workflow); some of this tutorial is taken from that documentation.

If you ever want to digitize a specific text for inclusion in the Coptic Scriptorium corpora and database, we would like to collaborate with you. Please contact us!

Workshop reseource (*open in a new window, or better yet, have someone in your group open this document as a reference while another person is transcribing*): [cheat sheet for transcribing & manuscript annotations](https://github.com/ctschroeder/tutorials/raw/master/basel/files/Transcription-cheat-sheet-for-DH-workshop.pdf)

(Workshop resources, which will be deleted right after: https://www.dropbox.com/s/1jk15i02hh3oc4t/Chaine%2CApophthegmata.pdf?dl=0, https://www.dropbox.com/s/an0hdu5aazgiqw6/AUT_4985-for-Basel.jpg?dl=0)


##### Login and Orientation to GitDox

GitDox is an online XML and spreadsheet editor which uses [GitHub](github.com/CopticScriptorium/) for data storage and versioning. Coptic Scriptorium currently uses GitDox to transcribe texts and edit them in a spreadsheet.  Although you don't need to have a GitHub account to use GitDox, it's helpful.  For the purposes of the this workshop, you don't need an account.  If you want to collaborate with us or use GitDox in the future, you can get an account later.

GitDox is located at https://corpling.uis.georgetown.edu/gitdox/ .  Navigate there on your computer, and login using the username and password I will provide you.

When you log in to GitDox, you see a list of current documents. Use the dropdown menu above the list to display only documents from a certain corpus. You can also use the arrows to the right of each column name to sort by that column.

Documents are assigned to users (as noted in the fifth column). Please only edit documents assigned to you. If you believe a document should be assigned to you but isn't, please contact the person to whom it is currently assigned to confirm that you should be assigned the document before editing it.

Find the text we assigned to you in the workshop.  Click on the "Edit" button for your text.  Assign it to yourself.

##### Saving and Committing

The transcription mode of GitDox has two options for saving work: save and commit. The save button saves changes within GitDox but does not commit those changes to GitHub. Your permission levels will not allow you to commit to GitHub; one of the workshop facilitators will complete this step of the process. Because GitDox depends on an internet connection, it's a good idea to save your work frequently while you're working using the save button.

##### Adding metadata

Use the button at the bottom of the page to add metadata. We've added minimal metadata for the tutorial.  You will need to add your own names.  Click the metadata button.  Enter "annotation" in the first window and people in your group's names separated by commas in the second (e.g., Caroline T. Schroeder, Rebecca Krawiec).  After you click submit, the metadata will appear in a chart on the bottom of the page. You can't edit metadata you've already submitted, but you can delete the entry from the list and re-enter the correct field and information.

##### Transcribing and encoding

Now begin typing in your text.  Use a utf-8 (Unicode) characterset, such as the Antinoou font and keyboard.  Transcribe as you would any manuscript.  You may use regular returns to create line breaks.

You'll notice two "tags" already in your otherwise empty document.  These are XML tags for annotating text.  If you want to annotate something in your text, you'll wrap the relevant text in "tags".  The first tag (the open tag) is in brackets, such as `<TEI>`; the close tage has brackets and a slash, such as `</TEI>` (If you want, you can read more about [TEI XML](http://www.tei-c.org/index.xml) and the [Epidoc](https://sourceforge.net/p/epidoc/wiki/Home/) subset of XML.)

Start your transcription _inside_ the TEI tags.

You will want to encode for information about pages and columns.  
  * `<pb></pb>` The page break tags will wrap around all the text in a given page.  We use what's called an attribute to encode the page number of the manuscript.
  *  `<cb></cb>` Column break tags will wrap around all the text in a given column.

When you open an angle bracket, GitDox suggests tags that are currently available. GitDox will also suggest attributes for tags. Improperly closed tags and other errors are highlighted in red.

If you need to provide other information, such as if a letter in the manuscript is large or ekthetic (hangs out in the margin), see this cheatsheet or our longer [Transcription Guidelines](https://github.com/CopticScriptorium/tagger-part-of-speech/blob/master/scriptorium-transcription-guidelines.pdf) for instructions.

Below, see a sample text encoded as an example:

![screenshot of sample text](https://github.com/CopticScriptorium/NAPS2017/raw/master/images/sample-text.png)

Either while you are typing or after you are done transcribing, separate Coptic bound groups with a space or underscore.  For example:

ⲁϥⲥⲱⲧⲙ̄ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ ⇒ ⲁϥⲥⲱⲧⲙ̄_ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ_

Be sure to separate the punctuation, as well.  

ⲁϥⲥⲱⲧⲙ̄ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ· ⇒ ⲁϥⲥⲱⲧⲙ̄_ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ_·_

Put a separator between all bound groups, even if a bound group ends at the end of a line:

ⲁϥⲥⲱⲧⲙ̄     ⲁϥⲥⲱⲧⲙ̄_
ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ ⇒  ⲛ̄ϭⲓⲡϫⲟⲉⲓⲥ_·_

If you need to provide other information, such as if a letter in the manuscript is large or ekthetic (hangs out in the margin), see the cheatsheet provided in the workshop or our longer [Transcription Guidelines](https://github.com/CopticScriptorium/tagger-part-of-speech/blob/master/scriptorium-transcription-guidelines.pdf) for instructions.

When you are done typing in your text, be sure to SAVE.

We will *ANNOTATE* a text for lemmas, part of speech, etc., on *DAY TWO* of the workshop.

### Publishing your digital edition in an easy to read format

If you have annotated your text in TEI XML, you can easily convert it to a webpage.

One advantage of XML is that you can direct the computer to *visualize* each annotation any way you like if you modify the stylesheet.  So you can visualize the same document in different ways.

TEI XML and stylesheets *can be complex*.  TEI XML also is NOT optimal for complex linguistic and syntactic annotations beyond basic normalization and/or lemmatization.  Densely annotated TEI XML also can be difficult to convert into other data formats.  Nonetheless, TEI XML remains the most common method of marking up text by Humanists.  (Coptic Scriptorium uses TEI only for manuscript information and simple annotations such as lemma, language of origin, part of speech; our full annotation set is available under a different XML schema).  One advantage of TEI XML is that it already provides models for how you can annotate a text. No one project uses the tagset in identical ways.  Although TEI is often cited as a way to enable annotated text to be interoperable and shared, different annotation choices across different projects mean it's not always interoperable out-of-the-box. The ways specific projects annotate their texts may not work for you, but at least you have a vocabulary and tagset to apply without having to reinvent the wheel.

Visit the following links to see how XML is visualized in a Papyri.info, Perseus, and Coptic Scriptorium, as well as the source files
  * Perseus Herodotus: http://www.perseus.tufts.edu/hopper/text?doc=Perseus:text:1999.01.0125
    * click on XML -- look at the TEI XML encoding
  * Perseus Cicero: http://www.perseus.tufts.edu/hopper/text?doc=Perseus:text:1999.02.0010:text=Catil.
    * click on XML -- look at the TEI XML encoding
  * for comparison, check out the more recent Greek XML from Open Greek and Latin 
    * [Read Aesop](http://cts.dh.uni-leipzig.de/text/urn:cts:greekLit:tlg0096.tlg002.First1K-grc1/passage/1-4b/ancient-greek-aesop-fabulae-fabulae-aesopicae-collectae)
    * [View XML](https://raw.githubusercontent.com/OpenGreekAndLatin/First1KGreek/master/data/tlg0096/tlg002/tlg0096.tlg002.First1K-grc1.xml)
    * [View morphological annotation](https://raw.githubusercontent.com/gcelano/LemmatizedAncientGreekXML/master/texts/tlg0096.tlg002.First1K-grc1.xml)
  * Scriptorium TEI source file: https://github.com/CopticScriptorium/corpora/blob/master/AP/apophthegmata.patrum_TEI/AP.004.poemen.65.xml , other source files in https://github.com/CopticScriptorium/corpora/blob/master/AP
  * Papyri.info: http://papyri.info/ddbdp/bgu;1;213
    * click on XML -- look at the TEI XML encoding
  
I will demonstrate creating an HTML file using the XML editor software [Oxygen](https://www.oxygenxml.com/download.html). 

Papyri.info also uses the TEI as the backbone of its searchable database.

Tools:
  * Create your own SUBSET of the TEI XML tagset and a schema to validate your documents at http://www.tei-c.org/Roma/
  * Learn more about stylesheets that work in Oxygen at http://www.tei-c.org/Tools/ and http://www.tei-c.org/release/doc/tei-xsl/

TEI is not required for creating plain text corpora for text analysis using a lot of software. Consider it if you need variable visualizations and/or vocabularies for basic annotations.
