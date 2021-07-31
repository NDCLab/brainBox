**Question:**
Broadly: how does the processing of emotional inputs impact our behavior?  Specifically: in what ways does valence (including known effects in semantic integration and priming) impact performance when reading a text aloud, and how is such performance moderated by the relationship between the participant's own mood and the mood that the passage endeavors to evoke?  Is valence or mood congruency a better predictor of performance?

**Summary**
[Recent research](https://journals.sagepub.com/doi/pdf/10.1177/0963721419831992) is throwing away the old notion of "emotional" and "non-emotional" experiences and redefining valence and arousal as part of the default human condition. In this way, a person's mood might be viewed as a filter through which they experience the world.  When faced with conflicting emotional stimuli, an individual might be required to deploy inhibitory control in order to ignore their own mood and interact with the stimulus.  One would be expected to perform better (faster, more accurately) on any task when they do not have to expend resources on such inhibitory control.  Likewise, switching between ends of the valence spectrum may operate similarly to switching between tasks, with emotional switches serving as stumbling blocks to the smooth execution of a task.

This research idea dives into these questions by exploring speed and articulation accuracy in an ecologically valid context: reading a text aloud.  Texts are designed to be heavy on emotional words, allowing performance to be analyzed according to elements of the stimuli themselves (passage valence and direction of the emotional switch) as well as on individual differences (mood state, emotion regulation abilities, and measures of anxiety).

**Lit Review:**
(See literature/lit-review.xlsx.)

Emotion has moderator effects on cognition and behavior, with processing advantages often seen for valenced (positive/negative) words presented visually relative to neutral and, once stimuli are corrected for unprimed response times, improved processing for positive over negative targets.  Additional effects have been seen for positive stimuli with N400 amplitudes and strategies used for memorization.  Some highlights of the lit review include:

- slower processing of negative stimuli (versus positive) as seen by slower response times on negative target words in lexical decision tasks with stimuli that have been matched for response time on unprimed lexical decision tasks (Kazanas and Altarriba (2015a, 2015b))
- positive primes in lexical decision tasks ostensibly cause spreading activation in the semantic network, thereby shortening response time for related target words but slowing response for unrelated target words; negative primes seem to cause an emotional reaction inhibition that precludes any change in response time for related/unrelated targets but enables faster processing for unrelated targets than a positive prime, with its larger network activation (Sass et al. (2012))
- N400 amplitudes are believed to index the activation of semantic knowledge structures, with larger N400 amplitudes for mood-incongruent words (Chung et al. (1996) as mentioned in Kiefer et al. (2007))
- smaller N400 amplitudes for pleasant v. unpleasant adjectives in silent reading, which may indicate that pleasant words are semantically-integrated more easily, possibly as a result of congruency with default, mildly positive mood states (Herbert et al. (2008))
- facilitation of encoding of mood-congruent words in positive mood thanks to a greater tendency toward an elaborative (rather than rote) encoding style (Kiefer et al., 2007)


**Hypotheses:**
_Prediction 1A_
When sublexical characteristics are held constant in a primed reading paradigm, individuals appear to process positive words faster than negative.  As a result, this positivity bias -- which is ostensibly caused by the larger network activation of positive words -- would impact reading speed and error rate in valenced passages, with faster reading speeds and fewer errors in positive passages than negative passages.  However, the real world does not hold sublexical characteristics constant and unprimed lexical decision tasks do not find a significant difference between positive and negative stimuli, only a bias toward emotional stimuli relative to nonemotional stimuli in accordance with the model of motivated attention, which posits that emotion-evoking stimuli capture and retain attention better than neutral stimuli.  Therefore, performance may not differ when reading positive and negative passages, provided that the passages are matched on non-neutrality.
* **A**: no difference in reading speed/disfluency between positive and negative passages
* **B**: positivity bias: faster speeds and fewer disfluencies on positive passages relative to negative

_Prediction 1B_
If good mood and bad mood lead to differing adaptive strategies  (appetitive/assimilative/creative for good mood, aversive/accommodative/non-creative for bad mood), participant mood state may moderate the relationship between passage valence and reading aloud performance, with faster reading speeds and fewer errors in passages that more closely match the participant's mood state.  This effect may be heightened in positive mood; that is, participants in more positive mood may perform better on positive passages than all other conditions, including negative passages read in negative mood state.  This effect may also be curbed in negative mood, such that negative mood leads to similar performance on positive and negative passages.  It is also possible that the more "creative" strategies deployed in good mood could lead to faster performance but a dampened concern over errors such that good mood results in faster speeds across valence conditions but a higher probability of articulatory error.
* **A**: mood-congruency: faster speeds and fewer disfluencies on passages that better match mood state
* **B**: mood-congruency + positivity advantage: best performance on positive passages in good mood
* **C**: negativity dampening: similar performance in negative mood on positive and negative passages
* **D**: creativity trap: faster speed but more disfluencies in positive mood

    Independent Variables
    - variable 1: valence rating of passage-portion, calculated using the "emotional tone" rating from [LIWC](https://liwc.wpengine.com/) {continuous, higher numbers represent more positive tone}
    - variable 2: whether passage-portion was pre- or post-switch {categorical, treated as binary}
    - variables 3+ (1B only): participant measures on initial questionnaires (BMIS, etc.) {continuous}

    Dependent Variables
    - speed of reading aloud: syllables (required to read the text, not necessarily as produced) / second {continuous}
    - percentage of disfluent syllables: number of disfluent syllables (repeated syllable, pre-syllable pause or interjection, and/or mispronounced syllable) / syllables required to read the text aloud {continuous}

_Prediction 2_
Sass et al. (2012) found an interesting pattern in valence priming: positive words are highly effective in priming other positive words, but negative words don't really "prime" anything (that is, RT on lexical decision for target words is similar for both related (negative) and unrelated (positive) targets following a negative prime).  More interesting yet, when they compared RTs for positive-prime>negative-target against negative-prime>positive-target, participants actually performed better in the **latter**.  If positive words activate a larger semantic network whereas compensatory mechanisms prevent such extensive network activation following exposure to negative words, one would expect a greater likelihood of disfluency at a positive>negative switch than a negative>positive switch.  Alternately, if shifting between valence contexts is akin to task-switching, the surprisal associated with the conflicting valence would be expected to impede performance in either direction, but particularly when hitting a valenced word contradictory to one's current mood state.
* **A**: positive activation and negative compensation: fewer disfluencies in negative>positive switches than reverse
* **B**: general surprisal: similar disfluency rates positive>negative and negative>positive
* **C**: mood-incongruent surprisal: enhanced disfluency rates when hitting switch that conflicts with current mood state

    Independent Variable
    -variable 1: type of switch (pos>neg or neg>pos) {categorical}
    - variables 2: participant measures on initial questionnaires (BMIS, etc.) {continuous}

    Dependent Variable
    percentage of disfluent syllables across three factors:
    | pre-switch group| switch group | post-switch group|
    |--- | --- |
    | 7 6 5 4 3 | 2 1 switch 1 2 | 3 4 5 6 7 |
        a) within the switch group (two words prior to the switch, the switch itself, and two words following the switch)
        b) in the word group prior to the switch (the five words prior to the switch group)
        c) in the post-switch word group (the five words that following the switch group)
    *Note 1*: I feel that syllables form a logical 'unit' in which to measure disfluency.  However, as semantic integration is required to prepare articulation during reading aloud, I propose that we slice on the word level for analyzing disfluency around the switch.
    *Note 2*: As a starting point, I selected groups of five words; this may need to be revised.  Some prior research has looked into how far ahead people begin semantic and phonological encoding (so they understand an upcoming word and prepare to articulate it). For instance, if a participant is articulating three words prior to the switch word, but they have already seen the switch word and begun to integrate it semantically (and assuming this does actually affect their performance in reading aloud), they might stumble three words before the actual switch word. Alternately, they might recruit all the necessary resources to articulate the switch correctly...and then stumble after they successfully make it past the switch word. My to-read list includes [this article](https://www.frontiersin.org/articles/10.3389/fpsyg.2015.01432/full), which may provide better guidance.

**Design:**
Prior to the experimental task, participants complete several questionnaires:
- Demographic questionnaire
- Emotion Regulation Questionnaire (ERQ)
- Interpersonal Emotion Regulation Questionnaire (IERQ)
- Beck Depression Inventory (BDI-II)
- State-Trait Anxiety Inventory (STAI)
- Affective Reactivity Index (ARI)
- Brief Mood Introspection Scale (BMIS)

After completion of the questionnaires, participants are prompted to speak briefly (~1 minute) on any topic; this brief narrative is recorded.  Ostensibly, the purpose of this is to test and calibrate the online recording system.  For the initial analyses, this brief narrative does not serve any specific purpose; however, future analyses may be able to correlate qualities of the narrative with the BMIS measurement.

The main study task involves the reading aloud of 21 short texts (~200 words each) that are designed to evoke a certain mood state in the reader (positive/negative) at the start of the passage, but include a single valence "switch point" where the mood of the text suddenly reverses. (Examples: [pos>neg passage](https://github.com/NDCLab/brainBox/blob/rwe-valence-jess/brainy-ideas/rwe-valence-jess/stimuli/pos-neg_dolphins.txt) and [neg>pos passage](https://github.com/NDCLab/brainBox/blob/rwe-valence-jess/brainy-ideas/rwe-valence-jess/stimuli/neg_pos_dolphins.txt).)  Seven blocks of texts, with each block including three texts, are presented back-to-back in such a way that "switch points" are passage-internal (not between passages) and the total amount of "positive" text is equal to the total amount of "negative" text.  Participants are instructed to read the texts aloud at a comfortable speed, articulating clearly and naturally as if they were rehearsing for a documentary voiceover.  Between each block, a "break" is provided during which the participant is prompted to speak on any topic (similar to the initially recorded narrative) and in keeping with the ecological validity of the study: people typically "chat" when they take breaks between regular life tasks.  The primary functions of these breaks are to give the participant a rest period from the tasking activity of reading aloud and to put the participant back in control of their own mood state before the next block.  A secondary function, if future analyses are able to correlate narrative qualities with the initial BMIS measurement, is to offer the possibility of identifying more dynamic changes in mood during the reading aloud task.

After all seven blocks of the reading aloud task are complete, the participant is prompted to share their overall impression of the activity (~1 minute), which is recorded.  They then re-complete the BMIS.

I believe that, with careful setup, this study could be completely asynchronous as [PsychoJS now supports microphone input](https://www.psychopy.org/changelog.html).

**Funding:**
Require guidance on short-term funding. Some longer-term possibilities include:

- NIH R03
- NIH R21 (for greater RWE)
- NSF CogNeuro
- NSF PAC (Perception, Action & Cognition)

**Authors:**
Jess/George, co-authors TBD

**Milestones:**

_Piloting_
In order to get to a piloting stage, we will need to: submit the IRB protocol (including recruitment materials, sample stimuli, and informed consent) and receive approval, create the full stimuli set, determine the neutral prompts for the "breaks", code and test the Pavlovia experiment, setup the REDCap project, and draft the experimental protocol.  It is estimated that this could be completed in the second half of the fall semester.

_Data Coders_
All recordings of the valenced passages must be coded for errors.  I believe that this should be done independently by two coders who are blind to the experimental questions, to decrease the risk that they will be biased in their evaluation of what constitutes a disfluent syllable.  An example tool for coding is provided [here](https://github.com/NDCLab/brainBox/blob/rwe-valence-jess/brainy-ideas/rwe-valence-jess/data/pos-neg_dolphins_coding.xlsx).  Ideally, at least one coder would have completed an introductory Linguistics course.  Training of coders should take place in the second half of the fall semester so that they can begin coding recordings as soon as pilot data begin coming in.

_Analysis 1A_
This analysis involves two multiple regression analyses (one for reading speed, one for accuracy), plus individual t-tests on the assumption the F is significant.

_Analysis 1B_
This analysis involves a slightly more complex model than 1A.  My explicit prediction only involves the BMIS measurement, but I believe that we will want to explore how scores on emotion regulation and state/trait anxiety measures might impact the model.

_Poster: Cognitive Science Society_
This poster would share the results of the 1A and 1B analyses.  The submission deadline is anticipated to be mid-June 2022.

_Analysis 2_
Because each participant will only see 21 switches, a sufficient number of participants will need to be enrolled before analysis can begin on the switches themselves.  We may also need to refine the scope of each "switch group" (see note above).  I do not have an explicit prediction on how emotion regulation abilities and state/trait anxiety measures might impact performance, but we may also want to run exploratory analyses that include these measures.

_Publication_
This paper would share the results of analyses 1A, 1B, and 2.  The goal is to have it submitted by early fall 2022.

_Future Analyses_
Pending further research, it might be possible to use the narrative "breaks" as a dynamic measure of mood state.  The pre-task narrative could potentially be correlated with the pre-task BMIS measurement by looking at acoustic data and lexical choice.  If a reasonable correlation were found, we could then analyze the content of the narrative breaks to better understand how a participant's mood evolved over the course of the task.  The following are on my reading list to better understand feasibility, but I have read that [similar endeavors](https://www.pnas.org/content/115/44/11203) have proven promising...
- [The Psychological Meaning of Words: LIWC and Computerized Text Analysis Methods](https://journals.sagepub.com/doi/pdf/10.1177/0261927X09351676)
- [The role of voice quality in communicating emotion, mood and attitude](https://www.sciencedirect.com/science/article/abs/pii/S0167639302000821)
- [Human voice perception](https://www.sciencedirect.com/science/article/pii/S096098221001701X)
- [A dimensional approach to vocal expression of emotion](https://psycnet.apa.org/doi/10.1080/02699930441000445)