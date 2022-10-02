# Awesome-Spatio-Temporal-Sentence-Grounding-in-Videos
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<p valign="middle"> <p align="center">  
  <img width="250" src="https://camo.githubusercontent.com/1131548cf666e1150ebd2a52f44776d539f06324/68747470733a2f2f63646e2e7261776769742e636f6d2f73696e647265736f726875732f617765736f6d652f6d61737465722f6d656469612f6c6f676f2e737667" "Awesome!">
</p>

A curated list of Spatio-Temporal Sentence Grounding in Videos papers and benchmarks.  <br/>
This task is the updated version of temporal sentence grounding where the object is not only to localise temporally but also detect the object referred in the query.

<br/>

## Task definition:

  <div align="center" valign="middle"><img height="400px" src="figs/pd.png"></div>

<br/>

# 00 - Table of Contents

* [01 - Datasets](#01%20-%20Datasets)
<!-- * [02 - Benchmark Results](#02%20-%20Benchmark%20Results) -->
* [02 - Papers](#03%20-%20Papers)

<br/>

# 01 - Datasets

<br/>

## Videos Statistics

<table style="table-layout: fixed; margin: 0; padding: 0; ">
  <colgroup>
       <col span="0" style="width: 10%;">
       <col span="0" style="width: 10%;">
       <col span="0" style="width: 20%;">
       <col span="0" style="width: 30%;">
       <col span="0" style="width: 20%;">
       <col span="0" style="width: 10%;">
    </colgroup>
  <tr>
    <td> <p valign="middle"> <p align="left">     Dataset         </p></p></td>
    <td colspan="3"> <p valign="middle"> <p align="center">  Number of Videos </p></p></td>
    <td> <p valign="middle"> <p align="center">   Avg. Query<br/>Duration </p></p></td>
    <td> <p valign="middle"> <p align="center">   Avg. Video<br/>Duration </p></p></td>
  </tr>
  <tr>
    <td></td>
    <td> <p valign="middle"> <p align="center"> Train   </p></p></td>
    <td> <p valign="middle"> <p align="center"> Val     </p></p></td>
    <td> <p valign="middle"> <p align="center"> Test    </p></p></td>
    <td><p valign="middle"> <p align="center">  Sec. </p></p></td>
    <td><p valign="middle"> <p align="center">  Sec.   </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="http://www.coli.uni-saarland.de/projects/smile/page.php?id=software">VidSTG</a>              </p></p></td>
    <td> <p valign="middle"> <p align="center"> 7000    </p></p></td>
    <td> <p valign="middle"> <p align="center"> 835    </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1265   </p></p></td>
    <td> <p valign="middle"> <p align="center">  declarative=11.12 <br/> interrogative=8.98  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 28.01  </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://github.com/tzhhhh123/HC-STVG">HC-STVG</a> </p></p></td>
    <td> <p valign="middle"> <p align="center"> 4500 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0    </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1160 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 5.37 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 20 </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://github.com/tzhhhh123/HC-STVG">HC-STVG2.0</a> </p></p></td>
    <td> <p valign="middle"> <p align="center"> 8511 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1094 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1037 </p></p></td>
    <td> <p valign="middle"> <p align="center"> - </p></p></td>
    <td> <p valign="middle"> <p align="center"> 20 </p></p></td>
  </tr>
</table>

<!-- <br/> -->

<!-- ## Sentences Statistics

<table style="table-layout: fixed; margin: 0; padding: 0; ">
  <colgroup>
       <col span="0" style="width: 10%;">
       <col span="0" style="width: 10%;">
       <col span="0" style="width: 20%;">
       <col span="0" style="width: 30%;">
       <col span="0" style="width: 20%;">
       <col span="0" style="width: 10%;">
    </colgroup>
  <tr>
    <td> <p valign="middle"> <p align="left">     Dataset         </p></p></td>
    <td> <p valign="middle"> <p align="center">   Features<br/>(Download) </p></p></td>
    <td colspan="3"> <p valign="middle"> <p align="center">  Number of Queries </p></p></td>
    <td> <p valign="middle"> <p align="center">   Avg.<br/>Tokens </p></p></td>
    <td> <p valign="middle"> <p align="center">   Total<br/>Tokens </p></p></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
    <td> <p valign="middle"> <p align="center"> Train   </p></p></td>
    <td> <p valign="middle"> <p align="center"> Val     </p></p></td>
    <td> <p valign="middle"> <p align="center"> Test    </p></p></td>
    <td><p valign="middle"> <p align="center">   </p></p></td>
    <td><p valign="middle"> <p align="center"> (Millions)  </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="http://www.coli.uni-saarland.de/projects/smile/page.php?id=software">TACoS</a>              </p></p></td>
    <td> <p valign="middle"> <p align="center">       </p></p></td>
    <td> <p valign="middle"> <p align="center"> 10146 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 4589  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 4083  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 10.5  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.2   </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://allenai.org/plato/charades/">Charades-STA</a> </p></p></td>
    <td> <p valign="middle"> <p align="center">       </p></p></td>
    <td> <p valign="middle"> <p align="center"> 12404 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0     </p></p></td>
    <td> <p valign="middle"> <p align="center"> 3720  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 7.2   </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.1   </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://github.com/LisaAnne/LocalizingMoments">DiDeMo</a> </p></p></td>
    <td> <p valign="middle"> <p align="center">       </p></p></td>
    <td> <p valign="middle"> <p align="center"> 33005 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 4180  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 4021  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 8.0   </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.3   </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="http://cs.stanford.edu/people/ranjaykrishna/densevid/">ActivityNet Captions</a>             </p></p></td>
    <td> <p valign="middle"> <p align="center">       </p></p></td>
    <td> <p valign="middle"> <p align="center"> 37421 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 17505 (val1)<br/>17031(val2) </p></p></td>
    <td> <p valign="middle"> <p align="center"> ?     </p></p></td>
    <td> <p valign="middle"> <p align="center"> 14.8  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1.0   </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="">MAD</a> </p></p></td>
    <td> <p valign="middle"> <p align="center"> <a href="">CLIP</a></p></p></td>
    <td> <p valign="middle"> <p align="center"> 280183    </p></p></td>
    <td> <p valign="middle"> <p align="center"> 32064     </p></p></td>
    <td> <p valign="middle"> <p align="center"> 72044    </p></p></td>
    <td> <p valign="middle"> <p align="center"> 12.7 </p></p></td>
    <td> <p valign="middle"> <p align="center"> 5.0 </p></p></td>
  </tr>
</table>

</br> -->

<!-- ## Language Statistics - (Unique tokens)

<table style="table-layout: fixed; margin: 0; padding: 0; ">
  <colgroup>
       <col span="0" style="width: 10%;">
       <col span="0" style="width: 10%;">
       <col span="0" style="width: 20%;">
       <col span="0" style="width: 30%;">
       <col span="0" style="width: 20%;">
       <col span="0" style="width: 10%;">
    </colgroup>
  <tr>
    <td> <p valign="middle"> <p align="left">    Dataset    </p></p></td>
    <td> <p valign="middle"> <p align="center">  Adjectives </p></p></td>
    <td> <p valign="middle"> <p align="center">  Nouns      </p></p></td>
    <td> <p valign="middle"> <p align="center">  Verbs      </p></p></td>
    <td> <p valign="middle"> <p align="center">  Vocabulary </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="http://www.coli.uni-saarland.de/projects/smile/page.php?id=software">TACoS</a>              </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.2 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.9 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.6 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 2.3 K  </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://allenai.org/plato/charades/">Charades-STA</a> </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.1 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.6 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.4 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1.3 K  </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://github.com/LisaAnne/LocalizingMoments">DiDeMo</a> </p></p></td>
    <td> <p valign="middle"> <p align="center"> 0.6 K </p></p></td>
    <td> <p valign="middle"> <p align="center"> 4.1 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1.9 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 7.5 K  </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="http://cs.stanford.edu/people/ranjaykrishna/densevid/">ActivityNet Captions</a>             </p></p></td>
    <td> <p valign="middle"> <p align="center"> 1.1 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 7.4 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 3.7 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 15.4 K </p></p></td>
  </tr>
  <tr>
    <td> <p valign="middle"> <p align="left">   <a href="https://github.com/Soldelli/MAD">MAD</a> </p></p></td>
    <td> <p valign="middle"> <p align="center"> 5.3 K  </p></p></td>
    <td> <p valign="middle"> <p align="center"> 35.5 K </p></p></td>
    <td> <p valign="middle"> <p align="center"> 13.1 K </p></p></td>
    <td> <p valign="middle"> <p align="center"> 61.4 K </p></p></td>
  </tr>
</table>



<!-- 
<br/><br/>

# 02 - Benchmark Results
* Evaluation metric: Recall@k for IoU=m ([link](https://medium.com/qloo/popular-evaluation-metrics-in-recommender-systems-explained-324ff2fb427d)).

* NOTE: For Activitynet-Captions, val1 / val2 or a combination of the two splits is used for evaluation. The most common choice is to use val1 as a validation set and val2 as a testing set. This is necessary as the official test set is withheld for competitions purposes. 

### Methods can be classified in:
* FS: Fully supervised
* WS: Weakly supervised
* RL: Reinforcement Learning

### Format
```markdown
* `Model` [ID](link) | `Features` |  R@k IoU=m |...| R@k IoU=m | Method |
```

Hit the paper `ID` to fast-forward to the paper details (link to pdf, venue, year, author and link to GitHub repo).

<br/>

### ActivityNet Captions (val 1)

| Models&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Features &nbsp;&nbsp;&nbsp;| R@1<br/>IoU0.3 | R@1<br/>IoU0.5 | R@1<br/>IoU0.7 | R@5<br/>IoU0.3 | R@5<br/>IoU0.5| R@5<br/>IoU0.7| Method |
| :---                       |:---:| :---: | :---: | :---: | :---: | :---: | :---: | :---:  | 
| ACRN          [[12]](#2018)| C3D | 31.29 | 16.17 |   -   |   -   |   -   |   -   | FS
| A2C           [[19]](#2019)| C3D |   -   | 36.90 |   -   |   -   |   -   |   -   | RL
| DEBUG         [[27]](#2019)| C3D | 55.91 | 39.72 |   -   |   -   |   -   |   -   | FS
| ExCL          [[28]](#2019)| I3D | 63.00 | 43.60 | 23.60 |   -   |   -   |   -   | FS
| TSP-PRL       [[37]](#2020)| C3D | 56.08 | 38.76 |   -   |   -   |   -   |   -   | RL
| GDP           [[40]](#2020)| C3D | 56.17 | 39.27 |   -   |   -   |   -   |   -   | FS
| DRN           [[41]](#2020)| C3D |   -   | 42.49 | 22.25 |   -   | 71.85 | 45.96 | FS
| VSLNet        [[48]](#2020)| I3D | 63.16 | 43.22 | 26.16 |   -   |   -   |   -   | FS

<br/>

### ActivityNet Captions (val 2)

| Models | Features | R@1<br/>IoU0.3 | R@1<br/>IoU0.5 | R@1<br/>IoU0.7 | R@5<br/>IoU0.3 | R@5<br/>IoU0.5| R@5<br/>IoU0.7| Method |
| :---                       |:---:| :---: | :---: | :---: | :---: | :---: | :---: | :---:  | 
| CTRL          [[6]](#2017)  | C3D | 47.43 | 29.01 |   -   | 75.32 | 59.17 |   -   | FS 
| TGN [[10]](#2018) | C3D<br/>VGG16<br/>Inception-V4 | 43.81<br/>42.24<br/>45.51 | 27.93<br/>23.90<br/>28.47 | 11.86<br/>-<br/>- | 54.56<br/>51.82<br/>57.32 | 44.20<br/> 40.17<br/>43.33 | 24.84<br/>-<br/>- | FS
| QSPN          [[17]](#2019) | C3D | 52.12 | 33.26 |   -   | 77.72 | 62.39 |   -   | FS
| WSDEC-W       [[26]](#2019) |     |  62.7 | 42.00 | 23.3  |   -   |   -   |   -   | WS
| WSLLN         [[26]](#2019) |     |  75.4 | 42.80 | 22.7  |   -   |   -   |   -   | WS 
| CMIN          [[29]](#2019) | C3D | 64.41 | 44.62 | 24.48 | 82.39 | 69.66 | 52.96 | FS
| 2D-TAN (pool) [[38]](#2020) | C3D | 59.45 | 44.51 | 26.54 | 85.53 | 77.13 | 61.96 | FS
| 2D-TAN (conv) [[38]](#2020) | C3D | 58.75 | 44.05 | 27.38 | 85.65 | 76.65 | 62.26 | FS
| SCN           [[39]](#2020) | C3D | 47.23 | 29.22 |   -   | 71.45 | 55.69 |   -   | WS
| DRN           [[41]](#2020) | C3D |   -   | 45.45 | 24.36 |   -   | 77.97 | 50.30 | FS
| HVTG          [[45]](#2020) | OBJ | 57.60 | 40.15 | 18.27 |   -   |   -   |   -   | FS
| PMI           [[46]](#2020) | C3D | 59.69 | 38.28 | 17.83 |   -   |   -   |   -   | FS
| DPIN          [[54]](#2020) | C3D | 62.40 | 47.27 | 28.31 | 87.52 | 77.45 | 60.03 | FS
| FIAN          [[55]](#2020) | C3D | 64.10 | 47.90 | 29.81 | 87.59 | 77.64 | 59.66 | FS
| CSMGAN        [[56]](#2020) | C3D | 68.52 | 49.11 | 29.15 | 87.68 | 77.43 | 59.63 | FS
| SMRN          [[58]](#2020) | C3D |   -   | 42.97 | 26.79 |   -   | 76.46 | 60.51 | FS
| VLG-Net       [[67]](#2021) | C3D |   -   | 46.32 | 29.82 |   -   | 77.15 | 63.33 | FS

<br/>

### ActivityNet Captions (val 1 + val2)

| Models&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Features &nbsp;&nbsp;&nbsp;| R@1<br/>IoU0.3 | R@1<br/>IoU0.5 | R@1<br/>IoU0.7 | R@5<br/>IoU0.3 | R@5<br/>IoU0.5| R@5<br/>IoU0.7| Method |
| :---                       |:---:| :---: | :---: | :---: | :---: | :---: | :---: | :---:  | 
| QSPN          [[17]](#2019)| C3D | 45.30 | 27.70 | 13.60 | 75.70 | 59.20 | 38.30 | FS  
| ABLR          [[20]](#2019)| C3D | 55.67 | 36.79 |   -   |   -   |   -   |   -   | RL
| SCDM          [[25]](#2019)| C3D | 54.80 | 36.75 | 19.86 | 77.29 | 64.99 | 41.53 | FS
| CBP           [[36]](#2020)| C3D | 54.30 | 35.76 | 17.80 | 77.63 | 65.89 | 46.20 | FS
| LGI           [[43]](#2020)| C3D | 58.52 | 41.51 | 23.07 |   -   |   -   |   -   | FS
| TripNet       [[47]](#2020)| C3D | 48.42 | 32.19 | 13.93 |   -   |   -   |   -   | RL
| TMLGA         [[49]](#2020)| I3D | 51.28 | 33.04 | 19.26 |   -   |   -   |   -   | FS
  
<br/>

### TACoS (test)

| Models&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Features | R@1<br/>IoU0.1 | R@1<br/>IoU0.3 | R@1<br/>IoU0.5 | R@1<br/>IoU0.7 | R@5<br/>IoU0.1 | R@5<br/>IoU0.3 | R@5<br/>IoU0.5| R@5<br/>IoU0.7| Method |
| :---                       |  :---:  | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | 
| CTRL          [[6]](#2017) |   C3D   | 24.32 | 18.32 | 13.30 |   -   | 48.73 | 36.69 | 25.42 |   -   | FS
| TGN           [[10]](#2018)|   C3D   | 41.87 | 21.77 | 18.90 | 11.88 | 53.40 | 39.06 | 31.02 | 15.26 | FS
| ACRN          [[12]](#2018)|   C3D   | 24.22 | 19.52 | 14.62 |   -   | 47.42 | 34.97 | 24.88 |   -   | FS
| MCF           [[13]](#2019)|   C3D   | 25.84 | 18.64 | 12.53 |   -   | 52.96 | 37.13 | 24.73 |   -   | FS
| ROLE          [[14]](#2018)|   C3D   | 20.37 | 15.38 |  9.94 |   -   | 45.45 | 31.17 | 20.13 |   -   | FS
| VAL           [[15]](#2018)|   C3D   | 25.74 | 19.76 | 14.74 |   -   | 51.87 | 38.55 | 26.52 |   -   | FS
| QSPN          [[17]](#2019)|   C3D   | 25.31 | 20.15 | 15.23 |   -   | 53.21 | 36.72 | 25.30 |   -   | FS
| ABLR          [[20]](#2019)|   C3D   | 34.70 | 19.50 |  9.40 |   -   |   -   |   -   |   -   |   -   | FS
| SAP           [[21]](#2019)|  VGG16  | 31.15 |   -   | 18.24 |   -   | 53.51 |   -   | 28.11 |   -   | FS
| SMRL          [[24]](#2019)|  VGG16  | 26.51 | 20.25 | 15.95 |   -   | 50.01 | 38.47 | 27.84 |   -   | RL
| SCDM          [[25]](#2019)|   C3D   |   -   | 26.11 | 21.17 |   -   |   -   | 40.16 | 32.18 |   -   | FS
| DEBUG         [[27]](#2019)|   C3D   | 41.15 | 23.45 | 11.72 |   -   |   -   |   -   |   -   |   -   | FS
| ExCL          [[28]](#2019)|   I3D   |   -   | 45.50 | 28.00 | 13.80 |   -   |   -   |   -   |   -   | FS
| CMIN          [[29]](#2019)| C3D<br/>I3D | 36.88<br/>41.73 | 27.33<br/>32.35  | 19.57<br/>22.54  |-<br/>- | 64.93<br/>69.15 | 43.35<br/>50.75 | 28.53<br/>32.11 | -<br/>- | FS
| SLTA     [[31]](#2019)|C3D +<br/>FRCNN| 23.13 | 17.07 | 11.92 |   -   | 46.52 | 32.90 | 20.86 |   -   | FS
| ACL-K         [[32]](#2019)|   C3D    | 31.64 | 24.17 | 20.01 |   -   | 57.85 | 42.15 | 30.66 |   -   | FS
| CBP           [[36]](#2020)|   C3D    |   -   | 27.31 | 24.79 | 19.10 |   -   | 43.64 | 37.40 | 25.59 | FS
| 2D-TAN (Pool) [[38]](#2020)|   C3D    | 47.59 | 37.29 | 25.32 |   -   | 70.31 | 57.81 | 45.04 |   -   | FS
| 2D-TAN convl) [[38]](#2020)|   C3D    | 46.44 | 35.22 | 25.19 |   -   | 74.43 | 56.94 | 44.21 |   -   | FS
| GDP           [[40]](#2020)|   C3D    | 39.68 | 24.14 | 13.50 |   -   |   -   |   -   |   -   |   -   | FS
| DRN           [[41]](#2020)|   C3D    |   -   |   -   | 23.17 |   -   |   -   |   -   | 33.36 |   -   | FS
| TripNet       [[47]](#2020)|   C3D    |   -   | 23.95 | 19.17 | 9.52  |   -   |   -   |   -   |   -   | RL
| VSLNet        [[48]](#2020)|   I3D    | 29.61 | 24.27 | 20.03 |   -   |   -   |   -   |   -   |   -   | FS
| TMLGA         [[49]](#2020)|   I3D    |   -   | 24.54 | 21.65 | 16.46 |   -   |   -   |   -   |   -   | FS
| DPIN          [[54]](#2020)|   C3D    | 59.04 | 46.74 | 32.92 |   -   | 75.78 | 62.16 | 50.26 |   -   | FS 
| FIAN          [[55]](#2020)|   C3D    | 39.55 | 33.87 | 28.58 |   -   | 56.14 | 47.76 | 39.16 |   -   | FS 
| CSMGAN        [[56]](#2020)|   C3D    | 42.74 | 33.90 | 27.09 |   -   | 68.97 | 53.98 | 41.22 |   -   | FS 
| SMRN          [[58]](#2020)|   C3D    | 50.44 | 42.49 | 32.07 |   -   | 77.28 | 66.63 | 52.84 |   -   | FS
| LGN           [[64]](#2020)|   C3D    | 52.46 | 41.71 | 30.57 |   -   | 76.86 | 63.06 | 50.76 |   -   | FS
| VLG-Net       [[67]](#2021)|   C3D    | 57.21 | 45.46 | 34.19 |   -   | 81.80 | 70.38 | 56.56 |   -   | FS 

<br/>

### DiDeMo (test)

| Models &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Features | R@1<br/>IoU0.5 | R@1<br/>IoU0.7 | R@1<br/>IoU1.0 | R@5<br/>IoU0.5 | R@5<br/>IoU0.7 | R@5<br/>IoU1.0 | Method |
| :---                       |  :---:      | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| MCN           [[5]](#2017) | VGG16<br/>Flow<br/>VGG16+Flow<br/>VGG16+Flow+TEF     |   -<br/>-<br/>-<br/>-   | -<br/>-<br/>-<br/>- | 13.10<br/>18.35<br/>19.88<br/>28.10  |   -<br/>-<br/>-<br/>-   | -<br/>-<br/>-<br/>- | 44.82<br/>56.25<br/>62.39<br/>78.21 |  FS
| TMN           [[9]](#2018) | VGG16<br/>Flow<br/>VGG16+Flow|   -<br/>-<br/>   | -<br/>-<br/>- | 18.71<br/>19.90<br/>22.92  | -<br/>-<br/>- | -<br/>-<br/>- | 72.97<br/>75.14<br/>76.08 | FS
| TGN           [[10]](#2018)| VGG16<br/>Flow<br/>VGG16+Flow|   -<br/>-<br/>   | -<br/>-<br/>- | 24.28<br/>27.52<br/>28.23  | -<br/>-<br/>- | -<br/>-<br/>- | 71.43<br/>76.94<br/>79.26 | FS
| ACRN          [[12]](#2018)|    VGG16    | 27.44 | 16.65 |   -   | 69.43 | 29.45 |   -   | FS
| ROLE          [[14]](#2018)|    VGG16    | 29.40 | 15.68 |   -   | 70.72 | 33.08 |   -   | FS
| MAN           [[22]](#2019)|     TAN     |   -   |   -   | 27.02 |   -   |   -   | 81.70 | FS
| TGA           [[23]](#2019)| VGG16+Flow  |   -   |   -   | 12.19 |   -   |   -   | 39.74 | WS
| SMRL          [[24]](#2019)| VGG16+FRCNN |   -   |   -   | 31.06 |   -   |   -   | 80.45 | RL
| WSLLN         [[26]](#2019)| VGG16<br/>Flow|-<br/>-|-<br/>-| 19.40<br/>18.40  |-<br/>-|-<br/>-| 53.10<br/>54.40 | WS
| SLTA          [[31]](#2019)| VGG16+FRCNN | 30.92 | 17.16 |   -   | 70.18 | 33.87 |   -   | FS
|VLANet         [[44]](#2020)|    VGG16    |   -   |   -   | 19.32 |   -   |   -   | 65.68 | WS
| RTBPN         [[51]](#2020)| VGG16<br/>Flow<br/>VGG16+Flow|   -<br/>-<br/>   | -<br/>-<br/>- | 20.38<br/>20.52<br/>20.79  | -<br/>-<br/>- | -<br/>-<br/>- | 55.88<br/>57.72<br/>60.26 | WS 
| VLG-Net       [[67]](#2021)|    VGG16    | 33.35 | 25.57 | 25.57 | 88.86 | 71.72 | 71.65 | FS
| LoGAN         [[69]](#2020)|  VGG16+Flow |   -   |    -  | 39.20 |   -   |   -   | 64.04 | WS 
 
<br/>

### Charades-STA (test)

| Models        | Features   | R@1<br/>IoU0.3 | R@1<br/>IoU0.5 | R@1<br/>IoU0.7 | R@5<br/>IoU0.3 | R@5<br/>IoU0.5 | R@5<br/>IoU0.7 | Method |
| :---                       |     :---:    | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| CTRL          [[6]](#2017) |      C3D     |   -   | 23.63 | 8.89  |   -   | 58.92 | 29.52 | FS
| ACRN          [[12]](#2018)|      C3D     |   -   | 20.26 | 7.64  |   -   | 71.99 | 27.79 | FS
| ROLE          [[14]](#2018)|      C3D     |   -   | 21.74 | 7.82  |   -   | 70.37 | 30.06 | FS
| VAL           [[15]](#2018)|      C3D     |   -   | 23.12 | 9.16  |   -   | 61.26 | 27.98 | FS
| ASST          [[16]](#2018)|      C3D     |   -   | 42.72 | 24.06 |   -   | 71.32 | 43.98 | FS
| QSPN          [[17]](#2019)|      C3D     | 54.70 | 35.60 | 15.80 | 95.80 | 79.40 | 45.40 | FS
| ABLR          [[20]](#2019)|      C3D     |   -   | 24.36 | 9.01  |   -   |   -   |   -   | FS
| SAP           [[21]](#2019)|     VGG16    |   -   | 27.42 | 13.36 |   -   | 66.37 | 38.15 | FS
| MAN           [[22]](#2019)|VGG16<br/>I3D | -<br/>- | 41.24<br/>46.53 | 20.54<br/>22.72 | -<br/>- | 83.21<br/>86.23 | 51.85<br/>53.72 | FS
| TGA           [[23]](#2019)|      ---     | 32.14 | 19.94 | 8.84  | 56.58 | 65.52 | 33.51 | WS |
| SMRL          [[24]](#2019)|     VGG16    |   -   | 24.36 | 11.17 |   -   | 61.25 | 32.08 | RL
| SCDM          [[25]](#2019)|      I3D     |   -   | 54.44 | 33.43 |   -   | 74.43 | 58.08 | FS
| DEBUG         [[27]](#2019)|      C3D     |   -   | 37.39 | 17.69 |   -   |   -   |   -   | FS
| ExCL          [[28]](#2019)|      I3D     | 65.10 | 44.10 | 22.40 |   -   |   -   |   -   | FS
| SLTA          [[31]](#2019)|   C3D+FRCNN  |   -   | 22.81 |  8.25 |   -   | 72.39 | 31.46 | FS
| ACL           [[32]](#2019)|      C3D     |   -   | 26.47 | 11.23 |   -   | 61.51 | 33.23 | FS
| ACL-K         [[32]](#2019)|      C3D     |   -   | 30.48 | 12.20 |   -   | 64.84 | 35.13 | FS
| CBP           [[36]](#2020)|      C3D     |   -   | 36.80 | 18.87 |   -   | 70.94 | 50.19 | FS
| TSP-PRL       [[37]](#2020)|      C3D     |   -   | 37.39 | 17.69 |   -   |   -   |   -   | RL
| TSP-PRL       [[37]](#2020)|  Two Streams |   -   | 45.30 | 24.73 |   -   |   -   |   -   | RL
| 2D-TAN (pool) [[38]](#2020)|     VGG16    |   -   | 39.70 | 23.31 |   -   | 80.32 | 51.26 | FS
| 2D-TAN (conv) [[38]](#2020)|     VGG16    |   -   | 39.81 | 23.25 |   -   | 79.33 | 52.15 | FS
| SCN           [[39]](#2020)|      C3D     | 42.96 |  23.58 | 9.97 | 95.56 | 71.80 | 38.87 | WS
| GDP           [[40]](#2020)|      C3D     |   -   | 39.47 | 18.49 |   -   |   -   |   -   | FS
| DRN           [[41]](#2020)| VGG16<br/>C3D<br/>I3D    |   -<br/>-<br/>-   | 42.90<br/>45.40<br/>53.09 | 23.68<br/>26.40<br/>31.75 |   -<br/>-<br/>-   | 87.80<br/>88.01<br/>89.06 | 54.87<br/>55.38<br/>60.05 | FS
| LGI           [[43]](#2020)|      I3D     |   -   | 59.46 | 35.48 |   -   |   -   |   -   | FS
| VLANet        [[44]](#2020)|      C3D     |   -   |  31.83 | 14.17 |   -   | 82.85 | 33.09 | WS
| HVTG          [[45]](#2020)|     FRCNN    |   -   | 47.27 | 23.30 |   -   |   -   |   -   | FS
| PMI           [[46]](#2020)|      C3D     |   -   | 39.73 | 19.27 |   -   |   -   |   -   | FS
| TripNet       [[47]](#2020)|      C3D     | 51.33 | 38.29 | 16.07 |   -   |   -   |   -   | RL
| VSLNet        [[48]](#2020)|      I3D     |   -   | 54.19 | 35.22 |   -   |   -   |   -   | FS
| TMLGA         [[49]](#2020)|      I3D     | 67.53 | 52.02 | 33.74 |   -   |   -   |   -   | FS
| RTBPN         [[51]](#2020)|      C3D     | 60.04 | 32.36 | 13.24 | 97.48 | 71.85 | 41.18 | WS
| DPIN          [[54]](#2020)|     VGG16    |   -   | 47.98 | 26.96 |   -   | 85.53 | 55.00 | FS
| FIAN          [[55]](#2020)|      I3D     |   -   | 58.55 | 37.72 |   -   | 87.80 | 63.52 | FS
| WSTG          [[61]](#2020)|      ---     | 39.80 | 27.30 | 12.90 |   -   |   -   |   -   | WS
| LGN           [[64]](#2020)|     VGG16    |   -   | 48.15 | 26.67 |   -   | 86.80 | 53.01 | FS
| LoGAN         [[69]](#2020)|      C3D     |   -   |  34.68 | 14.54 |   -   | 74.30 | 39.11 | WS
| AVMR          [[53]](#2020)|    ResNet    | 77.72 | 54.59 |   -   | 88.92 | 72.78 |   -   | WS -->

<br/><br/>

# 02 - Papers
Markdown format:

```markdown
* `ID` | `Model Acronym` | `Conference` | [Paper Name](link) | Author 1 et al |  [GitHub](link)
```

<br/>

## 2022

|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|1| `TubeDETR` | `CVPR`| [TubeDETR: Spatio-Temporal Video Grounding with Transformers](https://arxiv.org/abs/2203.16434) | Yang et al | [GitHub](https://github.com/antoyang/TubeDETR)
|2| `STCAT` | `NeurIPS`| [Embracing Consistency: A One-Stage Approach for Spatio-Temporal Video Grounding](https://arxiv.org/pdf/2209.13306.pdf) | Jin et al | 
|3| `--` | `ArXiv`| [GAUSSIAN KERNEL-BASED CROSS MODAL NETWORK FOR SPATIO-TEMPORAL VIDEO GROUNDING](https://arxiv.org/pdf/2207.00744.pdf) | Xiong et al | 



## 2021

|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|4| `STVBert` | `ICCV`| [STVGBert: A Visual-linguistic Transformer based Framework for Spatio-temporal Video Grounding](https://openaccess.thecvf.com/content/ICCV2021/papers/Yang_SAT_2D_Semantics_Assisted_Training_for_3D_Visual_Grounding_ICCV_2021_paper.pdf) | Su et al | 


## 2020

|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|5| `Where Does It Exist` | `CVPR`| [Where Does It Exist: Spatio-Temporal Video Grounding for Multi-Form Sentences](https://arxiv.org/abs/2001.06891) | Zhang et al | [GitHub](https://github.com/Guaranteer/VidSTG-Dataset)
|6| `--` | `IEEE TCSVT`| [Human-centric Spatio-Temporal Video Grounding With Visual Transformers](https://arxiv.org/abs/2201.02848) | Tang et al | [GitHub](https://github.com/tzhhhh123/HC-STVG)
|7| `--` | `IJCAI`| [Object-Aware Multi-Branch Relation Networks for Spatio-Temporal Video Grounding](https://www.ijcai.org/proceedings/2020/0149.pdf) | Zhang et al |




<!-- ## Analysis and Surveys
|ID| Model | Venue | Title | Authors  | Code  |
| :---: | :---: | :--- | --- | ---------- | :---: |
|-  |`--`  | `BMVC 2020` | [Uncovering Hidden Challenges in Query-Based Video Moment Retrieval](https://arxiv.org/pdf/2009.00325.pdf) | Otani et al | 
|-  |`--`  | `AAAI 2022`  | [A Closer Look at Temporal Sentence Grounding in Videos: Datasets and Metrics](https://arxiv.org/pdf/2101.09028.pdf) | Yuan et al | [GitHub](https://github.com/yytzsy/grounding_changing_distribution)
|-  |`--`  | `ArXiv 2021` | [A Survey on Temporal Sentence Grounding in Videos](https://arxiv.org/pdf/2109.08039.pdf) | LAN et al | 
|-  |`--`  | `ArXiv 2022` | [he Elements of Temporal Sentence Grounding in Videos: A Survey and Future Directions](https://arxiv.org/pdf/2201.08071.pdf) | Zhang et al | 
|-| `--` | `Arxiv`| [A Survey on Natural Language Video Localization](https://arxiv.org/abs/2104.00234) | Liu et al |


<br/>

## Early works
|ID| Model | Venue | Title | Authors  | Code  |
| :---: | :---: | :--- | --- | ---------- | :---: |
|1|`--`  | `ACL 2013`    | [Grounded Language Learning from Video Described with Sentences](https://www.aclweb.org/anthology/P13-1006/) |  Yu et al
|2|`--`  | `CVPR 2014`   | [Visual Semantic Search: Retrieving Videos via Complex Textual Queries](<https://www.cv-foundation.org/openaccess/content_cvpr_2014/papers/Lin_Visual_Semantic_Search_2014_CVPR_paper.pdf>) |  Lin et al
|3|`--`  | `AAAI 2015`   |  [Jointly Modeling Deep Video and Compositional Text to Bridge Vision and Language in a Unified Framework](https://www.aaai.org/ocs/index.php/AAAI/AAAI15/paper/view/9734) | Xu et al
|4|`--`  |  `IJCAI 2016` | [Unsupervised Alignment of Actions in Video with Text Descriptions](https://pdfs.semanticscholar.org/5893/7d427ff36e1470b18120245148355047e4ea.pdf) |  Song et al
 
 <br/>

## 2017

|ID| Model | Venue | Title | Authors  | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|5| `MCN`   | `ICCV`  | [Localizing Moments in Video with Natural Language](https://arxiv.org/abs/1708.01641)  | Hendricks et al | [GitHub](https://github.com/LisaAnne/LocalizingMoments)|
|6| `CTRL`  | `ICCV`  | [TALL: Temporal Activity Localization via Language Query](https://arxiv.org/abs/1705.02101)  | Gao et al | [GitHub](<https://github.com/jiyanggao/TALL>)  |
|7| `--`    | `ArXiv` | [Where to Play: Retrieval of Video Segments using Natural-Language Queries](<https://arxiv.org/abs/1707.00251>) | Lee et al | 

<br/>

## 2018

|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|8|`FIFO` | `ECCV`   | [Find and Focus: Retrieve and Localize Video Events with Natural Language Queries](<http://openaccess.thecvf.com/content_ECCV_2018/papers/Dian_SHAO_Find_and_Focus_ECCV_2018_paper.pdf>) | Shao et al | | 
|9|`TMN`  | `ECCV`   | [Temporal Modular Networks for Retrieving Complex Compositional Activities in Videos](<http://svl.stanford.edu/assets/papers/liu2018eccv.pdf>)  | Liu et al | |
|10|`TGN`  | `EMNLP`  | [Temporally Grounding Natural Sentence in Video](<https://aclweb.org/anthology/papers/D/D18/D18-1015/>)  | Chen et al | [GitHub](https://github.com/JaywongWang/TGN)
|11|`TEMPO`| `EMNLP`  | [Localizing Moments in Video with Temporal Language](<https://arxiv.org/abs/1809.01337>)                 | Hendricks et al | [GitHub](https://github.com/LisaAnne/TemporalLanguageRelease)
|12|`ACRN` | `SIGIR`  | [Attentive Moment Retrieval in Videos](http://staff.ustc.edu.cn/~hexn/papers/sigir18-video-retrieval.pdf)| Liu et al | [GitHub](https://sigir2018.wixsite.com/acrn)
|13|`MCF`  | `IJCAI`  | [Multi-modal Circulant Fusion for Video-to-Language and Backward](https://pdfs.semanticscholar.org/e2e5/cef45c60c52fb0d0415cca6cbf35beab3873.pdf) | Wu et al | [GitHub](<https://github.com/AmingWu/Multi-modal-Circulant-Fusion/>)
|14|`ROLE` | `ACM MM` | [Cross-modal Moment Localization in Videos](https://liqiangnie.github.io/paper/p843-liu.pdf)             |  Liu et al |  [GitHub](https://acmmm18.wixsite.com/role)
|15|`VAL`  | `PRCM`   | [VAL: Visual-attention action localizer](https://link.springer.com/content/pdf/10.1007%2F978-3-030-00767-6_32.pdf) | Song et al 
|16|`ASST` | `ArXiv`  | [Attentive Sequence to Sequence Translation for Localizing Clips of Interest by Natural Language Descriptions](https://arxiv.org/pdf/1808.08803.pdf) | Ning et al 

<br/>

## 2019
|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|17|`QSPN`| `AAAI` | [Multilevel Language and Vision Integration for Text-to-Clip Retrieval](<https://arxiv.org/abs/1804.05113>)| Xu et al | [GitHub](<https://github.com/VisionLearningGroup/Text-to-Clip_Retrieval>)
|18|`LNet`| `AAAI` | [Localizing Natural Language in Videos ](https://www.aaai.org/ojs/index.php/AAAI/article/view/4827/4700)| Chen et al
|19|`A2C` | `AAAI` | [Read, Watch, and Move: Reinforcement Learning for Temporally Grounding Natural Language Descriptions in Videos](https://arxiv.org/abs/1901.06829)| Dongliang et al | [GitHub](https://github.com/WuJie1010/Temporally-language-grounding)
|20|`ABLR`| `AAAI` | [To Find Where You Talk: Temporal Sentence Localization in Video with Attention Based Location Regression](http://arxiv.org/abs/1804.07014)| Yuan et al | [GitHub](https://github.com/yytzsy/ABLR_GitHub)
|21|`SAP` | `AAAI` | [Semantic Proposal for Activity Localization in Videos via Sentence Query](http://yugangjiang.info/publication/19AAAI-actionlocalization.pdf)| Chen et al
|22|`MAN`| `CVPR` | [MAN: Moment Alignment Network for Natural Language Moment Retrieval via Iterative Graph Adjustment](https://arxiv.org/abs/1812.00087)| Zhang et al | [GitHub](https://github.com/dazhang-cv/MAN)
|23|`TGA`| `CVPR` | [Weakly Supervised Video Moment Retrieval From Text Queries](<https://arxiv.org/abs/1904.03282>)| Mithun et al | [GitHub](https://github.com/niluthpol/weak_supervised_video_moment)
|24|`SMRL`| `CVPR` | [Language-Driven Temporal Activity Localization_ A Semantic Matching Reinforcement Learning Model](<http://openaccess.thecvf.com/content_CVPR_2019/papers/Wang_Language-Driven_Temporal_Activity_Localization_A_Semantic_Matching_Reinforcement_Learning_Model_CVPR_2019_paper.pdf>)|  Wang et al 
|25|`SCDM`| `NIPS` | [Semantic Conditioned Dynamic Modulation for Temporal Sentence Grounding in Videos](https://arxiv.org/pdf/1910.14303.pdf)| Yuan et al | [GitHub](https://github.com/yytzsy/SCDM)
|26|`WSLLN`| `EMNLP` | [WSLLN: Weakly Supervised Natural Language Localization Networks](https://arxiv.org/abs/1909.00239)| Gao et al 
|27|`DEBUG`| `EMNLP` | [DEBUG: A Dense Bottom-Up Grounding Approach for Natural Language Video Localization](https://www.aclweb.org/anthology/D19-1518.pdf)| Lu et al
|28|`ExCL`| `NAACL` | [ExCL: Extractive Clip Localization Using Natural Language Descriptions](https://arxiv.org/abs/1904.02755)| Ghosh et al
|29|`CMIN`| `SIGIR` | [Cross-Modal Interaction Networks for Query-Based Moment Retrieval in Videos](https://arxiv.org/abs/1906.02497)| Zhang et al |  [GitHub](https://github.com/ikuinen/CMIN_moment_retrieval)
|30|`CMIN`| `IEEE` | [Moment Retrieval via Cross-Modal Interaction Networks With Query Reconstruction](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8962274&tag=1)| Zhang et al | [GitHub](https://github.com/ikuinen/CMIN_moment_retrieval)
|31|`SLTA`| `ICMR` | [Cross-Modal Video Moment Retrieval with Spatial and Language-Temporal Attention](https://dl.acm.org/citation.cfm?id=3325019)| Jiang et al | [GitHub](https://github.com/BonnieHuangxin/SLTA)
|32|`ACL`| `WACV` | [MAC: Mining Activity Concepts for Language-based Temporal Localization](https://arxiv.org/abs/1811.08925)| Ge et al | [GitHub](https://github.com/runzhouge/MAC)
|33|`WSSTG`| `ACL` | [Weakly-Supervised Spatio-Temporally Grounding Natural Sentence in Video](https://www.aclweb.org/anthology/P19-1183.pdf)| Chen et al | [GitHub](https://github.com/zfchenUnique/WSSTG)
|34|`TCMN`| `ACM` | [Exploiting Temporal Relationships in Video Moment Localization with Natural Language](https://arxiv.org/pdf/1908.03846.pdf)| Zhang et al | [GitHub](https://github.com/Sy-Zhang/TCMN-Release)
|35|`CAL`| `ArXiv` | [Temporal Localization of Moments in Video Collections with Natural Language](https://arxiv.org/abs/1907.12763v1)| Escorcia et al| [GitHub](https://github.com/escorciav/moments-retrieval-page)

 <br/>

## 2020
|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|36|`CBP`    | `AAAI` | [Temporally Grounding Language Queries in Videos by Contextual Boundary-aware Prediction](https://arxiv.org/pdf/1909.05010.pdf) | Wang et al | [GitHub](https://github.com/JaywongWang/CBP)
|37|`TSP-PRL`| `AAAI` | [Tree-Structured Policy based Progressive Reinforcement Learning for Temporally Language Grounding in Video](https://arxiv.org/pdf/238.06680.pdf)| Wu et al| [GitHub](https://github.com/WuJie1010/TSP-PRL)
|38|`2DTAN`  | `AAAI` | [Learning 2D Temporal Localization Networks for Moment Localization with Natural Language](https://arxiv.org/abs/1912.03590) | Zhang et al | [GitHub1](https://github.com/microsoft/2D-TAN), [GitHub2](https://github.com/ChenJoya/2dtan)
|39|`SCN`    | `AAAI` | [Weakly-Supervised Video Moment Retrieval via Semantic Completion Network](https://arxiv.org/pdf/1911.08199.pdf) | Lin et al | | 
|40|`GDP`    | `AAAI` | [Rethinking the Bottom-Up Framework for Query-based Video Localization](https://zjuchenlong.github.io/papers/AAAI_2020.pdf) |  Chen et al | 
|41|`DRN`    | `CVPR` | [Dense Regression Network for Video Grounding](http://openaccess.thecvf.com/content_CVPR_2020/papers/Zeng_Dense_Regression_Network_for_Video_Grounding_CVPR_2020_paper.pdf) | Zeng et al | [GitHub](https://github.com/Alvin-Zeng/DRN)
|42|`STGRN`  | `CVPR` | [Where Does It Exist: Spatio-Temporal Video Grounding for Multi-Form Sentences](http://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_Where_Does_It_Exist_Spatio-Temporal_Video_Grounding_for_Multi-Form_Sentences_CVPR_2020_paper.pdf) | Zhang et al | [GitHub](https://github.com/Guaranteer/VidSTG-Dataset)
|43|`LGI`    | `CVPR` | [Local-Global Video-Text Interactions for Temporal Grounding](http://openaccess.thecvf.com/content_CVPR_2020/papers/Mun_Local-Global_Video-Text_Interactions_for_Temporal_Grounding_CVPR_2020_paper.pdf) |  Mun et al | [GitHub](https://github.com/JonghwanMun/LGI4temporalgrounding)
|44|`VLANet` | `ECCV` | [VLANet: Video-Language Alignment Network for Weakly-Supervised Video Moment Retrieval](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123730154.pdf) | Ma et al | 
|45|`HVTG`   | `ECCV` | [Hierarchical Visual-Textual Graph for Temporal Activity Localization via Language](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123650596.pdf) | Chen et al | [GitHub](https://github.com/forwchen/HVTG)
|46|`PMI`    | `ECCV` | [Learning Modality Interaction for Temporal Sentence Localization and Event Captioning in Videos](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123490324.pdf) | Chen et al | 
|47|`TripNet`| `BMVC` | [Tripping through time Efficient Localization of Activities in Videos](https://arxiv.org/pdf/1904.09936.pdf) | Hahn et al | 
|48|`VSLNet` | `ACL`  | [Span-based Localizing Network for Natural Language Video Localization](https://arxiv.org/pdf/2004.13931.pdf) | Zhang et al  | [GitHub](https://github.com/IsaacChanghau/VSLNet)
|49|`TMLGA`  | `WACV` | [Proposal-free Temporal Moment Localization of a Natural-Language Query in Video using Guided Attention](http://openaccess.thecvf.com/content_WACV_2020/papers/Rodriguez_Proposal-free_Temporal_Moment_Localization_of_a_Natural-Language_Query_in_Video_WACV_2020_paper.pdf) |  Rodriguez-Opazo et al| [GitHub](https://github.com/crodriguezo/TMLGA)
|50|`--`     | `NIPS` | [Counterfactual Contrastive Learning for Weakly-Supervised Vision-Language Grounding](https://papers.nips.cc/paper/2020/file/d27b95cac4c27feb850aaa4070cc4675-Paper.pdf) |  Zhang et al | 
|51|`RTBPN`  | `ACM`  | [Regularized Two-Branch Proposal Networks for Weakly-Supervised Moment Retrieval in Videos](https://dl.acm.org/doi/pdf/10.1145/3394171.3413967) |  Zhang et al | 
|52|`STRONG` | `ACM`  | [STRONG: Spatio-Temporal Reinforcement Learning for Cross-Modal Video Moment Localization](http://data-science.ustc.edu.cn/_upload/article/files/c4/4f/10f4da284171a6275429698edccf/16741411-8b8b-405a-90a8-5c4baac1c620.pdf) | Cao et al | 
|53|`AVMR`   | `ACM`  | [Adversarial Video Moment Retrieval by Jointly Modeling Ranking and Localization](https://dl.acm.org/doi/pdf/10.1145/3394171.3413841) | Cao et al | 
|54|`DPIN`   | `ACM`  | [Dual Path Interaction Network for Video Moment Localization](https://dl.acm.org/doi/abs/10.1145/3394171.3413975) | Wang et al | 
|55|`FIAN`   | `ACM`  | [Fine-grained Iterative Attention Network for Temporal Language Localization in Videos](https://dl.acm.org/doi/abs/10.1145/3394171.3414053) | Qu et al | 
|56|`CSMGAN` | `ACM`  | [Jointly Cross- and Self-Modal Graph Attention Network for Query-Based Moment Localization](https://dl.acm.org/doi/abs/10.1145/3394171.3414026) | Liu et all|  [GitHub](https://github.com/liudaizong/CSMGAN)
|57|`--`      | `DAVU`  | [Cross-Modality Video Segment Retrieval with Ensemble Learning](https://link.springer.com/chapter/10.1007/978-3-030-30671-7_5#Sec12) | Yu et al | 
|58|`SMRN`    | `ISNN`  | [Semantic Modulation Based Residual Network for Temporal Language Queries Grounding in Video](https://link.springer.com/chapter/10.1007/978-3-030-64221-1_11) |Chen et al | 
|59|`--`    | `Journal`  | [Cross-modal video moment retrieval based on visual-textual relationship alignment](https://engine.scichina.com/publisher/scp/journal/SSI/50/6/10.1360/SSI-2019-0292?slug=fulltext) |  Chen et al| 
|60|`--`    | `ArXiv`  | [Video Moment Retrieval via Natural Language Queries](https://arxiv.org/abs/2009.02406) | Yu et al | 
|61|`WSTG`| `ArXiv`  | [Look Closer to Ground Better: Weakly-Supervised Temporal Grounding of Sentence in Video](https://arxiv.org/pdf/2001.09308.pdf) | Chen et al | 
|62|`MARN`| `ArXiv`  | [Weakly-Supervised Multi-Level Attentional Reconstruction Network for Grounding Textual Queries in Videos](https://arxiv.org/pdf/2003.07048.pdf) | Song et al | 
|63|`LGN` | `ArXiv`  | [Language Guided Networks for Cross-modal Moment Retrieval](https://arxiv.org/pdf/2006.10457.pdf) | Liu et al | 
|64|`ACRM`| `ArXiv`  | [Frame-wise Cross-modal Match for Video Moment Retrieval](https://arxiv.org/abs/2009.10434) | Tang et al | 
|65|`CMA` | `ArXiv`  | [A Simple Yet Effective Method for Video Temporal Grounding with Cross-Modality Attention](https://arxiv.org/pdf/2009.11232.pdf) |  Zhang et al| 
|66|`--`  | `ArXiv`  | [Natural Language Video Localization: A Revisit in Span-based Question Answering Framework](https://arxiv.org/pdf/2102.13558.pdf) | Zhang et al | 

<br/>

## 2021

|ID| Model | Venue | Title | Authors | Code  |
| :---: | :--- | :--- | --- | ---------- | :---: |
|67|`VLG-Net`| `ICCVW`  | [VLG-Net: Video-Language Graph Matching Network for Video Grounding](https://arxiv.org/pdf/2011.10132.pdf) | Soldan et al | [GitHub](https://github.com/Soldelli/VLG-Net)
|68|`LoGAN`| `WACV`  | [LoGAN: Latent Graph Co-Attention Network for Weakly-Supervised Video Moment Retrieval](https://openaccess.thecvf.com/content/WACV2021/papers/Tan_LoGAN_Latent_Graph_Co-Attention_Network_for_Weakly-Supervised_Video_Moment_Retrieval_WACV_2021_paper.pdf) | Tan et al | 
|69|`CBLN` | `CVPR` | [Context-aware Biaffine Localizing Network for Temporal Sentence Grounding](https://arxiv.org/pdf/2103.11555.pdf) | Liu et al | [GitHub](https://github.com/liudaizong/CBLN)
|70|`DeNet`| `CVPR` | [Embracing Uncertainty: Decoupling and De-bias for Robust Temporal Grounding](https://arxiv.org/pdf/2103.16848.pdf) | Zhou et al |
|70| `DORi` |`WACV`| [DORi: Discovering Object Relationships for Moment Localization of a Natural Language Query in a Video](https://openaccess.thecvf.com/content/WACV2021/papers/Rodriguez-Opazo_DORi_Discovering_Object_Relationships_for_Moment_Localization_of_a_Natural_WACV_2021_paper.pdf) |  Rodriguez-Opazo et al | [GitHub](https://github.com/crodriguezo/DORi.git)
|71| `PEARL ` | `WACV`| [Natural Language Video Moment Localization Through Query-Controlled Temporal Convolution](https://www.ecse.rpi.edu/~rjradke/papers/zhang-wacv22.pdf) |  Zhang et al |
|72| `IVG-DCL` | `CVPR`| [Interventional Video Grounding With Dual Contrastive Learning](https://openaccess.thecvf.com/content/CVPR2021/papers/Nan_Interventional_Video_Grounding_With_Dual_Contrastive_Learning_CVPR_2021_paper.pdf) |  Nan et al | [GitHub](https://github.com/nanguoshun/IVG)
|73| `SMIN` | `CVPR`| [Structured Multi-Level Interaction Network for Video Moment Localization via Language Query](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_Structured_Multi-Level_Interaction_Network_for_Video_Moment_Localization_via_Language_CVPR_2021_paper.pdf) |  Wang et al |
|74| `--` | `CVPR`| [Multi-Stage Aggregated Transformer Network for Temporal Language Localization in Videos](https://openaccess.thecvf.com/content/CVPR2021/papers/Zhang_Multi-Stage_Aggregated_Transformer_Network_for_Temporal_Language_Localization_in_Videos_CVPR_2021_paper.pdf) | Zhang et al |
|75| `MMRG` | `CVPR`| [Multi-Modal Relational Graph for Cross-Modal Video Moment Retrieval](https://openaccess.thecvf.com/content/CVPR2021/html/Zeng_Multi-Modal_Relational_Graph_for_Cross-Modal_Video_Moment_Retrieval_CVPR_2021_paper.html) |  Zeng et al |
|76| `CPN` | `CVPR`| [Cascaded Prediction Network via Segment Tree for Temporal Video Grounding](https://openaccess.thecvf.com/content/CVPR2021/html/Zhao_Cascaded_Prediction_Network_via_Segment_Tree_for_Temporal_Video_Grounding_CVPR_2021_paper.html) | Zhao et al |
|77| `CRM` | `CVPR`| [Cross-Sentence Temporal and Semantic Relations in Video Activity Localisation](https://openaccess.thecvf.com/content/ICCV2021/papers/Huang_Cross-Sentence_Temporal_and_Semantic_Relations_in_Video_Activity_Localisation_ICCV_2021_paper.pdf) | Huang et al |
|78| `FVMR` | `CVPR`| [Fast Video Moment Retrieval](https://openaccess.thecvf.com/content/ICCV2021/papers/Gao_Fast_Video_Moment_Retrieval_ICCV_2021_paper.pdf) | Gao et al |
|79| `RMN` | `ACL`| [Reasoning Step-by-Step: Temporal Sentence Localization in Videos via Deep Rectification-Modulation Network](https://aclanthology.org/2020.coling-main.167/) | Liu et al |
|80| `--` | `ACL`| [Fine-grained Semantic Alignment Network for Weakly Supervised Temporal Language Grounding](https://aclanthology.org/2021.findings-emnlp.9.pdf) | Wang et al |
|81| `VCA` | `ACM`| [Visual Co-Occurrence Alignment Learning for Weakly-Supervised Video Moment Retrieval](https://dl.acm.org/doi/pdf/10.1145/3474085.3475278) | Wang et al |
|82| `CI-MHA` | `ACM`| [Cross Interaction Network for Natural Language Guided Video Moment Retrieval](https://dl.acm.org/doi/10.1145/3404835.3463021) | Yu et al |
|83| `MABAN` | `Journal`| [MABAN: Multi-Agent Boundary-Aware Network for Natural Language Moment Retrieval](https://ieeexplore.ieee.org/abstract/document/9451629?casa_token=B2wdbvbslGMAAAAA:3c6oGK-klY3MFYSfIFbMr33gt1LMIwQL5tRW51lrWnLqJypiv42h6q2WPIitU_dptIAhr_lXWxfRKI8) | Yu et al |
|84| `CFSTRI` | `Journal`| [Coarse-to-Fine Spatial-Temporal Relationship Inference for Temporal Sentence Grounding](https://ieeexplore.ieee.org/abstract/document/9475486) | Qi et al |
|85| `--` | `Journal`| [Regularized Two Granularity Loss Function for Weakly Supervised Video Moment Retrieval](https://ieeexplore.ieee.org/abstract/document/9580967) | Teng et al |
|86| `ACRM` | `Journal`| [Frame-wise Cross-modal Matching for Video Moment Retrieval](https://ieeexplore.ieee.org/abstract/document/9374685) | Tang et al |
|87| `DCT-net` | `Journal`| [DCT-net: A deep co-interactive transformer network for video temporal grounding](https://www.sciencedirect.com/science/article/pii/S0262885621000883) | Qi et al |
|88| `SV-VMR` | `Journal`| [Diving Into The Relations: Leveraging Semantic and Visual Structures For Video Moment Retrieval](https://ieeexplore.ieee.org/abstract/document/9428369) | Wu et al |
|89| `CAN` | `Journal`| [Context-aware network with foreground recalibration for grounding natural language in video](https://link.springer.com/article/10.1007/s00521-021-05807-z) | Chen et al |
|90| `--` | `Journal`| [Multi-scale 2D Representation Learning for weakly-supervised moment retrieval](https://ieeexplore.ieee.org/abstract/document/9412712) | Li et al |
|91| `LCNet` | `Journal`| [Local Correspondence Network for Weakly Supervised Temporal Sentence Grounding](https://ieeexplore.ieee.org/abstract/document/9356448) | Yang et al |
|92| `CLEAR` | `Journal`| [Coarse-to-Fine Semantic Alignment for Cross-Modal Moment Localization](https://ieeexplore.ieee.org/abstract/document/9464749) | Hu et al |
|93| `VSLNet` | `Journal`| [Natural Language Video Localization: A Revisit in Span-based Question Answering Framework](https://ieeexplore.ieee.org/abstract/document/9361191) | Zhang et al |
|94| `VSRNet` | `Journal`| [VSRNet: End-to-end video segment retrieval with text query](https://www.sciencedirect.com/science/article/pii/S0031320321002144) | Sun et al |
|95| `MS-2D-TAN` | `Journal`| [Multi-Scale 2D Temporal Adjacency Networks for Moment Localization with Natural Language](https://ieeexplore.ieee.org/abstract/document/9580623) | Zhang et al | [GitHub](https://github.com/microsoft/2D-TAN/tree/ms-2d-tan)
|96| `U-VMR` | `Journal`| [Learning Video Moment Retrieval Without a Single Annotated Video](https://ieeexplore.ieee.org/abstract/document/9415694) | Gao et al |
|97| `CPNet` | `AAAI`| [Proposal-Free Video Grounding with Contextual Pyramid Network](https://www.aaai.org/AAAI21Papers/AAAI-9134.LiK.pdf) | Li et al |
|98| `DepNet` | `AAAI`| [Dense Events Grounding in Video](http://www.muyadong.com/paper/3254_PeijunB.pdf) | Bao et al |
|99| `BPNet` | `AAAI`| [Boundary Proposal Network for Two-Stage Natural Language Video Localization](https://www.aaai.org/AAAI21Papers/AAAI-6267.XiaoS.pdf) | Xiao et al | 
|100| `STVGBert` | `ICCV`| [STVGBert: A Visual-Linguistic Transformer Based Framework for Spatio-Temporal Video Grounding](https://openaccess.thecvf.com/content/ICCV2021/html/Su_STVGBert_A_Visual-Linguistic_Transformer_Based_Framework_for_Spatio-Temporal_Video_Grounding_ICCV_2021_paper.html) | Su et al |
|101| `BSP` | `ICCV`| [Boundary-sensitive Pre-training for Temporal Localization in Videos](https://openaccess.thecvf.com/content/ICCV2021/papers/Xu_Boundary-Sensitive_Pre-Training_for_Temporal_Localization_in_Videos_ICCV_2021_paper.pdf) | Xu et al | [GitHub](https://github.com/frostinassiky/bsp)
|102| `SSCS` | `ICCV`| [Support-Set Based Cross-Supervision for Video Grounding](https://openaccess.thecvf.com/content/ICCV2021/papers/Ding_Support-Set_Based_Cross-Supervision_for_Video_Grounding_ICCV_2021_paper.pdf) | Ding et al |
|103| `DCM` | `SIGIR`| [Deconfounded Video Moment Retrieval with Causal Intervention](https://arxiv.org/pdf/2106.01534.pdf) | Yang et al | [GitHub](https://github.com/Xun-Yang/Causal_Video_Moment_Retrieval)
|104| `--` | `Arxiv`| [Video Moment Retrieval with Text Query Considering Many-to-Many Correspondence Using Potentially Relevant Pair](https://arxiv.org/abs/2106.13566) |  Maeoki et al |
|105| `HDRR` | `Arxiv`| [Hierarchical Deep Residual Reasoning for Temporal Moment Localization](https://arxiv.org/pdf/2111.00417.pdf) |  Ma et al | [GitHub](https://github.com/ddlBoJack/HDRR)
|106| `RaNet` | `EMNLP`| [Relation-aware Video Reading Comprehension for Temporal Language Grounding](https://arxiv.org/abs/2110.05717) | Gao et al |[GitHub](https://github.com/Huntersxsx/RaNet)
|107| `GTR` | `Arxiv`| [On Pursuit of Designing Multi-modal Transformer for Video Grounding](https://arxiv.org/abs/2109.06085) | Cao et al |
|108| `SeqPAN` | `Arxiv`| [Parallel Attention Network with Sequence Matching for Video Grounding](https://arxiv.org/pdf/2105.08481.pdf) | Zhang et al |
|109| `S^4TLG` | `Arxiv`| [Self-supervised Learning for Semi-supervised Temporal Language Grounding](https://arxiv.org/abs/2109.11475) | Luo et al |
|110| `IA-Net` | `EMNLP`| [Progressively Guide to Attend: An Iterative Alignment Framework for Temporal Sentence Grounding](https://arxiv.org/abs/2109.06400) | Liu et al |
|111| `LPNet` | `Arxiv`| [Natural Language Video Localization with Learnable Moment Proposals](https://arxiv.org/abs/2109.10678) | Xiao et al |
|112| `PLN` | `Arxiv`| [Progressive Localization Networks for Language-based Moment Localization](https://arxiv.org/abs/2102.01282) | Zheng et al |
|113| `SNEAK` | `Arxiv`| [SNEAK: Synonymous Sentences-Aware Adversarial Attack on Natural Language Video Localization](https://arxiv.org/abs/2112.04154) | Gou et al |
|113| `MGSL-Net` | `Arxiv`| [Memory-Guided Semantic Learning Network for Temporal Sentence Grounding](https://arxiv.org/abs/2112.04154) | Liu et al |
|114| `MMFA-CF` | `IWACIII`| [A Multi-modal Fusion Algorithm for Cross-modal Video Moment Retrieval](https://iwaciii2021.bit.edu.cn/docs/2021-12/3b1c30349c854e168ea5814eef11ac3c.pdf) | Jia et al | 

<br/> -->



<br/><br/>

# Licenses

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [muketong](https://github.com/iworldtong) all copyright and related or neighboring rights to this work.
