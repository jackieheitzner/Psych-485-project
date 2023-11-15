# All Things Pandoc

Hi! This page will help you understand pandoc and related software.

**What is Pandoc?**

Pandoc is a universal document converter. It can take word docs and convert them into markdown format or html. Pandoc is a very useful tool when working with different file formats. 

**How to Install Pandoc:**

To instal Pandoc you need to first download the correct package for your computers operating system. The downloads and more installation information can be found [here](https://pandoc.org/installing.html). 

**How to Use Pandoc to Convert From a markdown file to HTML:**

Lets say you wanted to convert your newly written markdown file into an HTML file for your website. You would need to do the following:

1. Opening your terminal (on a mac this should be found in your applications)

2. It can be helpful to make sure that pandoc is installed. In your terminal window you can type `pandoc --version` you should see something like this:

	pandoc 3.1.8
	Features: +server +lua
	Scripting engine: Lua 5.4
	User data directory: /Users/jackie/.local/share/pandoc
	Copyright (C) 2006-2023 John MacFarlane. Web: https://pandoc.org
	This is free software; see the source for copying conditions. There is no warranty, not even for merchantability or fitness for a particular purpose.
	
3. Once you have done that you then need to make sure you are in your correct directory this is so that your computer has access to the correct files that you are trying to convert. 

- On a mac this can be done with the following:
	- "pwd" will tell you what your current working directory is. 
	- "cd" will allow you to change directories 
	- "ls" lists what files are in that current directories. 
	
- So lets say you have the markdown file on your desktop. You would want to do something like the following:
	Jackie@Jackies-MacBook-Pro ~ % pwd
	/Users/jackie
	jackie@Jackies-MacBook-Pro ~ % cd Desktop
	jackie@Jackies-MacBook-Pro Desktop % pwd
	/Users/jackie/Desktop
	That blurb shows that I am now working in my Desktop Directory.
	
4. From there you can use the following command to convert your document for macs: `filename.md -o filename.html` this command can be done in reverse as well to go from .html to .md and if this was all done correctly you should now see the same file but in an html format. 
- For more detailed instructions see the following [website](https://pandoc.org/getting-started.html).

**How to Convert to a pdf format:**

Unfortunately, Pandoc on its own does not support pdf conversion. The good new though is that there is software that you can use that works with pandoc to convert to pdf format.  The software that mac users can use is called MacTeX. You can find the download page for MacTeX [here](https://tug.org/mactex/mactex-download.html). 
- You can follow the installation process and show have successfully installed what you need.   
- If everything is working correctly you should be able to follow the steps above to be in the correct directory while using the following command `pandoc filename.md -o filename.pdf` you should then see your file as a pdf format. 

**Conclusion** 

Pandoc is a very useful tool that you can use to convert files into various other file formats. Pandoc has been useful to me in this project for converting my markdown files into the html files that you see on the website. 
