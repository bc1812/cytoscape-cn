#Compile LaTeX codes from SVN on various platform

# Introduction #

This page will tell you how to compile the LaTeX codes from SVN code base to get the latest version of Cytoscape's manual in Chinese. I try my best to make the method described in this page works on different OSes and LaTeX distributions. Please let me know if any problem.


# Details #

On Windows:
  1. Install a LaTeX distribution. For Windows, MikTeX is highly recommended; for other OSs, TeX Live is a good choice.
  1. Install a SVN client, TortoiseSVN is highly recommended.
  1. Check out source codes, images, and other necessary files.
```
svn checkout http://cytoscape-cn.googlecode.com/svn/trunk/ cytoscape-cn-read-only
```
  1. Switch to the _cytoscape-cn-read-only_ directory, and compile the file named _Cytoscape\_manual.tex_ with _pdflatex_:
```
pdflatex Cytoscape_manual.tex
```