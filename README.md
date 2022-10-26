# Read Me

These are two newly annotated datasets for the research of identifying (dis)agreement relations between *(Quote, Response)* comment pairs in social media platform.

**Paper:** Few-Shot (Dis)Agreement Identification in Online Discussions with Regularized and Augmented Meta-Learning<br/>
**Accepted:** The 2022 Conference on Empirical Methods in Natural Language Processing (EMNLP 2022)<br/>
**Authors:** Yuanyuan Lei, Ruihong Huang<br/>
**Affiliation:** Texas A&M University, College Station, Texas, USA<br/>

<br/>

**Task Description**<br/>
In online discussion forums and social media platforms, people express different opinions towards a common topic, by posting their comments towards a given question or replying to another user's previous comments. We call the comments replying to another comments as *Response* and the comments being replied as *Quote*. Researching the relation between *(Quote, Response)* pairs will enable many opinion mining applications. To be detailed, the task is identifying the relation between *(Quote, Response)* pair to be *Agreement*, *Disagreement*, or *Neutral*.

<br/>

**Dataset Description**<br/>
We collected and annotated two datasets from Reddit (https://www.reddit.com/) on two recent new topics, mask mandate and COVID vaccine, containing 1.5k and 1.4k comment pairs respectively, in the year of 2021.
* **SubReddit-MaskMandate** (SubReddit-MaskMandate.csv) is collected from a sub forum on Reddit with the topic of mask mandate (https://www.reddit.com/r/antimaskers/), discussing whether people should wear masks during the COVID pandemic. The Cohen's kappa between annotators is 0.8012.
* **SubReddit-CovidVaccine** (SubReddit-CovidVaccine.csv) is collected from a sub forum on Reddit with the topic of COVID vaccine (https://www.reddit.com/r/CovidVaccinated/), discussing whether people should take the COVID vaccination. The Cohen's kappa between annotators is 0.8215.

<br/>

**Dataset Usage**<br/>
There are three columns in the two datasets:<br/>
* **quote_text:** the text of *Quote* comments
* **response_text:** the text of *Response* comments
* **relation:** the annotated relation between *(Quote, Response)* pairs, containing three different classes, where 0 represents *Disagreement*, 1 represents *Neutral*, and 2 represents *Agreement*

<br/>

**Dataset Statistics**<br/>
| Dataset                  | Agree | Disagree | Neutral |  Total  |
| ------------------------ | ----- | -------- | ------- | ------- |
| SubReddit-MaskMandate    |  645  |   546    |   343   |   1534  |
| SubReddit-CovidVaccine   |  272  |   425    |   703   |   1400  |

<br/>

**Annotation Guideline**<br/>
Every *(Quote, Response)* pairs are annotated with one of *Agreement*, *Disagreement*, and *Neutral* labels:
* ***Agreement:*** both *Quote* and *Response* express subjective opinions towards some topics instead of sharing objective experience or giving objective advice, and there is explicit or implicit evidence for agreement / support / semantically similarity.
* ***Disagreement:*** both *Quote* and *Response* express subjective opinions, and there is explicit or implicit evidence for disagreement / attack / denial / reject / challenge / semantically opposition.
* ***Neutral:*** *Quote* or *Response* is not expressing subjective opinions, or *Quote* and *Response* are stating quite different / unrelated things, or both *Quote* and *Response* express opinions but *Response* is expressing vague / not sure / weak agreement or disagreement, or partially agree partially disagree.

<br/>

**Citation:**<br/>





