# All Things Citation

Hi! This page will help you understand how to use pandoc as a way to integrate citations and references into your markdown and html file

**The Basics:**

Hopefully, by this stage you are comfortable and familiar with pandoc. When wanting to integrate citations into a markdown file there are a few things you need to do first. 
- First, it helps if you have the pdf of your articles. I find that if you use Zotero for your references importing the pdf gives you the best information. 
	- From there you can usually export your Zotero collection as a .bib file by exporting the collection as a bibtex format. 
	- This new .bib file allows us to have the references in one place. On a mac if you opened the .bib file it would open it in a reference manager.
- Second, you need to get a citation style file. This is usually denoted with .csl. For APA formating you can find and download the corresponding csl file from [here](https://www.zotero.org/styles). 
- In sum to add a citation to your markdown file you need to make use of three things: the bib file, csl file and later pandoc. 

**What are Bibliography Files (.bib)?**

Bibliography files are a way for your computer to gather and store your references. In a .bib file you will find what is called a citation key. A citation key allows you to tell the computer which article you are referring to. 

**How to Cite References in a Markdown File:**

To cite things in your markdown file you would need to put square brackets and the @ symbol around the citation key.
- For example if you wanted to cite an article with a citation key of "Heitzner2023" you would write your text "In the paper they used a variety of methods [@Hetizner2023]" this would then turn into the relevant in text citation for your output. 
- Lets say you wanted to add page numbers you could do the following "The authors used a specific method [@Heitzner2023 p. 14]" the output would then include the page number in the in text citation. 

**How to Use Pandoc for the Conversion:**

To use pandoc for the conversion you will need to open up your terminal again and specify the correct working directory that includes your markdown file, CSL file, and bibliography file. From there you can run the following command:
- pandoc filename.md --csl=apa.csl --filename.bib --citeproc --output filename.html
- Hopefully if things were done correctly you should have an html file with the in text citations and generated reference list. 

**Conclusion**

Pandoc can be useful for adding references and citations to an html file from a markdown file without having to fully write out all of the information. 