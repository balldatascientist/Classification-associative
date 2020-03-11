# Classification-associative
<b>Article</b> : <font color="blue" size=2> <a href="https://pdfs.semanticscholar.org/ec2c/b3a9abdcad58ea4acb73b1411f7eb98d8472.pdf" target="_blank"> An Integer Optimization Approach to Associative
Classiﬁcation --- Dimitris Bertsimas Allison Chang Cynthia Rudin </a></font>

L’objectif de ce travail est de mettre en pratique la méthode proposée par l'article.

#### Installation

Pour pouvoir exécuter ce projet, il faut:
1. installer
- Julia
- CPLEX (v12.8 ou v12.9): attention, la 12.10 n'est pas compatible avec Julia pour l'instant. 

2. installer les packages: tapez "julia" dans une console, puis :
```
using Pkg
Pkg.add("JuMP")
Pkg.add("DataFrames")
Pkg.add("CSV")
ENV["CPLEX_STUDIO_BINARIES"] = "votre chemin d'installation de cplex (plus d'infos en dessous)"
Pkg.add("CPLEX")
```

Le chemin à indiquer pour CPLEX :
```
# Linux
ENV["CPLEX_STUDIO_BINARIES"] = "/path/to/cplex/bin/x86-64_linux"

# OSX
ENV["CPLEX_STUDIO_BINARIES"] = "/path/to/cplex/bin/x86-64_osx"

# Windows
ENV["CPLEX_STUDIO_BINARIES"] = "C:/IBM/CPLEX_Studio128/cplex/bin/x64_win64"
```
