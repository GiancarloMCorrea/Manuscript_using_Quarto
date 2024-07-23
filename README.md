# Write your manuscript with Quarto

There are already some tutorials and templates to write scientific manuscripts (e.g., [this tutorial](https://quarto.org/docs/journals/)), which will commonly generate a journal-style PDF. Generating a PDF is okay and has several advantages; however, I am a non-native English speaker, and I rely on grammar checkers (e.g., [Grammarly](https://www.grammarly.com/)) to improve my writing. Grammar checkers do not normally work well with PDF documents, and that is the main reason why I have avoided to use Quarto or Rmarkdown to write manuscripts so far. However, I recently found out a nice way to generate Word (*.docx*) documents with a journal style using Quarto. 

In this repository, you will find the following files/folders:

- `_extensions`: folder that contains the style for the authors information.
- `images`: folder where the images are stored. 
- `tables`: folder where the tables (e.g., csv, xlsx) are stored.
- `canadian-journal-of-fisheries-and-aquatic-sciences.csl`: file that produces the citation style. You can find more styles used in distinct journals [here](https://github.com/citation-style-language/styles).
- `custom-reference-doc.docx`: file that contains the Word document style. I recommend not to edit this document, and be careful if you want to do so. You can find some instructions [here](https://quarto.org/docs/output-formats/ms-word-templates.html).
- `manuscript.qmd`: Quarto file where you will write your manuscript. 
- `references.bib`: Bibtex file where your citations information will be stored. You **do not** need to edit this file manually, it will be updated automatically. See more below.

## How to start writing my manuscript?

Clone this repository and make changes to the `manuscript.qmd` file. It will generate a Word file (`manuscript.docx`) when rendered.

## Pros

- Using the RStudio environment to write, which can be more intuitive than Word.
- Avoid dealing with slow Word documents. This has happened to me during the last few years. For some reason (probably due to several citations), some manucripts written in Word are **very slow** to edit.
- Keep track of your changes when using Github.
- Efficient management of citations (see more below).
- Use your grammar checker in the traditional way, if needed.
- More efficient collaboration with coauthors when using Github (assuming they are familiar with Quarto).
- The generated Word file can be shared with coauthors for review if they are not familiar with Quarto.
- Writing equations in Quarto is so much easier than Word.

## Cons

- You will always need to make edits in the Quarto file. So, tracked changes or comments in Word from collaborators cannot be saved.
- Producing elaborated tables is not efficient when generating Word documents using Quarto. So you will only be able to make simple tables (as far as I know).
- You will need to produce your figures as PNG files since that format works better (figure dimensions are mantained) when producing Word files from Quarto. 

## Tips

You can always edit the generated Word document as you wish before submitting your manuscript. Be sure to do these edits when you are done working from Quarto.

## Reference management

There are two main options to manage your citations in Quarto. 

1. Using a reference manager like Zotero. You can find a tutorial to link Quarto with Zotero [here](https://giancarlomcorrea.netlify.app/post/zotero-and-quarto/). The `manuscript.qmd` file was written using this approach.
2. Using [CiteDrive](https://www.citedrive.com/en/), which is quite efficient based on my experience. You could find a tutorial to use CiteDrive and Quarto [here](https://www.citedrive.com/en/quarto/). You will need to slightly modify the `manuscript.qmd` to use this approach.