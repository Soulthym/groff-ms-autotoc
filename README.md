# groff-ms-autotoc
automatic groff Table of Content building from anywhere in the document

automates the numbering of Table of Content references from anywhere in the document.  
By default groff builds automatic TOC references only at the end of the document, with this script you can actually build your table of content from anywhere in your document

# Warning  
This only works for a single TOC in the document so far.  
It is built from a double pass of groff and sed-ing through a .ps version of your document to extract the correct numbers.  
So far only .PX works, so use .bp to page break.  
It is HACKY, so might not work in some circumstances. Feel free to submit a PR if you are able to fix something, or report any bug you find in the issues that isn't referenced in this section.

# Tutorial  
run `:!.compile.sh` from vim and it will compile the current buffer  
