---
layout: post
title:  "Territorial Papers of the United States"
date:   2021-03-07 12:00:00 -0500
categories: TPUS
tags: Florida, data cleaning
---

This project is an attempt to use quantitative research methods to explore and assess how archival materials were valued, assembled, and disseminated in the twentieth century, and how those practices influenced historical writing about the U. S. Gulf South.

[*The Territorial Papers of the United States*](https://catalog.hathitrust.org/Record/000495370) (TPUS) is a 28-volume set of primary source documents published between 1934 and 1975. The project assembled historical documents from the United States Department of State and the National Archives dealing mostly with the administration of territories annexed by the United States that would later become states in the union. Historian Clarence Edwin Carter compiled and edited the first 26 volumes until his death in 1961. The last two volumes were edited by John Porter Bloom.

Print volumes of TPUS are commonly found in libraries throughout the United States. Digital scans are also available in the HathiTrust repository. As U. S. government publications, these volumes are in the public domain. HathiTrust provides plain text files of each volume for download.

As a case study for the broader project goals, the current project will focus on volumes 22-25 in the series, the five volumes dedicated to the territorial period of Florida, 1821-1845. After cleaning the plain text in order to separate the metadata of each document from its contents, I plan to use topic modeling to compare the contours of the documents themselves to historical writing on early Florida. Do the topics written about in journal articles that cite the published TPUS match those of the selected documents? Does that resemblance change over time? The findings of such a comparison may reveal the ways in which published primary sources influence the nature of historial writing.

### Data Cleaning

As mentioned above, the TPUS are available as PDF and plain text files for download from [HathiTrust](https://hathitrust.org). HathiTrust staff have run optical character reading (OCR) technology on the scanned paper editions in order to make the texts machine readable and keyword searchable. However, OCR introduces errors into the text when characters are misidentified and when formatting on the printed page confuses the OCR's algorithms. Thus, a certain about of data clearning is required to correct errors and to isolate the metadata associated with each included document from the text of the document itself.

As shown in the example page below, each document in TPUS is surrounded by descritive data and text provided by the series editor. The metadata include a descriptive header, a citation to the archives and collection from which the docment is taken, and the date and location the document was created, where known. Also included with most documents are explanatory footnotes. The consistency in formatting throughout the 28-volumes allows us to use a combination of regular expressions and OpenRefine to identify and tag with XML the various parts of each document. The detailed steps I used are availble in the [ReadMe.md](https://github.com/comp-methods-fsu-2021/Beauchamp_TPUS_project/blob/main/TPUS_Florida_corpus/TPUSv22/ReadMe.md) file associated with volume 22, the first volume in TPUS that deals with Florida, and the volume I started with to learn the text cleaning process.

![Example page from TPUS volume 22](/assets/images/TPUS_v22_Florida_p84.png)