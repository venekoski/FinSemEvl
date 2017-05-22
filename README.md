# FinSemEvl

(Copyright) Viljami Venekoski 2017

These are the resources produced for the NoDaLiDa 2017 conference short paper 
"Finnish resources for evaluating language model semantics" by V. Venekoski and J. Vankka. <br />
The full text can be found here: http://www.ep.liu.se/ecp/article.asp?issue=131&article=028. <br />

If you wish to use the data in your research, please cite the following:

@inproceedings{venekoski2017finnish, <br />
author = {Venekoski, Viljami and Vankka, Jouko}, <br />
institution = {National Defence University, Helsinki, Finland}, <br />
booktitle = {Proceedings of the 21st Nordic Conference on Computational Linguistics, NoDaLiDa, 22-24 May 2017, Gothenburg, Sweden}, <br />
number = {131}, <br />
pages = {231-236}, <br />
publisher = {Linköping University Electronic Press, Linköpings universitet}, <br />
title = {Finnish resources for evaluating language model semantics}, <br />
year = {2017}, <br />
issn = {1650-3740} <br />
} <br />

This repository contains three sets of data, one for each evaluation task:

(1) Similarity judgments
The directory has two files: <br />
	'FinnSim_judgment_scores' containing mean and standard deviation
of every 300 word pairs as answered by the 55 respondents <br />
	'SimLex-TranslationsScores' containing the original SimLex-999 scores for the 300 words
	   which were translated into Finnish. The file includes the additional information of
	   the original data set, but do note that the concreteness scores should probably not be
	   applied cross-lingually.<br />

(2) Word intrusion <br />
The directory has multiple files each containing a list of words. The lists were
retrieved from the Finnish language Wikipedia in December 2016. The word intrusion task randomly
samples 5 words from one list and 1 word from another, forming a 6 word intrusion set. This should
be repeated for each ordered pair of lists for a specified number of times. The lists used in
the paper and available here are the following: <br />
	- animals <br />
	- chemical_elements <br />
	- cities <br />
	- colors <br />
	- countries <br />
	- fruit <br />
	- illnesses <br />
	- mathematical_symbols <br />
	- minerals <br />
	- mythical_creatures <br />
	- philosophers <br /> 
	- pieces_of_clothing <br /> 
	- poker_terms <br />
	- professions <br />
	- religions <br />
	- sports <br />

(3) Analogies <br />
The analogy test set contains one file per type of semantic relation. For instance, the file
'ana_gender' gendered analogies, analogizing female-male and male-female pairs. Each file
contains all permutations of analogizable word pairs. Included relations are the following:
	- antonymic adjectives, e.g. 'WET is to DRY what RICH is to POOR' (in Finnish) <br />
	- capital-country, 'BANGKOK is to THAILAND what TALLINN is to ESTONIA" <br />
	- country-currency, 'RUSSIA is to RUBLE what JAPAN is to YEN' <br />
	- female-male, 'MOTHER is to FATHER what GIRL is to BOY' <br />
	- orthogonal directions, 'UP is to DOWN what LEFT is to RIGHT' <br />
	- hockey team-city, 'HIFK is to HELSINKI what TAPPARA is to TAMPERE' <br />
	- cardinal-ordinal number, 'ONE is to FIRST what FIVE is to FIFTH' <br />


We are unfortunately unable to provide the code used to calculate a language model's score in 
each of the above tasks due to the policy of the Finnish Defence Forces where this research was
conducted. However, one should be able to replicate the procedure using methods described in the 
paper. If you need assistance in using these resources in the described manner, do not hesitate
to contact the first author at venekoski[ät]gmail.com or social media.
