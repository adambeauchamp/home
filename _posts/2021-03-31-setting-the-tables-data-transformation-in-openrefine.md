---
layout: post
title:  "Setting the Tables: Data Transformations in OpenRefine"
date:   2021-03-30 21:00:00 -0500
categories: TPUS
tags: Florida, data cleaning
---

Last week I wrote a post about my data cleaning work, transforming plain text files from five volumes of the *Territorial Papers of the United States* into XML files that I can use for analysis of the collection as a whole. I have largely completed that phase of XML tagging; each volume of the *TPUS* relating to Florida is now tagged and uploaded into my GitHub site. 

Once I completed the XML tagging using regular expressions and some manual text cleaning, I create a table of the data using OpenRefine. I decided it was not critical to treat each of the five volumes separately, so I uploaded all five XML files at once into a single OpenRefine dataset. OpenRefine created a column that identified for each row which individual file it came from, which is handy, and may be of some interest later if I determine that the *TPUS* project itself changed over time. The first Florida volume was published in 1956 and the last in 1962, so I don't expect any radical changes in the selection process, but it may be worth comparing these to the earliest volumes of the set, published in the 1930s.

### Transforming Data

I'm still learning its finer points, but OpenRefine is a powerful tool for transforming large datasets. I'm pretty handy with an Excel spreadsheet, but OpenRefine can handle larger datasets and has the invaluable ability to [Cluster & Edit](https://docs.openrefine.org/manual/cellediting/#cluster-and-edit). This feature provides several different algorithms with which you can match similiar (but not exact) values in your data and merge or edit them as needed. This was particularly helpful for the many variant spellings and abbreviations I found in the *TPUS* documents. Some of the variation was from the original documents themselves, reflecting nineteenth-century inconsistencies. Other variations seem to be attributable to mistakes in the OCR. Months were particularly thorny in my text, with multiple abbreviations used for each month of the year. I also found a few instances where OIA, the abbreviation for Office of Indian Affairs, had been captured by the OCR as OLA.

I was also able to split columns into distinct variables across the entire dataset while joining others. My XML tagging using regular expressions simply identified the source citation for each doument. In OpenRefine, I split the ``<source>`` data into three columns, one for the institution (e.g. National Archives, Library of Congress), one for the records collection (e.g State Department, Andrew Jackson Papers), and the third for the rest of the citation. I then used the cluster & edit feature to standardize the spellings and names of these archival sources. This will be important for a later stage of the project where I attempt to both quantify the sources of documents and use topic modeling to generalize about the subject matter of each collection. 

I also used OpenRefine to standardize dates. As mentioned above, the months had wildly variant spellings, but the format of dates are also inconsistent. I put in a lot of effort during the XML tagging stage to isolate dates, months, and years, but there was still some cleaning to do. The faceting feature in OpenRefine allowed me to identify dates and years that made no sense and edit them. In some cases a regular expression had gone awry and identified a different number as the date. In others a bad OCR had transformed "3d", as in third, into "34." There are probably similar cases where "2d" was mistaken for a two-digit number, but since month is more interesting for my purposes, I determined it was not worth the effort to try to identify and correct these, if any. Once the three data points were cleaned, I was able to create a new column with dates standardized in the [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format, which will faciliate analysis and visualizations in the next phase of the project.

A ``TSV`` file of the entire dataset, now in tabular form, is uploaded to my GitHub site in the ``\TPUS_documents_TSV`` folder. It is perhaps worth noting that I originally named this folder CSV. However, since my data is full of commas already, it seemed unwise to create a *comma-separated values* file.

### Next Steps

Before I move into data visualizations, I want to return to OpenRefine and find a way to categorize the types of documents in my dataset. Before using OpenRefine, I had used a forumla in Excel to identify correspondence in volume 22, the first file that I cleaned. These always had document headers that followed the formula *PERSON* TO *PERSON*, where *PERSON* was either a proper name or title (e.g. The Secretary of War). Similar to regular expressions, there was not a single Excel formula that could isolate this pattern without missing some headings and misidentifying others. I want to work on this a bit more so that I can categorize each document type for further analysis. A ``CSV`` file of this work on volume 22 data is currently in the ``\TPUS_documents_TSV`` folder for reference.