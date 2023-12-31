# Introduction
A Python code designed to import some entries from a BibTex (.bib) bibliography and print them in a convenient Github Markdown (.md) format. For those people who are not familiar with Python, a Mathematica notebook is provided as well, which fulfills the same goal.

# Example

As an example, we use the code to import four entries (Bettles2016EnhancedArray, Shahmoon2017CooperativeArrays, Rui2020ALayer and Manzoni2018OptimizationArrays, in this order), from the file "example.bib". The format of these entries is the usual BibTeX format (the same automatic format provided, for example, by [Mendeley](https://www.mendeley.com/search/) reference manager). This can be exemplified by:

```BibTex
@article{Bettles2016EnhancedArray,
    title = {{Enhanced Optical Cross Section via Collective Coupling of Atomic Dipoles in a 2D Array}},
    year = {2016},
    journal = {Physical Review Letters},
    author = {Bettles, Robert J. and Gardiner, Simon A. and Adams, Charles S.},
    number = {10},
    month = {3},
    pages = {103602},
    volume = {116},
    publisher = {American Physical Society},
    url = {https://link.aps.org/doi/10.1103/PhysRevLett.116.103602},
    doi = {10.1103/PhysRevLett.116.103602},
    issn = {0031-9007}
}
```
Some entries can be empty or undefined. 
Here below, as an example, the starting index is defined as 18, leading to the output format:

```Markdown
<a id="Bettles2016EnhancedArray">[18]</a>
Bettles Robert J., Gardiner Simon A., Adams Charles S.,
*Enhanced Optical Cross Section via Collective Coupling of Atomic Dipoles in a 2D Array*,
[Physical Review Letters 116, 103602](https://dx.doi.org/10.1103/PhysRevLett.116.103602) (2016)
```

In a Markdown environment, the output of the four entries mentioned above will look like:

<a id="Bettles2016EnhancedArray">[18]</a>
Bettles Robert J., Gardiner Simon A., Adams Charles S.,
*Enhanced Optical Cross Section via Collective Coupling of Atomic Dipoles in a 2D Array*,
[Physical Review Letters 116, 103602](https://dx.doi.org/10.1103/PhysRevLett.116.103602) (2016)

<a id="Shahmoon2017CooperativeArrays">[19]</a>
Shahmoon Ephraim, Wild Dominik S., Lukin Mikhail D., Yelin Susanne F.,
*Cooperative Resonances in Light Scattering from Two-Dimensional Atomic Arrays*,
[Physical Review Letters 118, 113601](https://dx.doi.org/10.1103/PhysRevLett.118.113601) (2017)

<a id="Rui2020ALayer">[20]</a>
Rui Jun, Wei David, Rubio-Abadal Antonio, Hollerith Simon, Zeiher Johannes, Stamper-Kurn Dan M., Gross Christian, Bloch Immanuel,
*A subradiant optical mirror formed by a single structured atomic layer*,
[Nature 583, 369-374](https://dx.doi.org/10.1038/s41586-020-2463-x) (2020)

<a id="Manzoni2018OptimizationArrays">[21]</a>
Manzoni M. T., Moreno-Cardoner M., Asenjo-Garcia A., Porto J. V., Gorshkov A. V., Chang D. E.,
*Optimization of photon storage fidelity in ordered atomic arrays*,
[New Journal of Physics 20, 83048](https://dx.doi.org/10.1088/1367-2630/aadb74) (2018)

In the Markdown text, the entries are hyperlinked via their entry name, e.g. `[18](#Bettles2016EnhancedArray)` becomes [18](#Bettles2016EnhancedArray).

