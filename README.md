Assuming you've  pulled this  repo into  a subdirectory  of your  home directory
called "tex" (and please make  sure you don't accidentally overwrite anything!),
the instructions below  will sweep up the styles into  the TEXINPUTS environment
variable so you can call *tex on LaTeX files that use the included style sheets.


Include the following in the .profile (or equivalent):

for dir in $HOME/tex/latex/*
do
  TEXINPUTS=$TEXINPUTS:$dir
done

export TEXINPUTS=.:$TEXINPUTS


ACM style sheets:
http://www.acm.org/publications/latex_style/

IEEE style sheets:
http://www.ieee.org/conferences_events/conferences/publishing/templates.html

CLRS style sheets:
http://www.cs.dartmouth.edu/~thc/clrscode/

Springer style sheets:
http://www.springer.com/computer/lncs/lncs+authors?SGWID=0-40209-0-0-0

