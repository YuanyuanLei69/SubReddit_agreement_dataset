# Read Me

These are two newly annotated datasets for the research of identifying (dis)agreement relations between *(Quote, Response)* comment pairs in social media platform.

<br/>

**Paper:** Few-Shot (Dis)Agreement Identification in Online Discussions with Regularized and Augmented Meta-Learning<br/>
**Accepted:** The 2022 Conference on Empirical Methods in Natural Language Processing (EMNLP 2022)<br/>
**Authors:** Yuanyuan Lei, Ruihong Huang<br/>
**Affiliation:** Department of Computer Science and Engineering, Texas A&M University, College Station, Texas, USA<br/>

<br/>

**Task Description**<br/>
---
In online discussion forums and social media platforms, people express different opinions towards a common topic, by posting their comments or replying to another user's previous comments. We call the comments replying to another comments as *Response* and the comments being replied as *Quote*. Researching the relation between *(Quote, Response)* pairs will enable many opinion mining applications. Specifically, the task is identifying the relation between *(Quote, Response)* pair to be *Agreement*, *Disagreement*, or *Neutral*.

<br/>

**Dataset Description**<br/>
---
We collected and annotated two datasets from Reddit (https://www.reddit.com/) on two recent new topics, mask mandate and COVID vaccine, containing 1.5k and 1.4k comment pairs respectively, in the year of 2021.
* **SubReddit-MaskMandate** (SubReddit-MaskMandate.csv) is collected from a sub forum on Reddit with the topic of mask mandate (https://www.reddit.com/r/antimaskers/), discussing whether people should wear masks during the COVID pandemic. The Cohen's kappa between annotators is 0.8012.
* **SubReddit-CovidVaccine** (SubReddit-CovidVaccine.csv) is collected from a sub forum on Reddit with the topic of COVID vaccine (https://www.reddit.com/r/CovidVaccinated/), discussing whether people should take the COVID vaccination. The Cohen's kappa between annotators is 0.8215.

<br/>

**Dataset Usage**<br/>
---
There are three columns in the two datasets:<br/>
* **quote_text:** the text of *Quote* comments
* **response_text:** the text of *Response* comments
* **relation:** the annotated relation between *(Quote, Response)* pairs, containing three different classes, where 0 represents *Disagreement*, 1 represents *Neutral*, and 2 represents *Agreement*

<br/>

**Dataset Statistics**<br/>
---
| Dataset                  | Agree | Disagree | Neutral |  Total  |
| ------------------------ | ----- | -------- | ------- | ------- |
| SubReddit-MaskMandate    |  645  |   546    |   343   |   1534  |
| SubReddit-CovidVaccine   |  272  |   425    |   703   |   1400  |

<br/>

**Annotation Guideline**<br/>
---
Every *(Quote, Response)* pairs are annotated with one of *Agreement*, *Disagreement*, and *Neutral* labels:
* ***Agreement:*** both *Quote* and *Response* express subjective opinions towards some topics instead of sharing objective experience or giving objective advice, and there is explicit or implicit evidence for agreement / support / semantically similarity.
* ***Disagreement:*** both *Quote* and *Response* express subjective opinions, and there is explicit or implicit evidence for disagreement / attack / denial / reject / challenge / semantically opposition.
* ***Neutral:*** *Quote* or *Response* is not expressing subjective opinions, or *Quote* and *Response* are stating quite different / unrelated things, or both *Quote* and *Response* express opinions but *Response* is expressing vague / not sure / weak agreement or disagreement, or partially agree partially disagree.

<br/>

**Citation**<br/>
---
If you use this dataset in your research, please refer to and cite:

Yuanyuan Lei and Ruihong Huang. 2022. Few-Shot (Dis)Agreement Identification in Online Discussions with Regularized and Augmented Meta-Learning. In Findings of the Association for Computational Linguistics: EMNLP 2022, pages 5581–5593, Abu Dhabi, United Arab Emirates. Association for Computational Linguistics.

@inproceedings{lei-huang-2022-shot,<br/>
$title = "Few-Shot (Dis)Agreement Identification in Online Discussions with Regularized and Augmented Meta-Learning",<br/>
    author = "Lei, Yuanyuan  and<br/>
      Huang, Ruihong",<br/>
    booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",<br/>
    month = dec,<br/>
    year = "2022",<br/>
    address = "Abu Dhabi, United Arab Emirates",<br/>
    publisher = "Association for Computational Linguistics",<br/>
    url = "https://aclanthology.org/2022.findings-emnlp.409",<br/>
    pages = "5581--5593",<br/>
    abstract = "Online discussions are abundant with opinions towards a common topic, and identifying (dis)agreement between a pair of comments enables many opinion mining applications. Realizing the increasing needs to analyze opinions for emergent new topics that however tend to lack annotations, we present the first meta-learning approach for few-shot (dis)agreement identification that can be quickly applied to analyze opinions for new topics with few labeled instances. Furthermore, we enhance the meta-learner{'}s domain generalization ability from two perspectives. The first is domain-invariant regularization, where we design a lexicon-based regularization loss to enable the meta-learner to learn domain-invariant cues. The second is domain-aware augmentation, where we propose domain-aware task augmentation for meta-training to learn domain-specific expressions. In addition to using an existing dataset, we also evaluate our approach on two very recent new topics, mask mandate and COVID vaccine, using our newly annotated datasets containing 1.5k and 1.4k SubReddits comment pairs respectively. Extensive experiments on three domains/topics demonstrate the effectiveness of our meta-learning approach.",<br/>
}


