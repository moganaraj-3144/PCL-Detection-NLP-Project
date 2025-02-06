# Patronizing and Condescending Language - NLP - Project

Patronizing and condescending language (PCL) refers to a form of speech that implies a position of superiority over the listener, often directed towards vulnerable groups, creating a sense of being talked down to and undermining their agency; essentially, it is a way of speaking that treats someone as if they are less intelligent or capable than the speaker, often with the intention of belittling or dismissing their opinions or concerns. 

This project is a SemEval 2022 Task 4, Subtask 1 project, which addresses the topic of Patronizing and Condescending Language (PCL) Detection as a binary classification problem.The dataset is available only upon request to the authors. It can be accessed by contacting them through the link provided on their [SemEval GitHub page](https://github.com/Perez-AlmendrosC/dontpatronizeme).

The dataset contains paragraphs annotated with a label from 0 (not containing PCL) to 4 (being highly patronizing or condescending) towards vulnerable communities.
It contains one instance per line with the following format:

	- <par_id> <tab> <art_id> <tab> <keyword> <tab> <country_code> <tab> <text> <tab> <label>

	where
	- <par_id> is a unique id for each one of the paragraphs in the corpus.
	- <art_id> is the document id in the original NOW corpus (News on Web: https://www.english-corpora.org/now/).
	- <keyword> is the search term used to retrieve texts about a target community.
	- <country_code> is a two-letter ISO Alpha-2 country code for the source media outlet.
	- <text> is the paragraph containing the keyword.
	- <label> is an integer between 0 and 4. Each paragraph has been annotated by two annotators as 0 (No PCL), 1 (borderline PCL) and 2 (contains PCL). The combined annotations have been used in the following graded scale:

	0 -> Annotator 1 = 0 AND Annotator 2 = 0
	1 -> Annotator 1 = 0 AND Annotator 2 = 1 OR Annotator 1 = 1 AND Annotator 2 = 0
	2 -> Annotator 1 = 1 AND Annotator 2 = 1
	3 -> Annotator 1 = 1 AND Annotator 2 = 2 OR Annotator 1 = 2 AND Annotator 2 = 1
	4 -> Annotator 1 = 2 AND Annotator 2 = 2

	The experiments reported in the paper consider the following tag grouping: 
	- {0,1}   = No PCL
	- {2,3,4} = PCL

