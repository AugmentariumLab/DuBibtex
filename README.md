# DuBibtex
This script merges duplicated bibtex items from a list of .bib files, capitalize the titles, and more importantly, resolve missing DOIs, years.
Sources of DOI: 
* Google
* ACM
* IEEE
* Springer
* Caltech
* Wiley
* arxiv

Please feel free to make any pull requests!

Another useful tool for LaTeX writing is extracting the abstract: http://tool.duruofei.com/abstract, whose source code is added as a submodule here.

Known issues:
* It assumes the first line of each bibtex item contains its bib ID. This is typically true if the bibtex item is from Google Scholar or DBLP

## Run
Edit config.ini and put your list of bib files to 
```sh
inputFileList       =   input.bib,test.bib
```
, next run
```sh
python Dubibtex
```
the new bib file will be generated as output.bib by default

## Dependencies
* Python 3.6
* pip install requests

## License
Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)

## Author
[Ruofei Du](http://duruofei.com)


## References
[BibTeX Format Description](http://www.bibtex.org/Format/)