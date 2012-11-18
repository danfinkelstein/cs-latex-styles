###Readme
Academic LaTeX style sheets for mathematics, physics, and computer science are included in this repository and can easily be deployed on any UNIX-like system where the LaTeX program(s) can be found: simply follow the instructions for setting the `TEXINPUTS` variable and you'll be able to include the appropriate style sheets in your document sources without hunting down the style sheets each time you want to edit a document or paper.

###Instructions
Assuming you've  pulled this  repo into  a subdirectory  of your  home directory
called "`tex`" (and please make  sure you don't accidentally overwrite anything!),
the instructions below  will sweep up the styles into  the `TEXINPUTS` environment
variable so you can call *tex on LaTeX files that use the included style sheets.


####Setting the `TEXINPUTS` variable
Include the following in the `~/.profile` (or equivalent):

	for dir in $HOME/tex/latex/*
	do
	  TEXINPUTS=$TEXINPUTS:$dir
	done

	export TEXINPUTS=.:$TEXINPUTS

####Style sheet sources
The included style sheet sources found in compressed files included in this package in the `src` directory may be out of date, upon occasion, so the sources of the originals are found here:

*	ACM style sheets:
	http://www.acm.org/publications/latex_style/

*	IEEE style sheets:
	http://www.ieee.org/conferences_events/conferences/publishing/templates.html

*	CLRS style sheets:
	http://www.cs.dartmouth.edu/~thc/clrscode/

*	Springer style sheets:
	http://www.springer.com/computer/lncs/lncs+authors?SGWID=0-40209-0-0-0

