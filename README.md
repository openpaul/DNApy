DNApy
=====

A free and open source GUI toolkit for DNA editing - written in python

This project aims to provide a powerful codebase for viewing, editing and creating DNA in the GenBank format. The code is free to use, modify and re-distribute under a GPL license. Contributions in the form of improvements and new functions are welcome and encouraged!

The software is being developed on a GNU/Linux machine and works well in that environment. As the software matures testing will start on Windows and Mac to make sure it is cross-platform, as this is a major goal of development. The only external library that are needed are wxPython and pycairo. Launch main.py to give the software a go (it is still under heavy development though).

![DNApy GUI](Screenshot.png?raw=true "DNApy")

## Testing
To start testing the software you have to install python, wxpython and pycairo. For a Debian based distro this would be possible using apt-get:

```
sudo apt-get install python2.7 python-wxgtk2.8 python-cairo
```

Afterwoards you can download the software and run it:
```
cd ~
git clone https://github.com/mengqvist/DNApy.git
cd DNApy
python main.py
```

Please let us know about any bugs you encounter, using the issue tracker here on GitHub. Also feel free to contribute bugfixes yourself.



## Implemented Software features

* Visualization of DNA sequence with sequence features

* Plasmid view visualization

* DNA editing, copy, paste, reverse complement 

* Unlimited undo/redo 

* Easy search for nucleotide or amino acid positions or sequence

* Easy mutation by nucleotide or amino acid position (this one is pretty awesome!)

* Design of mixed base codons for libraries

* DNA translation to protein

* Addition/removal/modification of genbank features

* Addition/removal/modification of genbank qualifiers



##Not Yet Implemented Software features (and priority list)


* Analysis of sequence reads in the .ab1 format
* Display and handle linear sequences

* Restriction enzyme finder
 - [done] located restrictionsites in dna
 - [partly] display restriction sites in plasmid (missing zoom)
 - [todo] improve DNA editor to visualize cut location

* Addition/removal/modification of genbank header entries 
 - [todo] improve genbank parser to allow parsing of corrupted genbank files from ApE, Serial Cloner, SnapGen Viewer

* DNA codon optimization 

* Fetch genes/plasmids from NCBI 

* Primer design 

* Calculation of ribosome binding strength 

* NCBI blast for homologous genes

* Simulate PCR
* Simulate Gibson assembly
* Simulate restriction digest and/or ligation

* (Multiple) Sequence alignment
* Make DNApy installable using a common package manager. Thus prepare a tar.gz package with the appropriate installation files.



##Project Website
The project has its own website where announcements are made. While all of developing happens here on GitHub releases and such may be published on the website instead:

http://dnapy.org/

