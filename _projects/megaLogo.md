---
layout: post
title: megaLogo
description: Software designed to create large logoplots for deep mutational scanning data with customizability.
---

megaLogo
============

<a href="https://github.com/meganstumpf/megalogo"><img src="https://i.postimg.cc/50yrsgpH/megalogo-smaller.jpg" width=200px></a>

This project was aimed to design code to create large logoplots for deep mutational scanning data with customizability. These plots visualize the absence/presence of amino acid mutations at all mutated codon positions above specified quality and count filters. Made in collaboration with Tonya Brunetti.

To model its use, I generated a test data set that randomly assigned both the number (`NDET`) and identity of amino acids (`AA`) to individual codon positions (`POSITION`) and calculated equal ratios for each residue. This software relies on this ratio (`MERGE_FRAC`) to generate the height of each amino acid. This means, the height of each amino acid inversely corresponds to the detected diversity at each site, i.e., larger letters = less mutational tolerance. This metric was created to help quickly identify sites with differences in mutational tolerance in a more readable format. A sample logoplot using the test data set is shown below:
<br><br>

<div align = center>
<img src = "https://github.com/meganstumpf/megalogo/blob/master/outputs/sample.png?raw=true" width = 400px>
</div>
<br><br>

Want to try the software out yourself? Head on over to the GitHub repository: (https://github.com/meganstumpf/megalogo)[https://github.com/meganstumpf/megalogo] and follow the instructions!
