**Question:**
Broadly: how does our perception of emotion impact our behavior?  Specifically: in what ways does semantic valence (and known priming effects) impact performance when reading a text aloud, and how is such performance moderated by the relationship between the participant's own mood and the mood that the passage endeavors to evoke?

**Summary**
According to [Hutchinson and Barrett, 2019](https://journals.sagepub.com/doi/pdf/10.1177/0963721419831992):
> Valence and arousal might be better thought of as properties of consciousness, rather than properties of emotional episodes per se...

In this way, a person's mood might be viewed as a filter through which they experience the world.  When faced with conflicting emotional stimuli, an individual might be required to deploy inhibitory control in order to ignore their own mood and interact with the stimulus.  One would be expected to perform better (faster, more accurately) on any task when they do not have to expend resources on such inhibitory control.  Likewise, switching between ends of the valence spectrum may operate similarly to switching between tasks, with emotional switches serving as stumbling blocks to the smooth execution of a task.

This research idea dives into these questions by exploring speed and articulation accuracy in an ecologically valid context: reading a text aloud.  Texts are designed to be heavy on emotional words, allowing performance to be analyzed according to elements of the stimuli themselves (passage valence and direction of the emotional switch) as well as on individual differences (mood state, emotion regulation abilities, and measures of anxiety).

**Lit Review:**
(See literature/lit-review.xlsx.)

Emotion has moderator effects on cognition and behavior, with processing advantages often seen for positive, visually-presented words:

- slower processing of negative stimuli (versus positive) as seen by slower response times on negative target words in lexical decision tasks (Kazanas and Altarriba (2015))
- positive primes in lexical decision tasks ostensibly cause spreading activation in the semantic network, thereby shortening response time for related target words but slowing response for unrelated target words; negative primes seem to cause an emotional reaction inhibition that precludes any change in response time for related/unrelated targets but enables faster processing for unrelated targets than a positive prime, with its larger network activation (Sass et al. (2012))
- smaller N400 amplitudes for pleasant v. unpleasant adjectives in silent reading may indicate that pleasant words are semantically-integrated more easily, possibly as a result of congruency with default, mildly positive mood states (Herbert et al. (2008))

**Hypotheses:**
_Prediction 1A_
Positivity bias that is ostensibly caused by the larger network activation of positive words would impact reading speed and error rate in valenced passages, with faster reading speeds and fewer errors in positive passages than negative passages.

_Prediction 1B_
Participant mood state may moderate the relationship between passage valence and reading aloud performance, with faster reading speeds and fewer errors in passages that more closely match the participant mood state (that is, participants in more positive mood perform better on positive passages than participants in more negative mood, and vice versa).

    Independent Variables
    - variable 1: valence rating of passage-half, calculated using the "emotional tone" rating from [LIWC](https://liwc.wpengine.com/) {continuous}
    - variable 2: whether passage-half was pre- or post-switch {categorical, treated as binary}
    - variables 3+ (1B only): participant measures on initial questionnaires (BMIS, etc.) {continuous}

    Dependent Variables
    - speed of reading aloud: syllables (required to read the text, not necessarily as produced) / second {continuous}
    - percentage of disfluent syllables: number of disfluent syllables (repeated syllable, pre-syllable pause or interjection, and/or mispronounced syllable) / syllables required to read the text aloud {I think this can be either binary or continuous, depending upon how we run the analysis?}

_Prediction 2_
Larger network activation for positively valenced words and the compensatory mechanisms that seem to be triggered by negatively valenced words would operate to benefit negative>positive switches more than positive>negative, with a greater likelihood of disfluency at a positive>negative switch than a negative>positive switch.

    Independent Variable
    type of switch (pos>neg or neg>pos) {categorical}

    Dependent Variable
    percentage of disfluent syllables across three factors:
        a) within the switch word group (two words prior to the switch, the switch itself, and two words following the switch)
        b) in the pre-switch word group (the five words that precede the switch word group)
        c) in the post-switch word group (the five words that follow the switch word group)
    Note 1: I feel that syllables form a logical 'unit' in which to measure disfluency.  However, as semantic integration is required to prepare articulation during reading aloud, I propose that we slice on the word level for analyzing disfluency around the switch.
    Note 2: As a starting point, I selected groups of five words; this may need to be revised.  My future reading list includes [this article](https://www.frontiersin.org/articles/10.3389/fpsyg.2015.01432/full), which may provide better guidance.

**Design:**
Prior to the experimental task, participants complete several questionnaires:
- Demographic questionnaire
- Emotion Regulation Questionnaire (ERQ)
- Interpersonal Emotion Regulation Questionnaire (IERQ)
- Beck Depression Inventory (BDI-II)
- State-Trait Anxiety Inventory (STAI)
- Brief Mood Introspection Scale (BMIS)

After completion of the questionnaires, participants are prompted to tell a brief story (~1 minute) about something that has already happened to them that day; this brief narrative is recorded.  (Further research is needed to determine how best to ensure that this narrative prompt is neutral.)  For the initial analyses, this brief narrative does not serve any specific purpose; however, future analyses may be able to correlate qualities of the narrative with the BMIS measurement.

The main study task involves the reading aloud of texts (~200 words each) that are designed to evoke a certain mood state in the reader (positive/negative) at the start of the passage, but include a single valence "switch point" where the mood of the text suddenly reverses. (Examples: [pos>neg passage](https://github.com/NDCLab/brainBox/blob/rwe-valence-jess/brainy-ideas/rwe-valence-jess/stimuli/pos-neg_dolphins.txt) and [neg>pos passage](https://github.com/NDCLab/brainBox/blob/rwe-valence-jess/brainy-ideas/rwe-valence-jess/stimuli/neg_pos_dolphins.txt).)  Blocks of texts, perhaps three, are presented back-to-back in such a way that "switch points" are passage-internal (not between passages).  Between each block, a "break" is provided during which the participant is asked to reflect upon a thought/memory evoked by their reading, similar to the initially recorded narrative.  The primary function of these breaks is to recalibrate the participant's mood back to a default state before the next block.  A secondary function, if future analyses are able to correlate narrative qualities with the initial BMIS measurement, is to offer the possibility of identifying more dynamic changes in mood during the reading aloud task.

After the reading aloud task, the participant is prompted to share their overall impression of the activity (~1 minute), which is recorded.  They then re-complete the BMIS.

I believe that, with careful setup, this study could be completely asynchronous as [PsychoJS now supports microphone input](https://www.psychopy.org/changelog.html).

**Funding:**
Require guidance on short-term funding. Some longer-term possibilities include:

- NIH R03
- NIH R21 (for greater RWE)
- NSF CogNeuro
- NSF PAC (Perception, Action & Cognition)

**Authors:**
George/Jess, co-authors TBD

**Milestones:**

_Piloting_
In order to get to a piloting stage, we will need to: perform power analyses to determine an appropriate number of participants to analyze the two sets of predictions, submit the IRB protocol (including recruitment materials, sample stimuli, and informed consent) and receive approval, create the full stimuli set, determine the neutral prompts for the "breaks", code and test the Pavlovia experiment, and setup the REDCap project.  It is estimated that this could be completed in the second half of the fall semester.

_Data Coders_
All recordings of the valenced passages must be coded for errors.  I believe that this should be done independently by two coders who are blind to the experimental question, to decrease the risk that they will be biased in their evaluation of what constitutes a disfluent syllable.  An example tool for coding is provided [here](https://github.com/NDCLab/brainBox/blob/rwe-valence-jess/brainy-ideas/rwe-valence-jess/data/pos-neg_dolphins_coding.xlsx).  Ideally, at least one coder would have completed an introductory Linguistics course.  Training of coders should take place in the second half of the fall semester so that they can begin coding recordings as soon as pilot data begin coming in.

_Analysis 1A_
This analysis involves two multiple regression analyses (one for reading speed, one for accuracy), plus individual t-tests on the assumption the F is significant.

_Analysis 1B_
This analysis involves a slightly more complex model than 1A.  My explicit prediction only involves the BMIS measurement, but I believe that we will want to explore how scores on emotion regulation and state/trait anxiety measures might impact the model.

_Poster: Cognitive Science Society_
This poster would share the results of the 1A and 1B analyses.  The submission deadline is anticipated to be mid-June 2022.

_Analysis 2_
Because each passage only contains one switch, a sufficient number of participants will need to be enrolled before analysis can begin on the switches themselves.  Further work is needed to complete a power analysis in order to determine the appropriate number of participants.  We may also need to refine the scope of each "switch word group" (see note above).  I do not have an explicit prediction on how mood state, emotion regulation abilities, and state/trait anxiety measures might impact performance, but we may also want to run exploratory analyses that include these measures.

_Publication_
This paper would share the results of analyses 1A, 1B, and 2.  The goal is to have it submitted by early fall 2022.

_Future Analyses_
Pending further research, it might be possible to use the narrative "breaks" as a dynamic measure of mood state.  The pre-task narrative could potentially be correlated with the pre-task BMIS measurement by looking at acoustic data and lexical choice.  If a reasonable correlation were found, we could then analyze the content of the narrative breaks to better understand how a participant's mood evolved over the course of the task.  The following are on my reading list to better understand feasibility, but I have read that [similar endeavors](https://www.pnas.org/content/115/44/11203) have proven promising...
- [The Psychological Meaning of Words: LIWC and Computerized Text Analysis Methods](https://journals.sagepub.com/doi/pdf/10.1177/0261927X09351676)
- [The role of voice quality in communicating emotion, mood and attitude](https://www.sciencedirect.com/science/article/abs/pii/S0167639302000821)
- [Human voice perception](https://www.sciencedirect.com/science/article/pii/S096098221001701X)
- [A dimensional approach to vocal expression of emotion](https://psycnet.apa.org/doi/10.1080/02699930441000445)