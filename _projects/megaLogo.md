---
layout: post
title: megaLogo
profile:
  align: right
  image: megalogo_smaller.jpg
description: Software for Large Logoplots
order: 1
---

![GitHub last commit](https://img.shields.io/github/last-commit/meganstumpf/meganstumpf.github.io?path=_projects%2FmegaLogo.md&style=plastic&label=Last%20Updated&labelColor=%235F8575%09&color=%23353935%09)

This project was aimed to design code to create large logoplots for deep mutational scanning data with customizability. These plots visualize the absence/presence of amino acid mutations at all mutated codon positions above specified quality and count filters. Made in collaboration with Tonya Brunetti.

To model its use, I generated a test data set that randomly assigned both the number (`NDET`) and identity of amino acids (`AA`) to individual codon positions (`POSITION`) and calculated equal ratios for each residue. This software relies on this ratio (`MERGE_FRAC`) to generate the height of each amino acid. This means that each amino acid's height inversely corresponds to the detected diversity at each site, i.e., larger letters = less mutational tolerance. This metric was created to help quickly identify sites with differences in mutational tolerance in a more readable format. A sample logoplot using the test data set is shown below:

<h4>Example Logoplot:</h4>

<div align = center>
  <br>
<img src = "https://github.com/meganstumpf/megalogo/blob/master/outputs/sample.png?raw=true" width = 400px>
</div>

Additionally, we wanted to visualize which domain of our mutationally scanned proteins a particular site was located in and what the typical (or `WT`) amino acid was for that position. At the time, software that allowed for this large of a protein was not available with customization for features like how many positions to display per line, customization of the tick break intervals, or the option to add these annotations we were after. 

Stay tuned for some more customization options and feel free to submit your own ideas by submitting an issue!

Want to try the software out yourself? Head on over to the GitHub repository: <br>
<a href="https://github.com/meganstumpf/megalogo">https://github.com/meganstumpf/megalogo</a> and follow the instructions!
