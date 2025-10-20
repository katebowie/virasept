<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a id="readme-top"></a>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/katebowie/virasept">
    <img src="images/sink.png" alt="Logo" width="90" height="90">
  </a>

<h3 align="center">Disinfection of Hospital Sink Drains Enriches Pseudomonadota and Efflux Pump-Mediated Antibiotic Resistance in Reestablished Biofilms</h3><br>

  <p align="left">
    Biofilms growing in the sink drains of healthcare facilities are known to harbor pathogens and to also be the source of hospital-acquired infections. Many are exploring disinfection strategies to control these biofilms, however the effects of such interventions have not been well studied. 
    <br />
    <br />
    <br />
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#overview">Overview</a>
      <ul>
        <li><a href="#terms">Terms</a></li>
        <li><a href="#dataset">Dataset</a></li>
        <li><a href="#data-files">Data Files</a></li>
      </ul>
    </li>
    <li>
      <a href="#requirements">Requirements</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>




<!-- GETTING STARTED -->
## Overview

Here we have the code used to analyze data from our paper <i>"Disinfection of Hospital Sink Drains Enriches Pseudomonadota and Efflux Pump-Mediated Antibiotic Resistance in Reestablished Biofilms"</i>. There are two categories of code here: bash scripts used to process the raw data, and the R code used for downstream analysis. 

All R scripts are HTMLs and should be run using R and RStudio. The code is numbered in order of analysis.

The raw data is available on the NCBI SRA (accession number: PRJNA1310651). 


### Terms

<u>ARGs</u> — antibiotic-resistance genes<br>
<u>MAGs</u> — metagenome-assembled genomes



### Dataset

We generated the following datasets for this study:
* 24-hour culture colony counts for 156 sink drain biofilm samples 
* shotgun metagenomic data from 119 biofilm samples
* shotgun metagenomic data from 2 positive controls (mock community from [Zymo](https://www.zymoresearch.com/collections/zymobiomics-microbial-community-standards/products/zymobiomics-microbial-community-standard))
* shotgun metagenomic data from 2 negative controls
* pacbio long-read metagenomic data from 24 biofilm samples


### Data Files

Outside of the raw data, the processed data is as follows:
* CSV with metadata including colony counts from culture data --> [meta_deidentified](https://github.com/katebowie/virasept/blob/main/meta_deidentified.csv)
* ARG information for shotgun metagenomics --> [SR_AMR_deidentified](https://github.com/katebowie/virasept/blob/main/SR_merged_AMR_deidentified.csv)
* CSV with metadata from pacbio long-read sequencing --> [pb_metadata](https://github.com/katebowie/virasept/blob/main/pb_metadata_deidentified.xlsx)
* ARG information for the pacbio long-read sequencing MAGs --> [rgi_output](https://github.com/katebowie/virasept/blob/main/all_rgi_output_parsed.csv)
* Contig coverage of the MAGs for the pacbio long-read sequencing data --> [contig_coverage_summary](https://github.com/katebowie/virasept/blob/main/contig_coverage_summary.csv)
* Plasmid coverage from the pacbio long-read sequencing --> [plasmid_contig_coverage](https://github.com/katebowie/virasept/blob/main/plasmid_contig_coverage.tsv)
* Plasmid scores from the pacbio long-read sequencing --> [plasmid_scores](https://github.com/katebowie/virasept/blob/main/plasmid_scores.tsv)
* ARG information on plasmids from pacbio long-read sequencing --> [plasmid_ARGs](https://github.com/katebowie/virasept/blob/main/plasmid_ARGs.tsv)
* <i>The remaining processed data files are too big for github. We are in the process of hosting them on a different website and will update ASAP</i>
* Taxonomy table for shotgun metagenomics --> []()
* OTU table for shotgun metagenomics --> []()
  

### Requirements for data processing

1. Download files for [Pacbio HiFi MAG Pipeline](https://github.com/PacificBiosciences/pb-metagenomics-tools/blob/master/docs/Tutorial-HiFi-MAG-Pipeline.md)
2. Anvio version 8
3. Still under construction... 

<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- CONTACT -->
## Contact

Kate Bowie - [@katerbowie](https://twitter.com/katerbowie) - kate.bowie@yale.edu

Project Link: [https://github.com/katebowie/virasept](https://github.com/katebowie/virasept)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [The noun project](https://thenounproject.com) - sink at top by Nendra Wahyu Kuncoro from Noun Project (CC BY 3.0)
* []()
* []()

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/katebowie/virasept.svg?style=for-the-badge
[contributors-url]: https://github.com/katebowie/virasept/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/katebowie/virasept.svg?style=for-the-badge
[forks-url]: https://github.com/katebowie/virasept/network/members
[stars-shield]: https://img.shields.io/github/stars/katebowie/virasept.svg?style=for-the-badge
[stars-url]: https://github.com/katebowie/virasept/stargazers
[issues-shield]: https://img.shields.io/github/issues/katebowie/virasept.svg?style=for-the-badge
[issues-url]: https://github.com/katebowie/virasept/issues
[license-shield]: https://img.shields.io/github/license/katebowie/virasept.svg?style=for-the-badge
[license-url]: https://github.com/katebowie/virasept/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
<!-- Shields.io badges. You can a comprehensive list with many more badges at: https://github.com/inttter/md-badges -->
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 
