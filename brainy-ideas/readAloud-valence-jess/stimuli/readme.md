## Overview of the Experimental Stimuli

This folder contains the following:

**ReadAloud Task (readAloud/)**
- 3 txt files, each containing one stimulus passage and the challenge question associated with it (remaining passages currently being drafted)
- an Excel workbook containing passage-level and word-level characteristics for the readAloud stimuli completed to date (in progress)
- an Excel workbook containing coding structure for each reading passage (in progress)
- (TBD): for each passage, a CSV file from the English Lexicon Project used to acquire most of the word-level characteristics, along with a CSV file with summary characteristics (ELP transaction number is noted in cell A1 of the associated worksheet)

**Lexical Decision Task (ldt/)**
- an Excel workbook containing (sub)lexical characteristics for the LDT stimuli words
- a CSV file from the English Lexicon Project used to acquire most such characteristics
- a CSV file from the English Lexicon Project with summary characteristics


### Text Passage Characteristics

| characteristics | resource | notes |
|:-- | :-- | :-- |
|switch-type | manual extraction | Indication of directionality of the passage's valence shift, from negative to positive (neg2pos) or positive to negative (pos2neg) |
|emo-tone-all | LIWC | Overall emotional tone of the entire passage |
|emo-tone-pos | LIWC | Emotional tone of the positive portion of the passage |
|emo-tone-neg | LIWC | Emotional tone of the negative portion of the passage |
|flesch-all | MS Word | A measure of [reading ease](https://en.wikipedia.org/wiki/Flesch%E2%80%93Kincaid_readability_tests#Flesch_reading_ease) for the entire passage |
|flesch-pos | MS Word | Flesch score for the positive portion of the passage |
|flesch-neg | MS Word | Flesch score for the negative portion of the passage |
|len-words-all | manual extraction | Number of words in the entire passage |
|len-words-pos | manual extraction | Number of words in the positive portion of the passage |
|len-words-neg | manual extraction | Number of words in the negative portion of the passage |
|len-syll-all |manual extraction | Number of syllables in the entire passage, baed on the main pronunciation of the word |
|len-syll-pos |manual extraction | Number of syllables in the positive portion of the passage |
|len-syll-neg |manual extraction | Number of syllables in the negative portion of the passage |
|pos-avg-WAR |Warriner et al. (2013) {from ELP} | Average valence rating of word lemmas in the positive portion of the passage. Used as preliminary indicator during drafting of valenced passages. |
|neg-avg-WAR |Warriner et al. (2013) {from ELP} | Average valence rating of word lemmas in the negative portion of the passage. Used as preliminary indicator during drafting of valenced passages. |
|pos-strength-WAR |manual calculation | Distance between pos-avg-WAR and the average of the Warriner et al. (2013) corpus (5.2). Used as preliminary indicator during drafting of valenced passages. |
|neg-strength-WAR |manual calculation | Distance between neg-avg-WAR and the average of the Warriner et al. (2013) corpus (5.2). Used as preliminary indicator during drafting of valenced passages. |


### (Sub)Lexical Characteristics: Primary Interest

All characteristics are drawn from the lemma unless otherwise noted.  For characteristics drawn from the English Lexicon Project, the full lexicon was queried. Within the Excel workbook containing the passage-level and word-level characteristics for the readAloud stimuli, these characteristics are recorded for each word in each text passage; the switch words are copied into an additional, standalone tab.

| characteristics | resource | notes |
|:-- | :-- | :-- |
| valence | Kousta et al. (2009) rating (-kousta); ANEW 2017 (-ANEW); Warriner et al. (2013) {from ELP} (-WAR); Glasgow Norms (-GLAS)| Valence indicates the rating of the word on a scale from negative/unhappy to positive/happy.  The categorical rating attributed to Kousta et al. (2009) here is indicative of how stimuli were selected in their experimental setup; note, however, that in their analyses they used an extension of the ANEW ratings that provided a more normal frequency distribution across the valence spectrum than ANEW alone.  Subsequent work has found that the Warriner et al. (2013) ratings are more closely aligned with natural language.  Glasgow TBD. Scales: ANEW: from 1 (unhappy) to 9 (happy); Warriner: from 1 (unhappy) to 9 (happy); Glasgow: TBD |
| valence-strength-WAR | distance from neutral, median valence rating of 5.06| According to Warriner et al. (2013), more extremely valenced words tend to display less variability in their ratings than neutral words; therefore, words with higher values for valence-strength-WAR are likely to be more reliable than words with lower values. The median of the "V.Mean.Sum" column of data in the Warriner et al. (2013) dataset was calculated using the median() function in Microsoft Excel 16.52. |
| log-freq | HAL corpus {from ELP} (-HAL); SUBTLEX corpus {from ELP} (-SUB) | The log of the frequency of the word in the HAL corpus or SUBTLEX corpus, respectively. |
| no-syll | English Lexicon Project | Number of syllables in the main pronunciation of the (full) word. |
| no-lett | len() formula in Excel | Number of letters in the American spelling of the (full) word. |
| pos | English Lexicon Project | Part of speech: JJ (adjective), NN (noun), RB (adverb), VB (verb), encl (enclitic), minor (all other parts of speech), ? (unknown). A vertical bar is used to separate alternatives when a given word can be used as multiple parts of speech. |
| 5-gram-cum-surprisal | kenLM on Gigaword 3? (is FIU a member of the Linguistics Data Consortium?) | TBD: cumulative, linear surprisal predicts reading time very well, must be log transformed (Smith+Levy) |

### (Sub)Lexical Characteristics: Secondary Interest

| characteristics | resource | notes |
|:-- | :-- | :-- |
| arousal | ANEW 2017 (-ANEW); Warriner et al. (2013) {from ELP} (-WAR); Glasgow Norms (-GLAS)| Arousal indicates the rating of the word on a scale from calm to excitatory.  Kuperman et al. (2014) found that valence and arousal have independent effects on lexical decision and speeded naming, with arousal have a substantially stronger effect. Scales: ANEW: from 1 (calm) to 9 (excited); Warriner: from 1 (calm) to 9 (excited); Glasgow: TBD |
| dominance | ANEW 2017 (-ANEW); Warriner et al. (2013) {from ELP} (-WAR); Glasgow Norms (-GLAS)| Dominance indicates the rating of the word on a scale from low-control to high-control. Scales: ANEW: from 1 (controlled) to 9 (in control); Warriner: from 1 (controlled) to 9 (in control); Glasgow: TBD |
| aoa-root | Kuperman et al. (2012) {from ELP} | Average age the word is learned (age of acquisition). |
| OLD20 | English Lexicon Project | The mean Levenshtein distance (the minimum number of letter insertions/deletions/substitutions needed to transform the target word into another word) between the word and its 20 closest neighbors (orthographic Levenshtein distance). |
| PLD20 | English Lexicon Project | The mean Levenshtein distance (the minimum number of phoneme insertions/deletions/substitutions needed to transform the target word into another word) between the word and its 20 closest neighbors (phonologic Levenshtein distance). |
| no-phon| English Lexicon Project | Number of phonemes in the main pronunciation of the word.  Diphthongs and affricates count as single phonemes. |
| no-morph | English Lexicon Project | Number of morphemes in the word. |
| concreteness | Brysbaert et al. (2013) {from ELP} | Mean of concreteness, on a scale from 1 (abstract and language-based) to 5 (concrete and experience-based). |
| body-object | Pexman et al. (2018) {from ELP} | A measure of the ease with which the human body can interact with the word’s referent.  High body-object words tend to be more concrete. |
| mean-bigram-freq | English Lexicon Project |  Average bigram frequency, where a bigram is a sequence of two letters.  To calculate the average, the sum of the frequencies of successive bigrams is divided by the number of successive bigrams. |
| ldt-rt | English Lexicon Project | Standardized, mean lexical decision latency across all participants who encountered the word in the ELP lexical decision task. |
| ldt-acc | English Lexicon Project | Mean accuracy across all participants in the ELP lexical decision task, excluding errors and outliers. |
| ldt-obs | English Lexicon Project | Number of observations used to calculate ldt-rt and ldt-acc. |
| name-rt | English Lexicon Project | Standardized, mean naming latency across all participants who encountered the word in the ELP speeded naming task. |
| name-acc | English Lexicon Project | Mean accuracy across all participants in the ELP speeded naming, excluding errors and outliers. |
| name-obs | English Lexicon Project | Number of observations used to calculate name-rt. |
| imageability | Glasgow Norms | The degree of effort, from 1 (very unimageable) to 7 (very imageable), involved in generating a mental image of something. |
| familiarity | Glasgow Norms | A measure of a word’s subjective experience, from 1 (unfamiliar and rarely encountered) to 7 (familiar and often encountered). |
