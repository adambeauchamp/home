---
layout: post
title:  "The View from 30,000 (Linear) Feet"
date:   2021-04-13 20:00:00 -0500
categories: TPUS
tags: Florida, data visualization
---

One of my goals for this project is to consider the collections of primary sources in ways that are distinct from the individual source analysis that is the foundation of historical research. I propose that in addition to careful reading of "the sources," historians also critically read "the archives" and the way in which the organization, description, and preservation interacts with historical knowledge production. Of course I do not refer to *the* metaphorical *archive*, that ubiquitous term of art used to describe the sum total of possible historical source material, but rather that real archival collections that are kept in real buildings, organized and described by archivists, who work in the context of real institutions with budgets, policies, and missions that will determine, in part, what and how historians will discover in the course of their research.

In order to analyze collections, we have to consider a wider perspective on the source materials, the proverbial 30,000 foot view. Archivists are accustomed to seeing archives from this vantage point, assessing and appraising documents first in bulk, then with increasing granularity, but only as budgets and labor resources allow. Most collections will never be described at the individual document level. However, a publication such as *The Territorial Papers of the United States* (TPUS) offers an opportunity to see both sources and collections. In this case, the TPUS consists of documents selected from several colletions within the United States National Archives, and is itself a kind of synthetic collection, assembled not by provenance but by an editor's criteria.

Analyzing the TPUS as a collection lends itself to computational measures because we can count the number of documents that were drawn from the various collections of the National Archives. We can also describe and analyze the number of documents using the metadata we were able to identify and tag during the data cleaning process. For example, in this visualization, we are counting the number of documents from each archival collection by year. As you can see, the largest number of documents are from 1825 and 1827, while the TPUS has the fewest number of documents from 1837, 1838, and 1839.

<div class='tableauPlaceholder' id='viz1618361069177' style='position: relative'><noscript><a href='#'><img alt='Sources of Documents by Year included in the Territorial Papers of the United States ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;SourcesbyYearCollection&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TerritorialPapersoftheUSbyArchivalCollection&#47;SourcesbyYearCollection' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;SourcesbyYearCollection&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1618361069177');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

The dramatic difference in total documents by year may prompt questions about the historical events that might have caused this shift in documentation. Does the reduced size of the archive have something to do with the [Second Seminole War (1835-1842)](https://en.wikipedia.org/wiki/Second_Seminole_War)? That, of course, is a trick question. The TPUS is neither "the archive" of Territorial Florida, nor is it really "an archive" of Territorial Florida. It is a publication project whose contents were selected Clarence Edwin Carter, the editor of the TPUS until his death in 1961. Carter followed very specific criteria, which he devised, when deciding which documenets to include in the TPUS project. As he described in the Preface to volume 22, the first of five to cover the Territory of Florida, Carter's selection process was first and foremost determined by his budgetary constraints. He excluded documents previously published elsewhere, those he considered trivial or routine, and duplicates. Finally, he prioritized documents covering the federal administration of the territory in order to give the entire TPUS series a coherent theme.

Carter also made some decisions specific to the Territory of Florida. First, he admits that the adjudication of land claims was so important to the territorial period that to include all documents of the General Land Office and others relating to land titles and surveys would have overwhelmed any other type of document he might include. Carter also noted that documents pertaining to Indians in Florida "are so enormous in quantity that a separate and different publication would be required to provide an adequate documentary collection." (TPUS 22:vii). Thus, Carter himself reduced the number of documents in the TPUS pertaining to land claims and the Seminoles in Florida, potentially skewing the character of "the archive" he was presenting to future historians.

The effect of Carter's selection criteria certainly influence the balance of topics covered in the TPUS as compared to the numbers of documents one might find in the original archival collections. However, if we adjust our visualization to show how the documents by year are divided among the five published volumes of the TPUS, we might conclude that Carter's first criteria, budget, had a greater impact.

<div class='tableauPlaceholder' id='viz1618362491184' style='position: relative'><noscript><a href='#'><img alt='Sources of Documents by Year and Volumeincluded in the Territorial Papers of the United States ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;SourcesbyYearCollectionwithVolumes&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TerritorialPapersoftheUSbyArchivalCollection&#47;SourcesbyYearCollectionwithVolumes' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;SourcesbyYearCollectionwithVolumes&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1618362491184');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

With this detail added to the visualization we can begin to see differences among the volumes, which were published over several years between 1956 and 1962. Volume 23 seems to stack up like a tidal wave, with a large number of documents concentrated in a roughly three-year timespan. Volume 24 has fewer documents per year, but covers about six years total. Volume 25 covers about five years, but has noticeably fewer documents that the previous volume. The final volume, Volume 26, seems to return to the document levels of Volume 24, though the distribution over years seems less consistent.

If we remove the document years from our analysis and just compare total number of documents in each volume, the discrepancy is obvious.

<div class='tableauPlaceholder' id='viz1618363112271' style='position: relative'><noscript><a href='#'><img alt='Total Documents by Volume ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;TotalDocumentsbyVolume&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TerritorialPapersoftheUSbyArchivalCollection&#47;TotalDocumentsbyVolume' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;TotalDocumentsbyVolume&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1618363112271');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

Volume 25 has is nearly half the size of Volume 23, the largest of the Florida set. Why is this volume so much smaller that the others? Is this a function of Carter's selection criteria? Or was this a bad budget year? Or was something else entirely? Answering this question will require further research. However, we might be able to eliminate one hypothesis with a final visualization. 

<div class='tableauPlaceholder' id='viz1618363419557' style='position: relative'><noscript><a href='#'><img alt='Percent Source Collection by Volume ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;PercentSourceCollectionbyVolume&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='TerritorialPapersoftheUSbyArchivalCollection&#47;PercentSourceCollectionbyVolume' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Te&#47;TerritorialPapersoftheUSbyArchivalCollection&#47;PercentSourceCollectionbyVolume&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1618363419557');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

We know that Volume 25 has the fewest total documents. If we consider what percent of those documents come from each archival collection, however, we see some consistency across all five volumes. Volume 25 has a higher percentage of documents from the Treasury Department than previous volumes, perhaps accounting for the relative decrease in documents from other collections, but the decreases have been applied across the board, and do not seem to reflect a particular silencing of documents from one archival source. I suspect, then, that Carter did not adjust his selection criteria in some way. Instead, I hypothesize that a budget constraint of some sort resulted in a much smaller Volume 25 that just happened to coincide with the years marking the outbreak of the Second Seminole War. 

Perhaps the answers to these questions, elicited by visualizing the contours of the TPUS as a whole, can be found through a close reading of the documents themselves. More likely, we can find our answers by researching the administration of the TPUS project, perhaps discoverable among the [Clarence Edwin Carter papers](https://www.loc.gov/item/mm78015271/) at the Library of Congress.