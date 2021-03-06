---
layout: post
title:  "Topic Modeling"
date:   2021-03-10 08:00:00 -0500
categories: TPUS
tags: Florida, topic_modeling
---

One of the core questions of the *Territorial Papers of the United States* (TPUS) is to what extent did the selection of archival documents included in the published volumes influence the interpretations of those historians who relied on TPUS? There's potentially a lot to untangle. The premise of my research is that the structure of archives shapes the historical narrative, but at the same time existing historical narratives shape archives. They coproduce each other. So how can we tell if the TPUS shaped the historiography of Florida, or if the narrative of Florida's past had an influence on which documents were included in TPUS? 

Topic modeling may provide some clues. We expect the documents selected in the 1950s to reflect the contemporary emphasis on "great men" in history, with a traditional focus on political, diplomatic, and military histories. This seems confirmed both by the origin of the documents and the headings used to organize them in the published volumes. Out of 664 documents included in volume 22--the first volume on the Territory of Florida--the vast majority, 351 are from the State Department, which handled the administration of non-state territories until the 1870s when that duty shifted to the Department of the Interior. Another 106 documents come from the War Department files. However, it is possible that the contents of the documents may be more complex than this simple administrative narrative. 

In order to investigae the documents at a deeper content level, we can apply a topic modeling algorithm to obtain probably topics in the volume that can then be compared to selections from the historiography before and after TPUS was published.

I selected a random sample of 12 documents from volume 22 of TPUS to test the topic modeling tool. Since I have tagged the entire volume in using XML, it was easiest to load my XML file into OpenRefine and identify record by number using a random number generator. This also allowed me to copy and past the body of each document into individual `.txt` files and then export the rest into a `metadata.csv` file directly from OpenRefine. I tried the Topic Modeling Tool first set to 10 topics, then 5 topics, and finally 7 topics. This seemed to be right number of topics where each had a distinct and recognizable flavor.
<html>
<head>
<style>
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
</style>
</head>
<body>
<table>
	<caption>Topic words</caption>
	<tr>
		<th>Topic Id</th><th>Top Words</th>
	</tr>
	<tr>
		<td>0</td>
		<td>commissioners indians treaty rations intention number furnished president stated views great accompanied estimate meat bread hamilton floyd servant</td>
	</tr>
	<tr>
		<td>1</td>
		<td>bay shields barrels vessel tampa public 1824 burch cost carrying harbor voyage purchase feb 12 jan jesup brig ass</td>
	</tr>
	<tr>
		<td>2</td>
		<td>congress actual petitioners florida states land spanish mark manning claims settlers united hogg james similar acts places territory government floridas</td>
	</tr>
	<tr>
		<td>3</td>
		<td>indians agent government individuals seminole report authority creeks orders unprincipled relation states character find directed purpose sense duties limits tribes</td>
	</tr>
	<tr>
		<td>4</td>
		<td>augustine florida sir honor governor gen states authorities spanish united documents powers east endorsed st respectfully arrival buildings washington</td>
	</tr>
	<tr>
		<td>5</td>
		<td>john river st daniel place jacksonville james william johns dell tucker hogans joseph petition adams made condition youngblood jesse jun</td>
	</tr>
	<tr>
		<td>6</td>
		<td>delivery place supply amelia robert fortress destined troops part occupy island give subsist reached removal arrangements cross commâ condition detachment</td>
	</tr>
</table>
</body>
</html>
The `metadata.csv` file generated from the tool pairs each document in the set with the corresponding percentage of the document that deals with the topics modeled. Admittedly with such a small sample we can't make dramatic conclusions, but we can test the validity of the topic modeling itself. For example, making a pivot table I was able to see the average percentage of each topic's coverage compared to which archival collection the document came from. Topic 3 in this test run is about the indigenous peoples of Florida, with keywords like Indians, agent, Seminole, Creeks, and tribes. Also in this topic were more evocative words like unprincipled, relation, character, sense, and duties. Not surprisingly, this topic had by far the highest percentage in the 2 documents from the Office of Indian Affairs, with a distant second place going to documents from the War Department.

Topic 1 seems to be about war materials and supply lines. Again, we are not surprised to see the highest percentage of documents about this topic coming from the War Department files. Topic 2 about land claims and petitioners finds its highest percentage in the House of Representative Files. Topic 4, which seems to be about the conflict over Spanish government archives during the transition of imperial rule, has very high percentages in the War Department, State Department, and Jackson Papers collections, but significantly less coverage in the Office of Indian Affairs documents.

A much larger sample of documents, perhaps stratified to get better representation from each of the most important archival collections that included in volume 22, may result in more refined topics as well as confirm the distribution of those topics among the different archival components of TPUS. Even more interesting will be the next step, comparing these topics to the historical scholarship about early Florida published at intervals throughout the twentieth century, before TPUS was published, contemporary with the publication, and after TPUS fell out of use among professional historians.