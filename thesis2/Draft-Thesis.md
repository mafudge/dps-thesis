---
title: '[]{#_z65zo811j5e0 .anchor}📚 Draft-Thesis'
---

Abstract
========

Large Language Models (LLMs) represent a disruptive innovation in
programming education, acting as both a supportive tutor and a tool for
cognitive offloading. This study investigated how specific student
engagement patterns influence learning performance and computational
literacy. Utilizing a multi-method design, interaction LLM trace data
from an introductory Python course were categorized into adaptive
(learning) and maladaptive (task-completion) help-seeking behaviors.
Quantitative analysis revealed a mutual suppression effect: aggregate AI
usage volume was an unreliable predictor of success, whereas engagement
type was highly significant.

Findings indicated that task-completion behaviors negatively predicted
midterm exam scores and computational literacy gains. Conversely,
learning-oriented sessions positively correlated with exam performance.
Furthermore, a randomized controlled trial demonstrated that
context-aware AI significantly improved learning outcomes when
controlling for usage patterns, acting as a performance multiplier.
These results underscore an urgent need for pedagogical adaptation,
shifting from policing AI to empowering students as sophisticated,
adaptive, and metacognitively aware users of generative technology.

*Keywords:* Large Language Models, Help-Seeking Behavior, Computational
Literacy, Programming Education, In-Context Learning, and Suppression
Analysis.

**Help-Seeking Behaviors in AI-Mediated Programming:\
Impacts on Performance and Computational Literacy**

By

Michael A. Fudge, Jr.

B.S.,Oswego State University, 1993

M.S., Syracuse University, 2006

Thesis\
Submitted In partial fulfillment of the requirements for the degree of
Doctor of Professional Studies in Information Management

Syracuse University\
May 2026

Copyright © Michael A. Fudge, Jr. 2025\
All Rights Reserved

Acknowledgements
================

Pursuing a Doctorate has been an adventure. Like every adventure there
are highs, lows, moments of clarity, moments of confusion, moments of
confidence and moments of doubt. I have grown so much as an academic
these past few years, and there are many individuals to acknowledge;
Those who helped with each of those moments.

I am thankful for the support of my advisors, Dr. Bei Yu, Dr. Jeffrey
Stanton, and Dr. John Jordan. Each of you helped me along on this
journey by sharing your wisdom and expertise. You let me *explore* the
phenomena I see in the classroom everyday and helped me to materialize
it into this thesis.

I am thankful for my classmates. You were there to share in the highs,
listened to me complain during the lows, and always provided an
empathetic ear. I cannot imagine completing this program without you
all.

I'd like to acknowledge my friends and family. While many of you don't
quite get what I'm trying to accomplish in this thesis, that didn't stop
you from lending an attentive ear.

Most importantly, I would like to thank my loving wife Kim for her
persistence, patience and unwavering support throughout my Doctoral
journey, and my dog, Luna who is always ready to provide unconditional
love.

Contents
========

[**Abstract 1**](#abstract)

[**Acknowledgements 4**](#acknowledgements)

[**Contents 5**](#contents)

[**List of Figures 8**](#list-of-figures)

[**List of Tables 9**](#list-of-tables)

[**1.0 Introduction 1**](#introduction)

> [1.1 Background 1](#background)
>
> [1.2 Problem Statement 3](#problem-statement)
>
> [1.3 Purpose of the Study 6](#purpose-of-the-study)
>
> [1.4 Significance of the Study 7](#significance-of-the-study)
>
> [1.5 Thesis Organization 8](#thesis-organization)

[**2.0 Literature Review 9**](#literature-review)

> [2.1 Rise of the Large Language Model (LLM)
> 10](#rise-of-the-large-language-model-llm)
>
> [2.2 LLMs as a Disruptive Innovation for software development
> 11](#llms-as-a-disruptive-innovation-for-software-development)
>
> [2.2.1 Impacts on Developer Productivity
> 13](#impacts-on-developer-productivity)
>
> [2.2.2 Conversations on the Future of Programming
> 14](#conversations-on-the-future-of-programming)
>
> [2.3 Large-Language Model use in Higher Education
> 14](#large-language-model-use-in-higher-education)
>
> [2.4 LLM Use in Programming Education
> 16](#llm-use-in-programming-education)
>
> [2.4.1 Framing Novices and Programming Difficulties
> 16](#framing-novices-and-programming-difficulties)
>
> [2.4.2 Studies of LLM Use in Programming Courses
> 17](#studies-of-llm-use-in-programming-courses)
>
> [2.5 LLM Impacts on Computer Programming Education
> 20](#llm-impacts-on-computer-programming-education)
>
> [2.5.1 Computational Thinking 20](#computational-thinking)
>
> [2.5.2 Self-Efficacy 22](#self-efficacy)
>
> [2.5.3 Help-Seeking Behavior 23](#help-seeking-behavior)
>
> [2.5.4 Academic Performance 25](#academic-performance)
>
> [2.6 Summary 27](#summary)
>
> [2.6.1 Duality of LLM Use 27](#duality-of-llm-use)
>
> [2.6.2 Mechanisms by Which LLM Use Impacts Learning
> 28](#mechanisms-by-which-llm-use-impacts-learning)
>
> [2.6.3 Research Rationale and Gap Statement
> 28](#research-rationale-and-gap-statement)

[**3.0 Methods 29**](#methods)

> [3.1 Introduction 29](#introduction-1)
>
> [3.1.1 Research Questions 30](#research-questions)
>
> [3.2 Study Design 31](#study-design)
>
> [3.2.1 Overview 32](#overview)
>
> [3.2.2 Participant Funnel 35](#participant-funnel)
>
> [3.2.2.1 Population 1: Chatbot participants
> 36](#population-1-chatbot-participants)
>
> [3.2.2.1 Population 2: Chatbot participants with Survey Responses
> 36](#population-2-chatbot-participants-with-survey-responses)
>
> [3.2.3 Computational Literacy Instrument (C1/C2)
> 37](#computational-literacy-instrument-c1c2)
>
> [3.2.4 Chatbot Design 39](#chatbot-design)
>
> [3.2.4.1 LLM Selection 39](#llm-selection)
>
> [3.2.4.2 Random Assignment 40](#random-assignment)
>
> [3.2.4.3 Control Group (T1) 41](#control-group-t1)
>
> [3.2.4.4 Treatment Group (T2) 42](#treatment-group-t2)
>
> [3.2.5 Midterm Exam (E1) 43](#midterm-exam-e1)
>
> [3.2.6 Questionnaire (Q1) 44](#questionnaire-q1)
>
> [3.2.7 Chatbot Trace Data (D1) 45](#chatbot-trace-data-d1)
>
> [3.3 Data Analysis 47](#data-analysis)
>
> [3.3.1 Overview 47](#overview-1)
>
> [3.3.2 Tools 48](#tools)
>
> [3.3.3 Operationalizing D1 Chatbot Trace Data
> 49](#operationalizing-d1-chatbot-trace-data)
>
> [3.3.4 Model Selection Reliability Testing
> 51](#model-selection-reliability-testing)
>
> [3.3.5 Categorical Content Analysis 53](#categorical-content-analysis)
>
> [3.4 Hypothesis Formulation and Methodology
> 54](#hypothesis-formulation-and-methodology)
>
> [3.4.1 RQ1 Hypothesis and Methodology
> 54](#rq1-hypothesis-and-methodology)
>
> [3.4.2 RQ2 Hypothesis and Methodology
> 56](#rq2-hypothesis-and-methodology)
>
> [3.4.3 RQ3 Hypothesis and Methodology
> 58](#rq3-hypothesis-and-methodology)
>
> [3.4.4 Satisfying Assumptions of Linear Regressions
> 60](#satisfying-assumptions-of-linear-regressions)

[**4.0 Results 61**](#results)

> [4.1 Introduction 61](#introduction-2)
>
> [4.2 Findings for RQ1 63](#findings-for-rq1)
>
> [4.2.1 Model Overview for RQ1 63](#model-overview-for-rq1)
>
> [4.2.2 Regression Assumption Tests of the Model for RQ1
> 64](#regression-assumption-tests-of-the-model-for-rq1)
>
> [4.2.3 Hierarchical Regression Analysis for the RQ1 Model
> 67](#hierarchical-regression-analysis-for-the-rq1-model)
>
> [4.2.3.1 Model 0: E1 \~ Session Count 68](#model-0-e1-session-count)
>
> [4.2.3.2 Model 1: E1 \~ Task Complection Session Count
> 69](#model-1-e1-task-complection-session-count)
>
> [4.2.3.3 Model 2: E1 \~ Learning Session Count
> 70](#model-2-e1-learning-session-count)
>
> [4.2.3.4 Model 3: E1 \~ Learning Session Count + Task Completion
> Session Count
> 71](#model-3-e1-learning-session-count-task-completion-session-count)
>
> [4.2.4 Summary of Findings for RQ1 72](#summary-of-findings-for-rq1)
>
> [4.2.5 Conclusion for RQ1 73](#conclusion-for-rq1)
>
> [4.3 Findings for RQ2 74](#findings-for-rq2)
>
> [4.3.1 Model Overview for RQ2 74](#model-overview-for-rq2)
>
> [4.3.2 Regression Assumption Tests for the RQ2 Model
> 75](#regression-assumption-tests-for-the-rq2-model)
>
> [4.3.3 Regression Analysis for the RQ2
> 76](#regression-analysis-for-the-rq2)
>
> [4.3.3.1 Model 1: Total Effect for RQ2
> 76](#model-1-total-effect-for-rq2)
>
> [4.3.3.2 Models 2 a/b: Mediation Analysis for RQ2
> 78](#models-2-ab-mediation-analysis-for-rq2)
>
> [4.3.3.3 Models 3 a/b: Moderation Analysis for RQ2
> 79](#models-3-ab-moderation-analysis-for-rq2)
>
> [4.3.3.4 Model 4: Identification of RQ2 Treatment Effect via
> Suppression Analysis
> 81](#model-4-identification-of-rq2-treatment-effect-via-suppression-analysis)
>
> [4.3.4 Summary of Findings for RQ2 83](#summary-of-findings-for-rq2)
>
> [4.3.5 Conclusion for RQ2 84](#conclusion-for-rq2)
>
> [4.4 Findings for RQ3 85](#findings-for-rq3)
>
> [4.4.1 Model Overview for RQ3 85](#model-overview-for-rq3)
>
> [4.4.2 Regression Assumption Tests for the RQ3 Model
> 87](#regression-assumption-tests-for-the-rq3-model)
>
> [4.4.3 Model 1: ANCOVA for RQ3 Accounting for Baseline Literacy
> 90](#model-1-ancova-for-rq3-accounting-for-baseline-literacy)
>
> [4.4.3.1 Model 1a: Supplementary Analysis Change in Scores
> 92](#model-1a-supplementary-analysis-change-in-scores)
>
> [4.4.4 Summary of Findings for RQ3 93](#summary-of-findings-for-rq3)
>
> [4.4.5 Conclusion for RQ3 94](#conclusion-for-rq3)
>
> [4.5 Overall Summary of Findings 95](#overall-summary-of-findings)

[**5.0 Summary 99**](#summary-1)

> [5.1 Introduction 99](#introduction-3)
>
> [5.1.1 Research and Key Findings At a Glance
> 99](#research-and-key-findings-at-a-glance)
>
> [5.2 Finding 1: The Essentiality of Usage Classification
> 100](#finding-1-the-essentiality-of-usage-classification)
>
> [5.2.1 Discussion of Finding 1 100](#discussion-of-finding-1)
>
> [5.2.2 Contextualization of Finding 1
> 102](#contextualization-of-finding-1)
>
> [5.3 Finding 2: The Negative Impact of Executive Help-Seeking
> 104](#finding-2-the-negative-impact-of-executive-help-seeking)
>
> [5.3.1 Discussion of Finding 2 104](#discussion-of-finding-2)
>
> [5.3.2 Contextualization of Finding 2
> 105](#contextualization-of-finding-2)
>
> [5.4 Finding 3: The Positive Impact of Adaptive Help-Seeking
> 106](#finding-3-the-positive-impact-of-adaptive-help-seeking)
>
> [5.4.1 Discussion of Finding 3 106](#discussion-of-finding-3)
>
> [5.4.2 Contextualization of Finding 3
> 107](#contextualization-of-finding-3)
>
> [5.5. Finding 4: The Efficacy of Context-Aware Scaffolding
> 108](#finding-4-the-efficacy-of-context-aware-scaffolding)
>
> [5.5.1 Discussion of Finding 4 108](#discussion-of-finding-4)
>
> [5.5.2 Contextualization of Finding 4
> 110](#contextualization-of-finding-4)
>
> [5.5 Implications and Recommendations
> 111](#implications-and-recommendations)
>
> [5.5.1 Theoretical Implications 111](#theoretical-implications)
>
> [5.5.2 Practical Implications for Instructors
> 113](#practical-implications-for-instructors)
>
> [5.5.3 Practical Implications for Institutions
> 114](#practical-implications-for-institutions)
>
> [5.5.4 Practical Implications for Students
> 115](#practical-implications-for-students)
>
> [5.6 Limitations 116](#limitations)
>
> [5.7 Future Research 117](#future-research)
>
> [5.8 Conclusion 119](#conclusion)

[**References 121**](#references)

 

List of Figures
===============

  3.1    An Overview of the Study Design                                                                                                                                                 32
  ------ ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- ----
  3.2    Context-Selection from the IST256 AI Tutor                                                                                                                                      34
  3.3    The treatment group (T2) is aware of the selected content                                                                                                                       35
  3.4    The Participant Funnel for Chatbot Use (n = 87)                                                                                                                                 36
  3.5    The Participant Funnel Integrating Survey Responses (n = 77)                                                                                                                    37
  3.6    A Sample Question from The CT-Test                                                                                                                                              39
  3.7    System Prompt Configuration for the Control Group (T1)                                                                                                                          42
  3.8    Treatment T2 Context Prompt Template                                                                                                                                            42
  3.9    AI Response to Context Selection in the Treatment Condition (T2)                                                                                                                43
  3.10   Distribution of Chat Session Classifications From the D1 Dataset                                                                                                                54
  4.1    Partial regression plots when holding the other constant of E1 \~ Task Completion Session Count + Learning Session Count                                                        65
  4.2    Residuals vs Fitted Values for E1 \~ Learning Session Count + Task Completion Session Count                                                                                     66
  4.3    Evidence of normality among the residuals of E1 \~ Task Completion Session Count + Learning Session Count                                                                       67
  4.4    Forestplot of E1 \~ Session Count                                                                                                                                               68
  4.5    Forestplot of E1 \~Task Completion Session Count                                                                                                                                69
  4.6    Forestplot of E1 \~ Learning Session Count                                                                                                                                      70
  4.7    Forestplot of E1 \~ Task Completion Session Count + Learning Session Count                                                                                                      72
  4.8    Evidence of normality among the residuals of E1 \~ Treatment                                                                                                                    76
  4.9    Forestplot of E1 \~ Treatment                                                                                                                                                   77
  4.10   Forestplot of E1 \~ Treatment + Learning Session Count + Task Completion Session Count                                                                                          82
  4.11   Partial regression plots when holding the other constant of C2 \~ Task Completion Session Count + Learning Session Count. + C1 with Visual Confirmation of Heteroscedasticity   88
  4.12   Residuals vs Fitted Values for C2 \~ Learning Session Count + Task Completion Session Count + C1                                                                                89
  4.13   Evidence of normality among the residuals of C2 \~ Task Completion Session Count + Learning Session Count + C1                                                                  90
  4.14   Forestplot of C2 \~ Learning Session Count + Task Completion Session Count + C1                                                                                                 92

 

List of Tables
==============

  3.1   Summary of Study Observations and Experimental Conditions                   32
  ----- --------------------------------------------------------------------------- ----
  3.2   Internal Consistency (Cronbach's Alpha) of the E1 Midterm Exam              44
  3.3   Fields in the D1 Chatbot Trace Data                                         45
  3.4   Codebook of Participant Behaviors in Trace Data (D1)                        49
  3.5   Krippendorff's Alpha for Inter-coder Reliability and Internal Consistency   52
  4.1   Hierarchical Model Comparison for RQ1                                       73
  4.2   Analytical Findings for RQ2                                                 83
  4.3   Summary of Findings for RQ3                                                 94

**1.0 Introduction**
====================

1.1 Background
--------------

Computer programming is undergoing a profound transformation. Large
Language Models (LLMs), a type of artificial intelligence (AI) trained
on vast amounts of textual data, have shown remarkable programming
capability. A recent study found that with guided prompts, the GPT-4 LLM
outperformed 85% of human programmers on online programming challenges
[(Hou & Ji, 2025)](https://www.zotero.org/google-docs/?6YpWOL).
Furthermore, a 2023 study from code management platform GitHub revealed
92% of U.S.-based developers use AI coding tools, with 70% saying they
offer advantages at work [(Github,
2023)](https://www.zotero.org/google-docs/?IozMez).

In early 2025, Andrej Karpathy tweeted about his experience engaging in
a conversation with AI to build software without focusing on the code
itself [(Andrej Karpathy,
2025)](https://www.zotero.org/google-docs/?jY3fat). He named this
activity *vibe coding*, which recently became the Collins Dictionary
2025 Word of the Year [(Collins,
2025)](https://www.zotero.org/google-docs/?d5OUI1). This has given rise
to numerous vibe coding platforms such as Base44[^1], Cursor[^2],
Lovable[^3], and Replit[^4] which are designed to build software through
human-AI exchanges. These platforms provide access to the expertise of
computer programming at a fraction of the time and cost of a human, a
disruptive innovation by C[hristensen's
(1997)](https://www.zotero.org/google-docs/?9k76gP) definition . These
disruptions are sparking conversations among academia and industry
suggesting that computer programming as traditionally understood is
facing obsolescence. From this shift, a new human-AI cooperative set of
skills centered on AI literacy and computational thinking is expected to
emerge [(Lohr, 2025; Stiffler,
2025)](https://www.zotero.org/google-docs/?fvLVoS).

For educators teaching introductory programming courses, this seismic
shift presents an immediate and critical tension. LLMs are
simultaneously capable of serving as both legitimate learning aids and
as a means to circumvent learning completely. On one hand, they promise
unparalleled support by functioning as a 24/7 tutor ready to explain
concepts, provide examples and offer debugging assistance in ways that
help students form deep connections necessary for learning [(Cambaz &
Zhang, 2024; Finnie-Ansley et al., 2022; Hassan et al., 2025; Prather et
al., 2019; Prather, Reeves, Leinonen, et al.,
2024](https://www.zotero.org/google-docs/?hzM9cH)). On the other hand,
their answer-generating capabilities foster learning-avoidance behaviors
and cognitive offloading. These activities undermine the fundamental
development of critical thinking and problem-solving skills [(Abbas et
al., 2024; Becker et al., 2023; Margulieux et al., 2024; Pons, 2023;
Rahman & Watanobe, 2023)](https://www.zotero.org/google-docs/?ydyyXS).

This thesis moves beyond the binary discourse of prohibition versus
acceptance of AI in programming education. Recognizing that generative
AI is an enduring fixture, it argues that educators, students, and
institutions must adapt. Furthermore, as LLMs function beyond simple
information retrieval, their generative capabilities hold significant
implications for cognitive engagement. To this end, this thesis
investigates empirically how LLMs are used by students in an
introductory computer programming course, focusing on the impacts that
use has on learning and computational literacy skill acquisition.

Introducing LLMs into programming education is analogous to giving
novice hikers a GPS for navigation. The LLM, like the GPS, can be used
in two ways. Hikers can use it as a tool to improve their ability to
scout routes and survey the land around them. This represents the
learning-focused ways the student can use an LLM to become a better
programmer. In this scenario, the tool used ultimately improves the
skill of its user. Alternatively, a hiker can use the GPS to tell them
exactly how to get to a destination. This parallels the task-completion,
answer-seeking behaviors of students learning to code. The short-term
goals are met: a novice programmer completes their assignment, and the
novice hiker arrives at their destination. However, due to heavy
reliance on the tool, they fail to build the essential skills necessary
to become self-sufficient. It is hoped that the findings from this
thesis will encourage other academics teaching computer programming to
not only rethink how we teach this subject but also identify which
skills are necessary for future programmers in the age of AI.

1.2 Problem Statement
---------------------

While use of Large Language Models (LLMs) as an aid for computer
programming is becoming well established in practice, researchers are
only beginning to understand their impacts on computer programming
education. This has profound implications for how we best educate the
programmers of the future. Current academic literature presents several
limitations and inconsistencies regarding LLM use by novices in
programming education revealing three specific gaps.

First, research is inconsistent concerning whether use of AI coding
assistants is a benefit or harm to individuals learning to program. Some
studies suggest AI-assisted programming, or "copilots," are an asset for
less experienced programmers ([Moradi Dakhel et al., 2023; Peng et al.,
2023)](https://www.zotero.org/google-docs/?YZTJhA) making them more
productive. For instance, [Kazemitabaar et al.
(2023)](https://www.zotero.org/google-docs/?SPCcnb) found that students
using AI for coding completed programming tasks more quickly. However,
this productivity may negatively impact learning, particularly for
novices who may lack the expertise to detect flaws in generated code
([Moradi Dakhel et al., 2023; Peng et al.,
2023)](https://www.zotero.org/google-docs/?vfx5AV). While studies have
focused on identifying behavioral AI usage patterns among participants
[(Becker et al., 2023; Prather, Reeves, Leinonen, et al.,
2024)](https://www.zotero.org/google-docs/?KLJ13A), empirical consensus
on the education value of these tools remains elusive.

Second, while several studies highlight the drawbacks of LLM use among
novice programmers, specifically how it fosters learning avoidance and
cognitive offloading [(Abbas et al., 2024; Becker et al., 2023;
Margulieux et al., 2024; Pons, 2023; Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?jQZcQw), little research has
directly explored AI\'s impacts on academic performance and
computational literacy skill acquisition. Furthermore, prior work
correlating AI use and final grades often relied on self-reported
frequency surveys [(Jošt et al.,
2024a)](https://www.zotero.org/google-docs/?18I1T4). This points to an
opportunity to explore the impact of LLM use through more unobtrusive
methods, such as the analysis of direct student interactions via log
analysis.

Finally, research on student help-seeking behaviors using LLM assistants
has been largely descriptive, establishing categories like "asking
questions" or "requesting code assistance" [(Kazemitabaar et al.,
2024)](https://www.zotero.org/google-docs/?nWNhLK). This leaves gaps in
exploring the implications of these help-seeking behaviors (adaptive vs.
maladaptive) on specific student outcomes like course performance and
computational literacy gains. Specifically, the relationship between
task completion behaviors and the fundamental development of
computational literacy is still emerging presenting the opportunity to
measure this relationship using a formalized computational thinking
assessment [(Román-González et al.,
2017)](https://www.zotero.org/google-docs/?gFbxqS).

The central problem motivating this thesis is to address the lack of
empirical understanding among LLM use and its impacts on student
outcomes and computational literacy. This research explores the
phenomenon through two distinct lenses. The first is the theoretical
lens of help-seeking behavior. Help seeking can be defined as the
actions a learner takes to get assistance with a problem. [Nelson-Le
Gall, (1981](https://www.zotero.org/google-docs/?SDaDS2)) identified two
distinct forms of help seeking behavior: Instrumental help-seeking, an
active, complex process key to learning; and executive help seeking,
defined as seeking to complete the task without further interest in
understanding it. Later, research by [Newman
(1994)](https://www.zotero.org/google-docs/?mXTAFb) framed help-seeking
behavior within the Self-Regulated Learning (SRL) theory as an adaptive
process, categorizing Nelson-Le Gall's definitions into adaptive and
maladaptive help-seeking behaviors.

For data analysis, this thesis classifies student chat interactions with
the LLM into two distinct categories: learning sessions and
task-completion sessions. In learning sessions, the participant shows
evidence of interacting with the LLM to understand or clarify---an
adaptive help-seeking strategy. In task-completion sessions,
participants use the LLM for executive help-seeking behavior, such as
having the AI do the work on their behalf. This study utilizes trace
interactions of participants using an LLM and correlates those usage
patterns with midterm grades and computational literacy skill
acquisition.

The second research lens focuses on the impact of context-aware LLMs on
learning. A significant barrier identified in the literature is that
novices struggle with formulating effective prompts [(Hsu, 2025; Wang et
al., 2024)](https://www.zotero.org/google-docs/?fk8vBn). Without precise
prompting, students risk receiving unhelpful generations or
misinterpretations of their intent. In-context learning offers a
solution to this deficit: by embedding contextual information such as
the assignment instructions directly into the system, the LLM is steered
toward generating more relevant and accurate answers. This scaffolding
compensates for the novice\'s lack of prompting expertise, a benefit
supported by recent findings [(Becker et al., 2023; Moradi Dakhel et
al., 2023)](https://www.zotero.org/google-docs/?psqK4P).

Studying the impacts of generative AI use on learning to program is a
highly relevant topic due to the potential academic and practical
consequences. Foremost is the risk to foundational skills. Without an
understanding of the mechanisms through which LLM use impacts learning,
educators in computing risk adopting policies such as banning AI use in
the classroom [(Lau & Guo,
2023)](https://www.zotero.org/google-docs/?9evjOA). Considering the
benefits of AI as an always-available educational resource, banning may
have negative effects on learning and computational literacy skill
acquisition, two factors this study explicitly measures. Secondly,
human-AI cooperation in software development is already happening
[(GitHub, 2023)](https://www.zotero.org/google-docs/?ybehTc). Students
entering the field as computer, data, or information scientists must be
experienced in using AI for cooperative programming [(Lohr, 2025;
Stiffler, 2025)](https://www.zotero.org/google-docs/?JEpfTF). This
thesis proposes that it is better to understand usage behaviors and
devise mechanisms for fostering supportive learning behaviors while
discouraging negative ones. This approach allows instructors in
computing, and perhaps beyond, to rethink their pedagogy by positioning
AIs such as LLMs as effective and adaptive learning aids.

1.3 Purpose of the Study
------------------------

The goal of this study was to empirically understand how different
patterns of LLM engagement impact the learning and skill development of
novice programmers, as measured through their computational literacy.
Additionally, the study sought to understand the relationship between
context-aware LLMs and learning through a randomized controlled trial.
This study employed a systematic plan of action to capture, classify,
and quantify the relationship between LLM use and measurable academic
outcomes. The specific objectives were:

1.  To capture participant interactions with an LLM through trace data,
    > and then conduct a categorical content analysis on participant
    > sessions to quantify the interactions as either task-completion
    > focused (maladaptive help-seeking), learning focused (adaptive
    > help-seeking) or neither.

2.  To analyze the relationship between these quantified LLM use
    > patterns and student learning performance and computational
    > literacy. Learning was measured post-intervention through midterm
    > exam scores (E1), while skill acquisition was measured through a
    > post-intervention computational literacy instrument (C2),
    > controlling for baseline ability with a pre-intervention pretest
    > (C1).

3.  To determine the causal impact that the in-context learning
    > capabilities of an LLM have on student learning performance (E1).
    > In the treatment group, the LLM prompt was adjusted to include
    > assignment instructions, making it capable of generating
    > context-aware responses. Consequently, students in the treatment
    > group did not need to ask specific, detailed questions for the LLM
    > to elicit a contextual response.

The research questions guiding this study were derived directly from the
knowledge gaps identified in the current academic literature concerning
LLM use by novices in programming education.

• RQ1: How does Large Language Model (LLM) use influence student
learning performance?

◦ Approach: This was addressed by quantifying usage patterns (learning
sessions vs. task completion sessions) and correlating them with midterm
exam scores (E1).

• RQ2: When the prompt is adjusted to include assignment instructions
(in-context learning) what is the impact on student learning
performance?

◦ Approach: This utilized a randomized controlled trial comparing
context-aware AI (treatment T2) versus non-context-aware AI (control
T1).

• RQ3: What is the relationship between Large Language Model (LLM) use
and computational literacy?

◦ Approach: This was addressed using a pretest-posttest design (C1/C2)
with a formalized computational thinking assessment [(Román-González et
al., 2017)](https://www.zotero.org/google-docs/?fRdurf)..

By addressing these questions, this thesis aims to provide the empirical
evidence necessary for educators to refine computer programming pedagogy
and identify the essential skills required for future programmers in the
age of AI.

1.4 Significance of the Study
-----------------------------

This work advanced theoretical and conceptual understanding in computing
education and learning sciences. It provided empirical evidence for the
distinction between beneficial and detrimental LLM usage patterns. While
patterns such as answer-seeking [(Finnie-Ansley et al., 2022; Hassan et
al., 2025)](https://www.zotero.org/google-docs/?JUCZkh), cognitive
offloading for task completion [(Margulieux et al., 2024; Prather,
Reeves, Leinonen, et al.,
2024)](https://www.zotero.org/google-docs/?LqnMNM), scaffolding [(Hassan
et al., 2025; Prather et al., 2019; Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?i08f1z) and questioning
[(Cambaz & Zhang, 2024; Finnie-Ansley et al.,
2022)](https://www.zotero.org/google-docs/?eePwvg) were observed in
prior research, this study anchored these behaviors within established
help-seeking theory.

The study explored the impacts of LLM use not only on learning but also
on the development of the abstract problem-solving abilities essential
for computational literacy. A significant contribution of this work was
demonstrating the importance of accounting for competing behaviors when
modeling these impacts. Specifically, including both adaptive and
maladaptive help-seeking behaviors in the model helped explain the
effects on learning and computational literacy more effectively than
examining each individually. This finding extends existing help-seeking
research by [Kazemitabaar et al.,
(2024)](https://www.zotero.org/google-docs/?R0Y2yy) and [Sheese et al.,
(2024)](https://www.zotero.org/google-docs/?DLbiIR).

1.5 Thesis Organization
-----------------------

After the introduction, the supporting work from this thesis is
organized into four chapters. Each subsequent chapter builds upon the
previous ones to outlay the lens through which this research is
grounded, the methods by which the study was conducted, the key findings
and the implications of those findings. A summary of each chapter is
outlined in as follows:

  Chapter                 Summary
  ----------------------- ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
  1.0 Introduction        The introduction provides the necessary framing for this study, including motivation, key research questions and approaches to answering them.
  2.0 Literature Review   This chapter investigates the current and relevant literature on Large-Language Models through the lens of how they are transforming work, education, and then specifically programming education. LLM impacts are then studied through 4 research lenses: computational thinking, self-efficacy, help-seeking behavior and academic performance.
  3.0 Methods             The methods chapter formulates hypotheses from the research questions and structures the methodologies to address them. There is a detailed explanation of the study design and an outline of the methodological analysis to operationalize the data collected from the study.
  4.0 Results             This chapter outlines the findings from the study\'s findings. The results are structured by research questions since each question employs a different method of analysis.
  5.0 Summary             The summary section synthesizes the results from the previous chapter into findings, which are then contextualized within the academic literature. A discussion includes the implications of the findings, limitations, and areas for future research.

**2.0 Literature Review**
=========================

The following literature review presents the necessary background to
better understand Large Language Models (LLMs) and their impacts on how
novice programmers learn to code. I begin by exploring key research
around LLMs and how they have impacted disciplines since their
inception. Specifically, I provide evidence of LLMs as a disruptive
innovation in the field of computer programming. LLMs have transformed
not only how people code but also how programmers think about
programming itself. This has implications for not only how code will be
written in the future, but what skills are necessary for becoming a
programmer and the methods by which those skills are taught to novices.

In addition, this literature review will explore the research of LLM use
by teachers, students, and administration within higher education. The
research embodying the strengths, drawbacks, and unique challenges of
LLMs within this context is discussed. This is necessary to
differentiate between the overarching issues of LLMs in education and
those specific to the topic of computer programming education.

Research shows LLMs are transforming how skilled professionals write
code. LLMs are being used predominantly by teachers and students in
computer programming education as well, which has forced academics to
rethink not only how to teach computer programming to novices, but also
what should be taught in the first place. The literature will identify
this through the positive and negative impacts LLMs are having on
programming education.

The academic literature on computer science education discusses the
well-known challenges of novice users learning to program. These
challenges are the impacts of cognitive load on learning, getting
learners to focus on computational literacy over syntax and technology,
the role of self-efficacy and motivation on success, and the importance
of metacognition for building problem-solving skills. This literature
review will revisit each of these challenges through the lens of how
LLMs are impacting them both positively and negatively.

2.1 Rise of the Large Language Model (LLM)
------------------------------------------

Natural Language Processing (NLP) has undergone significant changes in
recent years. With the introduction of transformer-based neural network
architecture, Natural Language Processing took a giant step forward in
performance and accuracy [(Gillioz et al.,
2020)](https://www.zotero.org/google-docs/?8jjxZA).

The Generative Pre-Trained Transformer (GPT) reasonably predicts the
next word in a sequence using the input and previously generated output.
While predicting the next token in the sequence is the extent of their
ability [(Shanahan, 2024)](https://www.zotero.org/google-docs/?e7ZTju),
transformer-based language models trained on large data have
demonstrated highly effective reasoning capabilities.

OpenAI\'s foundational paper, \"Language Models are Few-Shot Learners\",
demonstrated that these transformer-based language models, when trained
on large corpora, demonstrated highly effective reasoning capabilities
[(Brown et al., 2020)](https://www.zotero.org/google-docs/?9CR2N9).
In-context learning, as it was referred to, was a pivotal discovery
because prior to this paper transformer-based models were trained to be
relatively task specific [(Zhao et al.,
2023)](https://www.zotero.org/google-docs/?Fu23s5). Follow-up research
by [Min et al., (2022)](https://www.zotero.org/google-docs/?bDOTgc) and
[Akyürek et al. (2022)](https://www.zotero.org/google-docs/?qgUVXw)
investigated the mechanisms behind the effectiveness of in-context
learning.

The paper from [Brown et al.
(2020](https://www.zotero.org/google-docs/?cccr3c)) led to significant
advancements in research with respect to understanding the capabilities
of LLMs, and identifying new ways to apply them. [Wei et al.
(2022)](https://www.zotero.org/google-docs/?BqrLlH) discovered the
reasoning capabilities of LLMs can be improved through a technique
called chain-of-thought prompting. By including few-shot examples that
break down complex reasoning into steps, the LLM can use those shots
provided as an example of how to explain or execute a complex process.

[Halevy et al.'s (2009)](https://www.zotero.org/google-docs/?sIUJsR)
seminal paper, "The unreasonable effectiveness of data," explains that
as the training data set size increases, so does the model accuracy. In
addition, the specific selected model algorithm becomes less relevant as
training data set size increases. [Wei, Bosma, et al.
(2022)](https://www.zotero.org/google-docs/?gEbEyt) documented a similar
effect with large language models. Larger-sized models exhibited
emergent abilities not found in their smaller counterparts. Examples of
emergent abilities seen in the larger models include complex arithmetic
and reading comprehension, and new capabilities seem to emerge with each
subsequent release.

2.2 LLMs as a Disruptive Innovation for software development
------------------------------------------------------------

[Christensen et al. (2018)](https://www.zotero.org/google-docs/?xFDXCJ)
divide technological innovations into two distinct types. Sustaining
innovations improve existing products and services, while disruptive
innovations provide a unique set of features to an initial set of
customers. From the perspective of companies that offer generative AI
such as Google, Anthropic, OpenAI, and Microsoft, Horn considers
generative AI to be a sustaining innovation [(Horn,
2024)](https://www.zotero.org/google-docs/?xCIUps). In their
comprehensive literature review of AI as a disruptive innovation,
[Păvăloaia and Necula
(2023)](https://www.zotero.org/google-docs/?45LH9g) consider the
application of Generative AI to be a disruptive innovation across
different sectors such as healthcare, agriculture, business, and
education.

One domain being transformed by LLMs is computer programming. This is
not without precedent. Using computers as a tool for the generation of
code has been a decades-old objective of the Artificial Intelligence
community [(Manna & Waldinger,
1971)](https://www.zotero.org/google-docs/?ypc2If). While initial models
such as pyMT5 and CodeBERT did not perform well enough for practical
use, that changed with OpenAI\'s Codex large language model trained on
code available from GitHub [(Chen et al.,
2021)](https://www.zotero.org/google-docs/?zX8919).

The rise of AI-assisted programming tools from industry provides
evidence of this disruption. There is an ever-growing set of
cloud-enabled AI programming assistants such as: Github Copilot[^5],
Amazon Kiro[^6], Google Antigravity[^7], Claude Code[^8], and OpenAI
Codex[^9]. While each provides a unique set of features for
differentiation, they all share primary functions such as code
completion, code generation, code explanations, code debugging and
discussion of code. The primary value-add touted by these tools is
developers will be able to write code in less time, improving
productivity. Vibe-coding platforms such as Lovable, Base44, Replit, and
Cursor, take AI code generation to the extreme allowing their users to
build complete software applications through human-AI interactions with
no coding experience necessary. These platforms are often criticized for
their implementation fragility and contributions to technical debt
acceleration in the projects employed by its users [(Maes,
2025)](https://www.zotero.org/google-docs/?QifN3l).

### 2.2.1 Impacts on Developer Productivity

Despite AI-assisted programming tools being a recent development, there
have been studies of their impact on developer productivity already.
Studies by [Ziegler et al.
(2022)](https://www.zotero.org/google-docs/?9NmgER), [Moradi Dakhel et
al. (2023)](https://www.zotero.org/google-docs/?CnR9Oq), and [Peng et
al. (2023)](https://www.zotero.org/google-docs/?Uaotg7) all concluded
that AI programming assistants increase developer productivity. In their
controlled experiment of GitHub Copilot, Peng et al. measured a 55.8%
increase in developer productivity measured as the time it took
participants to complete a specific programming task [(Peng et al.,
2023)](https://www.zotero.org/google-docs/?xDm6IM). [Vaithilingam et
al., (2022)](https://www.zotero.org/google-docs/?0vV8lO) performed a
similar study and did not observe a measured increase in productivity as
measured in time to complete a task; however, there was a preference
among study participants to use GitHub Copilot.

There were even mixed findings among two of the studies which cited
gains in developer productivity. [Moradi Dakhel et al.
(2023)](https://www.zotero.org/google-docs/?EDECmE) suggested copilots
are an asset for advanced-level programmers, yet a liability for novice
programmers because novice programmers may not have the capability to
detect potential flaws in the AI-generated code. This conclusion
contradicts [Peng et al.'s
(2023)](https://www.zotero.org/google-docs/?wUfp0C) findings that less
experienced programmers benefit from the assistance of copilot.

A case study by IBM research of engineers using Watson Code Assistant
(WCA) concluded code understanding as a top use case as opposed to code
generation, pointing to the complexity of the code being developed as
the reason. Developers cited productivity benefits completing code tasks
due to AI explaining complex code, yet expressed concerns over the
accuracy of AI code generations in addition to concerns over deskilling
from overreliance [(Weisz et al.,
2025)](https://www.zotero.org/google-docs/?aSjwfg).

### 2.2.2 Conversations on the Future of Programming

Productivity gains from AI programming assistants can be considered a
form of human augmentation (Klinova & Korinek, 2021). These assistants
undoubtedly improve the capabilities of their human counterparts through
code generations [(Peng et al.,
2023)](https://www.zotero.org/google-docs/?iBBj5L), debugging
[(Chinthapatla, 2024)](https://www.zotero.org/google-docs/?FktbgO), and
code explanations [(Weisz et al.,
2025)](https://www.zotero.org/google-docs/?EYYJut).

There are varying opinions on the likely impact AI will have on the
future of programming. According to Ernst and Bavota (2022)m it will
take time for these tools to mature and develop, but they are not likely
to be the solution to the key challenges of software development.

Other scholars believe computer programming as it is currently
understood and practiced is headed on the path to extinction. Software
developers will develop a new set of skills such as evaluating
AI-generated code outputs, understanding how to engineer prompts, and
exploring unexplainable code outputs (Ebert & Louridas, 2023). Welsh
believes the software developer role will be replaced with a dialogue
between AI and human (Welsh, 2023), although according to [Maes
(2025)](https://www.zotero.org/google-docs/?G5PwJm), the current state
of these platforms lacks sound software engineering principles necessary
to materialize this capability.

2.3 Large-Language Model use in Higher Education
------------------------------------------------

Large Language Models are also transforming higher education. These
tools, used by both teachers and students, offer significant value yet
also have some key drawbacks. This section will focus on the state of
research in this area but will omit specifics regarding how LLMs are
used for teaching computer programming. This is the foundation of the
next section.

The literature indicates teachers use large language models to support a
variety of activities. To support teaching, LLMs are used for lesson
planning and course material creation [(Holmes & Tuomi, 2022; Kasneci et
al., 2023; Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?ZOTHga), in addition to
creating assessments, rubrics, and homework exercises [(Holmes & Tuomi,
2022; Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?2N17BC). Teachers have also
used LLMs to evaluate student performance and provide feedback on
student work [(Kasneci et al., 2023; Rudolph et al.,
2023)](https://www.zotero.org/google-docs/?rJKhz8). [Rahman & Watanobe,
(2023)](https://www.zotero.org/google-docs/?rzmDbc) suggest LLMs can be
used for plagiarism detection.

As expected, there are significant drawbacks to LLM use in education.
The content used to train the model itself can lead to plagiarism,
copyright infringement, and other academic integrity issues [(Holmes &
Tuomi, 2022; Kasneci et al., 2023; Olga et al., 2023; Rahman & Watanobe,
2023; Rudolph et al.,
2023)](https://www.zotero.org/google-docs/?r3dOHT). This is compounded
by the fact that the LLM statistically buries the sources used to
generate content by design and therefore the output has no factual
grounding [(Olga et al., 2023; Rudolph et al.,
2023)](https://www.zotero.org/google-docs/?bf1SmH). Students do not have
a source to cite for the information generated by the model.

The Large Language Models themselves are prone to bias based on the
underlying data on which they were trained [(Allam et al., 2023;
Baidoo-Anu & Owusu Ansah, 2023; Kasneci et al., 2023; Pons,
2023)](https://www.zotero.org/google-docs/?6qAMpz). In addition, the
very nature of how generative AI works leads to hallucinations where the
LLM statistically strings together coherent output which is not based on
facts [(Allam et al., 2023; Baidoo-Anu & Owusu Ansah, 2023; Pons,
2023)](https://www.zotero.org/google-docs/?0oprZu). Baidoo-Anu and Owusu
Ansah (2023) and [Shanahan,
(2024)](https://www.zotero.org/google-docs/?M9SLEd) claim that to use
LLMs effectively users must understand their intrinsics: their
capabilities and limitations so as not to anthropomorphize them.

Because it directly impacts learning, an impactful drawback of LLM use
by students is cognitive offloading. An overreliance on the AI
capabilities leads to a reduction in critical thinking, and a negative
impact on learning performance follows [(Abbas et al., 2024; Pons, 2023;
Rahman & Watanobe, 2023)](https://www.zotero.org/google-docs/?yM5t7W).
These concepts are explored further in the next section.

2.4 LLM Use in Programming Education
------------------------------------

We discussed LLM impacts on computer programming, and its impact on
higher education. Now we will explore the literature around LLM use in
programming courses as taught in higher education. This has been a
highly studied area in recent years [(Bang & Dang, 2024; Denny, Prather,
et al., 2024a; Prather et al., 2023; Shein,
2024)](https://www.zotero.org/google-docs/?11NCmM). In academic
literature, introductory programming courses are commonly called CS1
courses [(Hertz, 2010)](https://www.zotero.org/google-docs/?siDVR7).
Traditionally these courses introduce fundamental concepts of computing
to novice programmers, but as [Hertz
(2010)](https://www.zotero.org/google-docs/?aSziUi) discovered there is
a wide variance within the topics covered.

### 2.4.1 Framing Novices and Programming Difficulties

Novice students\' difficulties with learning to program have been well
studied [(Qian & Lehman,
2018)](https://www.zotero.org/google-docs/?eDnuBC). Early foundational
work by [DuBoulay (1989)](https://www.zotero.org/google-docs/?sdaMsP)
sought to classify the types of misconceptions students possess. There
were three types of misconceptions: having incorrect analogies,
overgeneralizing problems, and incorrect sequencing. These errors could
be syntactic, such as with a lack of understanding of the programming
language, or pragmatic where the student is not able to plan, debug, or
test their creations.

Later work from [McGill and Volet
(1997)](https://www.zotero.org/google-docs/?g4IRJp) led to a framework
for analyzing students\' knowledge of programming. Their framework
focused on three levels of programming knowledge: syntactic, conceptual,
and strategic. The authors further break up each type into declarative,
or understanding of the concept, versus procedural, or being able to
apply it.

In their literature review related to teaching and learning programming,
[Robins et al. (2003)](https://www.zotero.org/google-docs/?D47wmY)
identified two types of novice users: effective and ineffective.
Effective novices can learn with minimal effort as they experiment with
code and persist through errors. Ineffective novices tend to give up
quickly and only learn after significant effort and assistance. The
authors claim future research exploring the possibility of identifying
the key deficits of ineffective novices could help them become more
effective learners.

### 2.4.2 Studies of LLM Use in Programming Courses

Large language models fine-tuned using code samples can generate code
from user prompts. [Chen et al.
(2021)](https://www.zotero.org/google-docs/?89xSIy) performed seminal
research in this area, training the GPT-3 LLM on Python code. The model
was able to generate code from Docstrings (Python code comments). This
code generation has several benefits and drawbacks within the context of
teaching and learning programming. In this section we will synthesize
the literature around research in this area.

Several researchers see the code generation capabilities afforded by
large language models as a benefit to teachers and learners. Students
can ask the LLM to write code from a text prompt [(Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?Gi2Wsk). Students can engage
in conversations about their code [(Lau & Guo,
2023)](https://www.zotero.org/google-docs/?3MPXcg), helping them to get
started or unstuck on their assignments. Code generating capabilities of
LLMs help instructors create programming exercises with sample solutions
and test cases using one-shot learning examples although the exercises
did need some adjustments before they could be used [(Sarsa et al.,
2022)](https://www.zotero.org/google-docs/?mb1Oyc).

In a study by [Kazemitabaar et al.
(2023)](https://www.zotero.org/google-docs/?UyuCX0), students were asked
to complete various programming tasks. The population that used OpenAI
Codex for assistance showed an increase in task completion time and code
correctness, over the population that did not. Of the population using
Codex, students with higher pre-test scores were able to retain what
they learned as demonstrated on their post-test. There was no
statistical measurement of learning among the population of Codex
students who did not perform well on the pre-test, indicating this group
did not benefit from LLM use. Considering [Robins et al.
(2003)](https://www.zotero.org/google-docs/?FcuSVP) and their study on
effective and ineffective novices, future research could investigate
ways to improve learning among ineffective novices.

Using large language models to explain code has also been researched. At
the time of their study, [Sarsa et al.
(2022)](https://www.zotero.org/google-docs/?LMto62) discovered OpenAI
Codex could explain 90% of the lines of code among a sample of 20 Python
programs; however, the explanations provided were 67% correct. In
research by [Leinonen et al.
(2023)](https://www.zotero.org/google-docs/?OzQUGp) their thematic
analysis showed students preferred code explanations created by GPT-3,
citing them to be more accurate and easier to understand when compared
to those created by their peers. When considered together, these two
studies suggest LLMs are better at creating code explanations than
novice students.

Code-trained LLMs are effective at debugging code, and students have
used them to correct issues with their code [(Ghimire & Edwards, 2024;
Lau & Guo, 2023; Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?eWq6YR). In their study on
the effectiveness of GitHub Copilot at solving algorithmic problems such
as sorting or data structures, [Moradi Dakhel et al.
(2023)](https://www.zotero.org/google-docs/?7kWIDf) discovered Copilot
was more effective at debugging incorrect student code than debugging
its own incorrectly generated code. This is not surprising given the
confidentially incorrect nature by which large language models produce
their output [(Dinan, S.,
2023)](https://www.zotero.org/google-docs/?0ek3g8).

Despite their benefits, there are several challenges to incorporating
large language models trained using code into the classroom. Students
struggle to understand the code generated from tools like GitHub Copilot
[(Prather, Reeves, Leinonen, et al.,
2024)](https://www.zotero.org/google-docs/?qLls23). These findings are
understandable as education is not the primary market for these models,
and the prompts were not customized. Also, students struggle with
formulating a good prompt and thus the generated output is unhelpful or
misinterpreted [(Becker, 2023; Moradi Dakhel et al.,
2023)](https://www.zotero.org/google-docs/?6jifvT). Later studies
demonstrated the importance of teaching students how to prompt the AI
effectively [(Hsu, 2025; Wang et al.,
2024)](https://www.zotero.org/google-docs/?1YIjM1).

A concern among teachers that is noted in the literature focuses on the
coding style taught to novice programmers versus that which is seen on
the internet and therefore ingrained into the LLM. Oftentimes the code
generated by the LLM does not match the style taught in the course
[(Becker et al., 2023; Denny, Leinonen, et al., 2024; Lau & Guo,
2023)](https://www.zotero.org/google-docs/?usRg1o). This can confuse
students, lead to academic integrity issues, and make learning more
difficult as students fail to recognize differences in code structure or
understand the intention behind the code.

There is also the issue of code security. AI-generated code was found to
be less secure incorporating outdated practices [(Pearce et al., 2022;
Perry et al., 2023)](https://www.zotero.org/google-docs/?S9yA67). Novice
programmers, not aware of best practices in security, are unaware the
generated code does not follow these best practices.

LLMs are adequate at solving problems and answering questions typically
posed to students on exams and programming assignments in introductory
courses [(Finnie-Ansley et al., 2022; Rahman & Watanobe, 2023; Savelka,
Agarwal, Bogart, et al.,
2023)](https://www.zotero.org/google-docs/?7uAYil). While this can be
helpful as a study aid for students, when used inappropriately this can
cause academic integrity issues and invalidate assessments [(Denny,
Prather, et al., 2023; Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?kit1Q4). Researchers have
studied just how effective LLMs can be in completing the work of a
student. [Finnie-Ansley et al.
(2022)](https://www.zotero.org/google-docs/?YKl0ad) learned OpenAI Codex
was able to obtain a class ranking of 17 out of 71 on coursework. In
addition, the authors claimed it was difficult to evaluate whether AI or
the student generated the code. Another problem is that AI models get
better with each subsequent generation. In a study of multiple-choice
exam questions about Python programming, the GPT-3, GPT-3.5, and GPT-4
answered 37.5%, 64.3%, and 84.1% of questions correctly [(Savelka,
Agarwal, An, et al., 2023)](https://www.zotero.org/google-docs/?EbVy0Q).

Another major concern of LLM use for programming, especially among
novices, is overreliance. Repeated use of an LLM to provide the answers
reinforces behaviors detrimental to learning [(Becker et al., 2023;
Margulieux et al., 2024)](https://www.zotero.org/google-docs/?gz468Q).
Students may be too trusting of the code outputs, assuming it is correct
rather than critically evaluating whether the suggested code actually
solves the computational problem. This leads to poor metacognition,
hindering self-knowledge and self-understanding [(Denny, Prather, et
al., 2024a)](https://www.zotero.org/google-docs/?ahY9eu). This concern
is not only among educators. The students interviewed in the [Prather,
Reeves, Leinonen, et al.
(2024)](https://www.zotero.org/google-docs/?0g3Utb) study mentioned
concerns of their own overreliance on AI based on the ease and
convenience at which the model provided suggestions.

2.5 LLM Impacts on Computer Programming Education
-------------------------------------------------

This section explores the impacts of large language model use on key
theories and concepts associated with learning to program. There are
four main areas that will be discussed: computational thinking ability,
self-efficacy, help-seeking behavior, and learning performance.

Each area will begin with a discussion of the foundational literature,
then include specific framing as to why the theory is important within
the context of programming education. Next, academic literature that
studies the impact of large language models on the theory in question is
explored. Any gaps in literature or potential future areas of study will
be noted where appropriate, and the section will conclude by
synthesizing the current findings regarding LLM impacts on student
learning outcomes.

### 2.5.1 Computational Thinking

Cuny, Snyder, and Wing define computational thinking as \"the thought
processes involved in formulating problems and their solutions so that
the solutions are represented in a form that can be effectively carried
out by an information-processing agent\" [(Wing,
2011)](https://www.zotero.org/google-docs/?2n2owj). More than mere
problem-solving, computational thinking involves crafting a solution
that could be carried out systematically, as if by a machine. [Wing
(2008)](https://www.zotero.org/google-docs/?RMmtYB) argues computational
thinking will be essential to new discoveries in fields beyond computer
science and is therefore an essential skill for all disciplines.
Computational thinking aids in solving problems efficiently and
effectively, understanding complex systems, and modeling complex
systems.Computational thinking is essential to literacy and is therefore
a foundational element of K--12 learning [(Jacob et al.,
2018)](https://www.zotero.org/google-docs/?7D6iBq).

Computational literacy is not synonymous with computer programming. Wing
argues that researchers need to differentiate among the tools used to
reinforce the concepts and the concepts themselves [(Wing,
2008)](https://www.zotero.org/google-docs/?lBFy1y). In this regard,
programming languages like Python are analogous to a calculator, while
computational thinking is analogous to knowing math. Not all researchers
believe learning to program a computer is the best method to learn
computational thinking either, and other more abstract methods are
suggested [(Lu & Fletcher,
2009)](https://www.zotero.org/google-docs/?w9sGro).

Research into large language models for code generation and its impact
on computational literacy is in its early phases. [Denny, Kumar, et al.
(2023)](https://www.zotero.org/google-docs/?acybaU) explored the
performance of GitHub Copilot use on various programming problems. The
study suggests prompt engineering - the art of crafting inputs to elicit
a desired output - may become an activity that promotes computational
thinking skills. This concept was followed up by [Denny, Leinonen, et
al.'s (2024)](https://www.zotero.org/google-docs/?l7sY1D) paper titled
"Prompt problems: A new Programming Exercise for the Generative AI Era"
where they crafted a pedagogical approach to help students learn
effective AI prompting for problem-solving.

In an experimental design study of undergraduate students, [Yilmaz and
Karaoglan Yilmaz, (2023)](https://www.zotero.org/google-docs/?rTonVt)
found a statistically significant increase in students\' computational
thinking ability among the treatment group allowed to use ChatGPT.
Computational thinking ability was measured using the computational
thinking scale developed by [Korkmaz et al.,
(2017)](https://www.zotero.org/google-docs/?acAfkj). The population was
chosen from among students who were taking a programming course.
Students were not omitted from the study based on prior ability, so
these results corroborate with other research on these tools and their
benefit to experienced users.

[Korkmaz](https://www.zotero.org/google-docs/?3OIJcE)'s instrument
measures computational thinking on a scale, and is not an assessment. An
opportunity exists to study the impacts of Generative AI use on
computational thinking ability, in a pretest-posttest measure using a
validated computational thinking assessment such as the CT-test from
[Román-González et al.
(2017)](https://www.zotero.org/google-docs/?UzJXoY).

### 2.5.2 Self-Efficacy

Self-efficacy can be defined as the belief in one\'s capabilities to
succeed. [Bandura (1977)](https://www.zotero.org/google-docs/?Q9HHP4)
theorized our self-efficacy determines how we think, behave, and
self-motivate. Bandura claims self-efficacy plays a major role in how we
approach difficult challenges as it holds influence over our choices,
effort, persistence, and perseverance.

Self-efficacy theory has long been applied within the domains of health,
education, and athletics. It was first applied to computer use by
[Compeau and Higgins,
(1995)](https://www.zotero.org/google-docs/?7FYNcp). They found that
computer self-efficacy influences a user's expectations, emotions, and
engagement with technology. In addition, self-efficacy and outcome
expectations are positively shaped by peer behavior and encouragement
within workgroups.

Since learning to program is a form of education, studying the
self-efficacy of beginning programmers is sensible. There have been
several studies to this effect such as [Kinnunen and Simon
(2012)](https://www.zotero.org/google-docs/?YS1ttV) who found students
make self-efficacy assessments through the comparison of themselves to
their classmates. In their momentary study of self-efficacy and
affective experiences, [Lishinski and Rosenberg
(2021)](https://www.zotero.org/google-docs/?Rbo9b4) discovered novices'
early experiences can have a substantial impact on their attitudes
toward computing. These attitudes, in turn, shape future interest in
computing. A study across computer science students at three different
universities established a link between negative self-assessment and
lower self-efficacy [(Gorson & O'Rourke,
2020)](https://www.zotero.org/google-docs/?h3MTX7). Common themes among
these studies are students' negative assessment of self when dealing
with common programming challenges such as fixing errors, not knowing
how to start problems, and confidence in the correctness of their own
solutions.

Generative AI is good at debugging and code explanations. Therefore, it
seems reasonable to study the implications of self-efficacy when using
LLM to assist with coding tasks. There are indications that AI use may
amplify the gap between effective and ineffective novices. Results from
one study suggest that students with higher self-efficacy, lower fear of
failure, or higher prior grades tended to use AI less but more
effectively [(Margulieux et al.,
2024)](https://www.zotero.org/google-docs/?1T88Y6). Another study from
[Yilmaz and Karaoglan Yilmaz
(2023)](https://www.zotero.org/google-docs/?VipJcZ) indicates that
novice students may become overconfident and overreliant from use of AI.
This points to a gap in literature to study the relationship between
overconfidence and self-efficacy.

### 2.5.3 Help-Seeking Behavior

Prior to Sharon Nelson-Le Gall's seminal work on the subject, help
seeking was widely viewed as an undesirable behavior [(Nelson-Le Gall,
1981)](https://www.zotero.org/google-docs/?oLU7zJ). Help-seeking
behavior was perceived as symptomatic of weakness, immaturity, or
passivity. It was widely believed that the solitary, unaided completion
of tasks led to competence.

Nelson-Le Gall studied-problem solving skills in elementary school
children, and observed two distinct forms of help-seeking. Instrumental
help-seeking was defined as an active, complex social-cognitive activity
key to learning and achievement. On the other hand, executive
help-seeking represents the intention to have someone else achieve a
goal on behalf of the help-seeker. This was considered an undesirable
characteristic with negative long-term effects on learning.

Her contribution successfully reframed help-seeking not as a deficiency
but as an adaptive approach to managing challenges. This new perspective
established adaptive help-seeking as an important developmental skill in
addition to a key resource management component for self-regulated
learners. This historical shift laid the groundwork for clear
differentiation between beneficial and detrimental forms of help
solicitation.

[Newman (1994)](https://www.zotero.org/google-docs/?b39sij) refined the
categories of help seeking as defined by Nelson-Le Gall to fit within
the framework of self-regulated learning (SRL) theory. Self-regulated
learners were defined as proactive learners who adapt their strategies
to overcome barriers to learning. They use cognitive, behavioral, and
motivational strategies to achieve their goals. An adaptive help seeker
under Newman's definition used the same instrumental approaches as
defined by Nelson-Le Gall.

[Aleven et al., (2003)](https://www.zotero.org/google-docs/?7esJFp) was
among the first researchers to form the connection between adaptive
help-seeking activity and the design of technology to facilitate it.
These systems have evolved over time to include terms like cognitive
tutors and intelligent tutoring systems. A later paper by [(Aleven et
al., 2006)](https://www.zotero.org/google-docs/?XthPry) computationally
modeled adaptive and maladaptive help seeking behaviors with the goal of
building an intelligent tutoring system to identify and encourage
adaptive help-seeking behaviors.

The advance of AI use and Large Language Models has proliferated into
research on help-seeking behaviors of students using AI for learning
computer programming. [Kazemitabaar et al.
(2024)](https://www.zotero.org/google-docs/?emZBuy) studied the help
seeking behaviors of students while using CodeAid, an LLM-powered
programming assistant designed to provide assistance with course
material. One of the mechanisms for studying student use of CodeAid was
to analyze the interaction logs. A thematic analysis of the interactions
established four unique types of inquiry: asking questions, requests for
debugging code, requests for code writing assistance, and asking for
code explanations. These categories were discussed as informational and
not associated with adaptive or maladaptive learning strategies. Results
were descriptive and not correlated with student learning outcomes. An
interesting finding was students used CodeAid more around assignment and
exam due dates. The convenience of 24/7 access to the tool allowed
students to seek-help on their terms.

The second highlighted study did establish a correlation between
quantity of AI tool use in an introductory programming course and course
performance (N=52, r=0.35, p=0.0147) [(Sheese et al.,
2024)](https://www.zotero.org/google-docs/?WpNIqU). The study followed a
similar methodological approach as [Kazemitabaar et al.
(2024)](https://www.zotero.org/google-docs/?6bNchs). A custom AI tool,
called CodeHelp, was deployed to students. Trace interaction logs were
collected and analyzed using a thematic analysis broken into four
categories: debugging questions, code implementation questions,
understanding, and nothing (no category). In addition, low-effort
student queries were identified where students copied code or text and
provided little interactions. Their findings illustrated students tended
to be focused on immediate help with a current problem versus seeking to
understand broader concepts. Student help requests were unsophisticated,
often writing little to nothing. In their future work section, the
researchers discussed exploring the implications of students\'
relationship between lower effort interactions and their potential
impacts on learning.

The two studies leave gaps in literature where the impacts on the types
of help-seeking employed by the student can be explored. This can be
investigated through the lens of course performance on exams in addition
to skill acquisition through computational literacy gains.

### 2.5.4 Academic Performance

As pointed out in previous areas of the literature review, LLM use has
been observed as having both positive and negative impacts on
programming skills, cognitive offloading of tasks, computational
thinking, and self-efficacy. Most of the research to date has centered
on these advantages or disadvantages [(Cambaz & Zhang,
2024)](https://www.zotero.org/google-docs/?6TVsEe). Little research has
explored AI's impacts on academic performance, making this a suitable
area of exploration.

An empirical study from [Abbas et al.,
(2024)](https://www.zotero.org/google-docs/?PBpAdD) explored the impacts
of generative AI use on university students. They found a negative
correlation between student use of ChatGPT and grades, specifically when
the LLM was to manage workload and time pressures and subsequent
academic performance. The factors were captured via a survey that was
administered as part of the study. Participants were college students
and not enrolled in an introductory programming course, specifically.
The findings are significant, as they point to harms of using LLMs for
learning-avoidance activities, such as answer-seeking behavior in
addition to over-reliance on AI to complete academic tasks. This
corroborates research conducted in computer science disciplines that
found similar findings, but did not directly measure academic
performance [(Finnie-Ansley et al., 2022; Hassan et al., 2025;
Margulieux et al., 2024; Prather, Reeves, Leinonen, et al.,
2024)](https://www.zotero.org/google-docs/?bEmgj2).

There was research which did measure the impact of AI use on learning
outcomes within the domain of programming education [(Jošt et al.,
2024b)](https://www.zotero.org/google-docs/?Q5UbDK). The findings
indicated a significant negative correlation between reliance on LLMs
for critical programing tasks like code generation and debugging and
final grades (N = 32). Programming tasks employed by students were
identified using a survey issued after the course. Participants were
asked to recall the frequency by which they used AI for debugging, for
example, on a 5-point Likert scale. Correlations between responses and
course grades were calculated using Spearman's Rho. This research points
to an opportunity to conduct a similar study but use an unobtrusive
method such as the analysis of trace interactions between the students
and the LLM similar to [Kazemitabaar et al. (2024) and Sheese et al.
(2024)](https://www.zotero.org/google-docs/?rI32No).

When used constructively, LLM use may improve the academic performance
of students learning to program. Techniques such as scaffolding
[(Prather et al., 2019)](https://www.zotero.org/google-docs/?w87nwB) or
clarification of concepts [(Finnie-Ansley et al.,
2022)](https://www.zotero.org/google-docs/?pPvFWO) demonstrate AI can be
used as a tutor and subject-matter expert. Impacts of using AI in this
way as part of an adaptive help-seeking process should be explored
further as to better understand their potential implications on academic
performance.

2.6 Summary
-----------

The literature review demonstrated that Large Language Models (LLMs)
represent a significant, disruptive innovation [(Păvăloaia & Necula,
2023)](https://www.zotero.org/google-docs/?izzuEE) that is fundamentally
changing how programming is performed, taught, and learned. The
synthesis of the research highlights two key trends and one critical gap
relevant to novice programmers.

### 2.6.1 Duality of LLM Use

The first trend is the literature confirms the dual nature of LLM use by
programmers and in programming education. On the one hand, these tools
are lauded for their potential to enhance developer productivity for
both experienced programmers and novices [(Moradi Dakhel et al., 2023;
Peng et al., 2023; Vaithilingam et al., 2022; Ziegler et al.,
2022)](https://www.zotero.org/google-docs/?uuTaw5). Furthermore, their
ability to offer convenient, 24/7 access to expert-level assistance
presents compelling use cases for educators to build chatbots for their
courses [(Kazemitabaar et al., 2024; Sheese et al.,
2024)](https://www.zotero.org/google-docs/?DBtNbK).

On the other hand, this convenience simultaneously introduces critical
risks, including threats to academic integrity [(Denny, Kumar, et al.,
2023; Rahman & Watanobe,
2023)](https://www.zotero.org/google-docs/?QBATEm), and new
vulnerabilities in code security [(Pearce et al., 2022; Perry et al.,
2023)](https://www.zotero.org/google-docs/?ForTax). Critically, when
LLMs facilitate executive help-seeking, seeking answers rather than
understanding, they can result in detrimental outcomes such as
overreliance, poor metacognition [(Denny, Prather, et al., 2024a;
Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?UmZBFJ) and skill
depreciation, or \"deskilling\" [(Weisz et al.,
2025)](https://www.zotero.org/google-docs/?bnp2MQ).

### 2.6.2 Mechanisms by Which LLM Use Impacts Learning

Secondly, the literature is currently limited in explaining the
mechanisms by which LLM use impacts learning to program. While existing
studies have documented important outcomes such as changes in assignment
completion [(Kazemitabaar et al., 2023; Prather, Reeves, Leinonen, et
al., 2024)](https://www.zotero.org/google-docs/?StYPlK) or course grades
[(Jošt et al., 2024b)](https://www.zotero.org/google-docs/?Ebw1it), they
are only beginning to identify interaction patterns for student use of
AI [(Denny, Leinonen, et al., 2024; Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?E6RG3J) and largely fail to
connect these patterns to objective earning outcomes. Specifically, much
of the research relies on student self-report or retrospective analysis
[(Denny, Prather, et al., 2024b; Jošt et al.,
2024b)](https://www.zotero.org/google-docs/?OhZbmp). This limitation
hinders the ability to objectively differentiate beneficial LLM use
(i.e. using AI as an instrumental tool for conceptual scaffolding) from
detrimental use (e.g. such as using it for executive completion of
assignments). This deficiency in process-level data and its connection
to learning outcomes is a critical barrier to addressing concerns like
cognitive offloading and poor metacognition [(Denny, Prather, et al.,
2024a; Margulieux et al., 2024; Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?zHgzsw).

### 2.6.3 Research Rationale and Gap Statement

To date, literature has identified several interaction patterns of LLM
use among students learning to program and these behaviors can be mapped
onto the help-seeking framework [(Nelson-Le Gall, 1981; Newman,
1994)](https://www.zotero.org/google-docs/?qwQmW7). Activities such as
scaffolding, debugging, clarification [(Cambaz & Zhang, 2024;
Finnie-Ansley et al., 2022; Hassan et al., 2025; Prather et al., 2019;
Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?MByjF3) are considered
adaptive help-seeking behaviors supportive of learning. Conversely,
interactions such as over-reliance, low-effort query, and answer-seeking
[(Finnie-Ansley et al., 2022; Hassan et al., 2025; Margulieux et al.,
2024; Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?tan31K) are executive
help-seeking behaviors that reflect a focus on task-completion.

As explained in sections 2.5.3 and 2.5.4, the existing literature relies
heavily on self-reported and retrospective analysis [(Denny, Prather, et
al., 2024b; Jošt et al.,
2024b)](https://www.zotero.org/google-docs/?wMfyCb). This presents a
critical methodological opportunity to study LLM use in a more
unobtrusive manner, recording use as it happens to objectively identify
interaction patterns and measure their impacts on learning outcomes.

This study is designed to address this critical gap by leveraging
automated, objective interaction logs from an LLM-powered assistant to
categorize student help-seeking behaviors and correlate these patterns
with computational literacy and academic performance. The findings will
provide empirical evidence necessary for educators to develop and
implement ethical, effective, and evidence-based policies for LLM
integration in introductory programming courses.

**3.0 Methods**
===============

3.1 Introduction
----------------

The objective of this study was to examine the impact of generative
artificial intelligence (AI) on student learning outcomes. Specifically,
this research investigated the impacts of Large Language Model (LLM) use
among students enrolled in an introductory Python programming course.
Learning was assessed through two primary lenses: academic performance
on a summative mid-term assessment and scores derived from a
computational literacy instrument. Interaction trace data from student
LLM use were systematically categorized into behaviors representing
either superficial task-completion or active learning-seeking based on
help-seeking behavior. These interactions were quantified for each
participant, allowing for a unit of analysis that investigated the
relationship between AI usage patterns and exam performance. To further
explore these complexities, a randomized controlled trial (RCT) was
utilized, involving control and treatment groups to determine the effect
of context-awareness on summative scores. This chapter details the
experimental design, participant selection, data collection procedures,
and analytical methods used to address the research questions.

### 3.1.1 Research Questions

The following research questions were established to guide this
study.These questions were addressed using a multi-method quantitative
approach integrating content analysis [(Krippendorff,
2018)](https://www.zotero.org/google-docs/?uG3pUt) of student-LLM
interactions with rigorous statistical modeling [(Creswell & Creswell,
2017, p. 60)](https://www.zotero.org/google-docs/?ZTlUYY).

***RQ1: How does large language model use influence student learning
performance?***

This question was addressed using a quantitative correlational design
[(Creswell & Creswell, 2017: Chapter
8)](https://www.zotero.org/google-docs/?xdLUt4). The quantified
categories derived from the content analysis of student LLM usage served
as the independent variables, while mid-term exam scores represented the
dependent variable. Hierarchical linear regression analysis [(Raudenbush
& Bryk, 2002)](https://www.zotero.org/google-docs/?yQ82m3) was employed
to evaluate the unique contribution of specific interaction
patterns---such as instrumental versus executive help-seeking---as well
as their collective impact on academic performance.

***RQ2: When the LLM prompt is adjusted to include assignment
instructions (in-context learning), what is the impact on student
learning performance?***

This question was investigated through a between-subjects randomized
controlled trial [(Creswell & Creswell, 2017: Chapter
8)](https://www.zotero.org/google-docs/?hW9Uri). Linear regression
analysis was used to evaluate the causal effect of in-context learning,
utilizing a dummy variable for group assignment (control vs. treatment)
and exam scores as the dependent variable. Furthermore, mediation and
moderation analyses [(Edwards & Lambert,
2007)](https://www.zotero.org/google-docs/?Z6x4PU) were conducted to
explore the underlying behavioral mechanisms of LLM usage that might
explain the observed effects.

***RQ3: What is the relationship between large language model use and
computational literacy?***

This question was addressed using quantitative correlational design with
repeated measures [(Creswell & Creswell, 2017, Chapter
8)](https://www.zotero.org/google-docs/?KiDAww). Participants\'
computational literacy was measured at the onset of the course then at
the mid-term using identical validated instruments. Similar to RQ1,
linear regression analysis was performed where quantified LLM usage
patterns served as independent variables. An Analysis of Covariance
(ANCOVA) was utilized to control for individual differences in prior
knowledge (pre-test scores). To provide a comprehensive understanding of
these relationships, a supplementary change score analysis examined
whether specific usage patterns predicted the magnitude of improvement
in computational literacy.

3.2 Study Design
----------------

![A diagram of the study
design](./publish/thesis2/md/media/image2.png){width="6.5in"
height="3.2916666666666665in"}\
*Figure 3.1: An Overview of the Study Design.*

  **Code**   **Item**                    **Description**                                            **Timing**
  ---------- --------------------------- ---------------------------------------------------------- ------------
  C1         Diagnostic Pre-test         Baseline measure of computational literacy                 Week 1
  T1         Control Group               LLM interface without assignment-specific context          Weeks 1--6
  T2         Treatment Group             LLM interface with assignment-specific context injection   Weeks 1--6
  D1         Chat Trace Data             Interaction logs (prompts/responses) from self-hosted AI   Weeks 1--6
  E1         Midterm Exam                Summative assessment of Python programming skills          Week 7
  C2         Diagnostic Post-test        Re-issue of C1 to measure computational literacy gains     Week 7
  Q1         Participant Questionnaire   Demographic data and self-reported AI usage habits         Week 15

*Table 3.1: Summary of Study Observations and Experimental Conditions*

### 3.2.1 Overview

This study was conducted over a six-week period during the Spring 2025
semester within an introductory Python programming course IST256[^10] at
the Syracuse University School of Information Studies. The course
focused on programming fundamentals from an informatics perspective and
was designed for non-computer science majors. A total of 173 students
were enrolled. The research focused on the initial six weeks of the
semester, as these units cover foundational computational literacy
constructs: instruction sequencing, variables, branching, iteration, and
functional composition.

The study was classified as exempt by the University Institutional
Review Board (IRB\# 24-346) under Category 1 (§46.104), which pertains
to research conducted in established educational settings. While the
study elements were integrated into the curriculum, students were
provided the opportunity to opt-out of having their data included in the
final analysis.

To capture the complexities of AI-assisted learning, a multi-method
research design was adopted. A correlational design was used to examine
the relationship between AI usage patterns and summative exam scores
(Creswell & Creswell, 2017, Chapter 1). A pretest-posttest design
established a baseline and measured growth in computational literacy.
Finally, a between-subjects experimental design was employed to measure
the impacts of in-context learning via randomly assigned control and
treatment groups.

The study commenced with the administration of the diagnostic instrument
(C1) to establish a baseline for each participant\'s computational
literacy prior to instruction. Concurrently, students were introduced to
a self-hosted AI tutor application powered by GPT-4o-mini[^11].
Throughout the intervention period, students were encouraged to use the
AI as a virtual tutor for Python-related queries and course assignments.

A key feature of the AI tutor interface was a context-selection
drop-down menu (see Figure 3.2). For the control group (T1), selecting
an assignment from this menu provided no additional data to the model.

![](./publish/thesis2/md/media/image3.png){width="5.09375in"
height="5.614583333333333in"}\
*Figure 3.2: Context-Selection from the IST256 AI Tutor*

For the treatment group (T2), selecting an assignment automatically
injected the specific lab or assignment instructions into the LLM's
context (see Figure 3.3).\
![](./publish/thesis2/md/media/image14.png){width="6.5in"
height="4.0in"}\
*Figure 3.3: The treatment group (T2) is aware of the selected content.*

Because the chatbot was self-hosted, all student-AI interactions were
captured as a trace dataset (D1). Following the six-week intervention,
three primary observations were recorded:

1.  A midterm exam (E1) covering the foundational six-week content.

2.  A second administration of the diagnostic instrument (C2) to measure
    > literacy gains.

3.  A demographic questionnaire (Q1) administered at the conclusion of
    > the course to gather participant background data.

### 3.2.2 Participant Funnel

Participants (*N* = 173) were recruited from a Spring 2025 section of
IST256, an introductory Python programming course.The study was
classified as exempt by the Syracuse University Institutional Review
Board (IRB\# 24-346) under 45 CFR § 46.104(d)(1), which pertains to
research conducted in established or commonly accepted educational
settings. Of the 173 eligible students, 126 provided informed consent to
participate in the study. Five consenting students were excluded for
failing to complete all required observations (C1, C2, or E1), resulting
in a final sample of 121 participants for the broader study analysis.

#### 3.2.2.1 Population 1: Chatbot participants 

The analysis distinguished between two primary sub-populations.
Population 1 consisted of participants who engaged with the AI chatbot,
thereby generating the trace data (D1) required for interaction
analysis. This group included *n* = 87 participants, with 48 assigned to
the control group (T1) and 39 to the treatment group (T2).

![](./publish/thesis2/md/media/image5.png){width="6.5in"
height="3.5833333333333335in"}*Figure 3.4: The Participant Funnel for
Chatbot Use (n = 87)*

#### 3.2.2.1 Population 2: Chatbot participants with Survey Responses

The participant questionnaire (Q1) was administered to identify
potential covariates, including demographic data (gender, major, and
class rank) and prior programming experience. Ten chatbot users failed
to complete this survey, resulting in a reduced sample size of *n* = 77
for analyses requiring survey-derived covariate data. Among these 77
participants, 41 were in the control group and 36 were in the treatment
group.

![](./publish/thesis2/md/media/image12.png){width="6.5in"
height="3.0555555555555554in"}*Figure 3.5: The Participant Funnel
Integrating Survey Responses (n = 77)*

### 3.2.3 Computational Literacy Instrument (C1/C2)

Computational literacy is a fundamental objective of introductory
programming curricula, where the specific programming language serves
primarily as a vehicle for experiential learning. Rather than mere
syntax proficiency, the primary learning objective is the development of
abstract computational reasoning necessary to address future technical
challenges.

Because no consensus model currently exists for the development of
computational thinking, there is a lack of universally accepted
measurement instruments [(Shute et al.,
2017)](https://www.zotero.org/google-docs/?DLRbui). [Brennan and Resnick
(2012)](https://www.zotero.org/google-docs/?EpJMU8) identified three
primary dimensions of the computational thinking framework:
computational concepts (programming structures), computational practices
(debugging and remixing), and computational perspectives (problem
framing).

The psychometrically validated CT-Test, developed by [Román-González et
al., (2017)](https://www.zotero.org/google-docs/?Tkr7qs), focuses
exclusively on computational concepts. The concepts evaluated by the
instrument include: loops, branching, arrays, functions, data
representation, and instruction sequencing. These concepts aligned
closely with the instructional content within the first six weeks of the
IST256 course.

The CT-Test consists of 28 multiple-choice questions, and students were
allotted 45 minutes for completion. The instrument was administered in
class using the Syracuse University Blackboard learning management
system, with items delivered individually in a randomized order.
Consistent with the original instrument\'s design, participants were
permitted to skip and revisit items. The post-test (C2) utilized the
same items as the pre-test (C1), though the question order was
re-randomized for each participant. Students received a raw score out of
28 but were provided no feedback regarding the accuracy of specific
responses as to minimize the practice effect.

The following figure is an example question from the CT-Test. The entire
instrument can be found in appendix A.

![](./publish/thesis2/md/media/image7.png){width="6.5in"
height="3.1666666666666665in"}\
*Figure 3.6: A Sample Question from The CT-Test*

### 3.2.4 Chatbot Design

The AI chatbot application[^12] developed for this study was programmed
in Python utilizing the Streamlit[^13] framework. It was released as
open source under the Apache 2.0 license and published to GitHub[^14].
The platform was deployed to a Kubernetes cluster at Syracuse University
data center. To access the application, users were required to
authenticate using their institutional Syracuse University credentials.
Participant chat interaction trace data (D1) were stored in a PostgreSQL
database located within the same data center. A custom Python script was
developed to extract these data from the database for subsequent
analysis.

#### 3.2.4.1 LLM Selection

Acceptance criteria for selecting a Large Language Model (LLM) for the
AI chatbot were primarily based on accuracy and response time. It was
essential that performance metrics remain comparable to popular
commercially hosted platforms available at the time of the study, such
as ChatGPT[^15] and Claude[^16] to minimize participant attrition
resulting from technical friction. Several self-hosted, open-weight
models, including Dolphin3[^17], Llama3[^18], CodeLlama[^19] and
Qwen2.5[^20], were initially evaluated; however, tests revealed these
models exhibited significant performance degradation under concurrent
load due to their deployment on time-shared institutional GPU hardware.
While model accuracy of their generations was deemed suitable for the
course content, their scalability was insufficient for the study\'s
requirements.

Ultimately, OpenAI's GPT-4o-mini[^21] was selected as the foundational
model. This model provided an optimal balance of cost-efficiency,
response time, and performance. Furthermore, its deployment via the
Azure cloud environment ensured robust handling of concurrent text
generation. While OpenAI's GPT-4o[^22] model was also evaluated, its
performance was comparable to the \"mini\" variant despite a sixteenfold
increase in operational cost; consequently, GPT-4o-mini was deemed the
most efficient choice.

With optimized prompting, the GPT-4o-mini model generated valid
solutions for all course programming assignments and laboratory
exercises. Additionally, the model correctly answered 43 of 45 questions
on the midterm exam (E1), placing its performance in the 98th
percentile. This exceeded benchmarks established by prior research
conducted by [Savelka et al.,
(2023)](https://www.zotero.org/google-docs/?sTuNTA).

#### 3.2.4.2 Random Assignment

Once authenticated to the AI chatbot website, participants were assigned
to the control or treatment groups based on the MD5 hash of their
student ID being odd or even. This method assured each student was
always assigned to the same group at each login session. The algorithm
is provided here:

hash = md5(student\_id)\
number = int(hash)\
in\_treatment = mod(number, 2) \# odd or even

#### 3.2.4.3 Control Group (T1)

Every request processed by the AI Tutor incorporated a standardized
system prompt designed to establish operational guardrails and regulate
the generated output. The primary objectives of this system prompt were
to:

1.  Enforce Code Alignment: Ensure the generation of Python code
    > followed the specific stylistic conventions taught in the course.

2.  Provide Instructional Scaffolding: Mandate comprehensive,
    > plain-English explanations for all generated code segments.

3.  Adopt a Tutoring Persona: Maintain the persona of a helpful and
    > friendly virtual tutor tailored for a college-level introductory
    > Python course.

4.  Enforce Content Filtering: Restrict responses to course-related
    > inquiries and decline to respond to questions not related to
    > Python programming or the course.

These constraints were implemented to mitigate challenges identified in
prior research, where AI models failed to provide pedagogical
explanations or generated code that deviated from instructional
standards [(Prather, Reeves, Leinonen, et al.,
2024)](https://www.zotero.org/google-docs/?ScROEN). Following an
iterative evaluation process, a final prompt configuration was selected
to optimize the balance between objective achievement and token
efficiency. This configuration served as the baseline model for the
control group (T1)\
![](./publish/thesis2/md/media/image1.png){width="6.5in"
height="2.0in"}\
*Figure 3.7: System Prompt Configuration for the Control Group (T1)*

#### 3.2.4.4 Treatment Group (T2)

The treatment group (T2) utilized the same foundational LLM and system
prompt configurations as the control group (T1), supplemented by a user
prompt injected into the conversation based on the participant\'s
contextual selection. For instance, if a participant selected
*"03-HW-Conditionals"* as the assignment context, the full content of
the corresponding homework notebook file:
"*lessons/03-Conditionals/HW-Conditionals.ipynb"* was loaded into the
chat session. This file was identical to the assignment provided to the
students and contained all instructions, suggested approaches, and
scaffolded code sections. This technique provided in-context learning to
the LLM as the assignment instructions were now included in the
conversational memory.

The following prompt template was employed to integrate this metadata
into the conversation:

![A black screen with white text AI-generated content may be
incorrect.](./publish/thesis2/md/media/image15.jpg){width="6.5in"
height="1.3472222222222223in"}

*Figure 3.8: Treatment T2 Context Prompt Template*

Following the injection of this context, the AI chatbot acknowledged its
readiness to assist with the specific assignment, demonstrating
immediate context awareness.

![A black background with white text AI-generated content may be
incorrect.](./publish/thesis2/md/media/image22.jpg){width="6.5in"
height="1.3611111111111112in"}

*Figure 3.9: AI Response to Context Selection in the Treatment Condition
(T2)*

When a participant requested assistance with a specific section, the AI
responded with functional code accompanied by a pedagogical explanation.
This mechanism highlights the primary distinction between the two
groups: while T1 could generate similar outputs, participants in the
control condition were required to manually provide the necessary
instructions or code snippets to the model. Essentially, T2 automated
the prompting process that T1 participants would otherwise have to
perform manually. This design allowed the study to investigate whether
such context-awareness improved user engagement and learning or merely
provided a higher degree of convenience in question-answering.

### 3.2.5 Midterm Exam (E1)

The primary objective of the midterm exam (E1) was to assess participant
proficiency regarding the fundamental computational concepts taught
during the six-week intervention period. The assessment targeted four
specific domains: (a) theoretical concepts, such as the distinction
between definite and indefinite loops; (b) the practical application of
concepts, such as identifying the appropriate circumstances for using
specific programming structures; (c) language-specific implementation,
focusing on Python syntax and keyword usage; and (d) functional code
tracing, requiring students to predict the output of provided code
snippets.

The exam consisted of 45 multiple-choice questions, and participants
were allotted 45 minutes for completion. The assessment was conducted
under closed-book conditions, with the exception of a single-page
reference sheet allowed as a study aid. To maintain academic integrity,
the exam was administered in a proctored, paper-based format. Five
distinct versions of the exam were utilized, featuring randomized
question and answer sequences. Versions A through D were distributed
during the standard class session, while Version E was reserved for
students requiring accommodations at the university testing center. The
internal consistency for all versions, as measured via Cronbach's alpha
(𝛼), ranged from .83 to .88, establishing the instrument as a reliable
measure of student subject knowledge [(Cronbach,
1951)](https://www.zotero.org/google-docs/?WLDVx1).

  **Exam Version (E1)**   ***n***   **𝛼**
  ----------------------- --------- -------
  A                       40        0.87
  B                       40        0.86
  C                       40        0.83
  D                       39        0.87
  E                       9         0.88
  Total                   168       

*Table 3.2: Internal Consistency (Cronbach's Alpha) of the E1 Midterm
Exam*

### 3.2.6 Questionnaire (Q1)

A debriefing questionnaire (Q1) was administered following the
conclusion of the experimental intervention. The primary objectives of
this instrument were to:

1.  Demographic Profiling: Collect baseline data regarding the
    > participant pool, including gender, academic major, and class
    > rank.

2.  Prior Experience Assessment: Identify participants with previous
    > computer programming experience.

3.  External AI Usage Monitoring: Identify participants who utilized
    > artificial intelligence tools other than the self-hosted AI tutor
    > provided for the course.

4.  Perceptual Data Collection: Evaluate student perceptions of computer
    > programming and the utility of AI in an educational context.

The questionnaire was delivered via the Syracuse University Qualtrics
survey system; the complete instrument is available in Appendix B. For
the purposes of the subsequent data analysis, only demographic data and
indicators of prior programming experience were utilized to test for
covariates.

### 3.2.7 Chatbot Trace Data (D1)

As previously described, the AI chatbot recorded all participant
interactions and system responses within a PostgreSQL database. These
records captured the timing of interactions, the selected assignment
context, and the participant\'s experimental group assignment. The
structure of the D1 trace data is detailed in the following data
dictionary

  **Field**        **Data Type**                  **Purpose**
  ---------------- ------------------------------ ------------------------------------------------------------------------------------------------------------------------------------------------------------
  Id               Sequential integer             A unique number for each item in the trace data, the higher the number the more recent the interaction.
  Session Id       Universally Unique ID (UUID)   A globally unique identifier to record the chat session. Filtering on a specific session Id will produce a conversation between user and the AI assistant.
  Participant ID   Text                           The participant number. Unique for each participant, so that AI use can be traced back to observations C1, C2, E1 and questionnaire Q1.
  Timestamp        ISO8601 timestamp              The UTC timestamp user's prompt or AI response as text string in IST8601 format
  Model            Text                           The AI Model used. This is always gpt-4o-mini
  Rag              Boolean                        True is the treatment group T1 whereas False is the control group T2
  Context          Text                           The user selected context at the time of the user prompt or AI response
  Role             Text                           Values "user" or "assistant" Indicator of whether the row was a user prompt or an AI response.
  Content          Text                           In the case of Role == "user", the Content is the prompt. When the Role == "assistant", the content is the AI generated response.

*Table 3.3: Fields in the D1 Chatbot Trace Data*\
While trace data can be coded through various lenses, such as prompt
specificity or question type, this study utilized the data to classify
interactions at the session level and quantify those interactions for
statistical analysis.

The raw D1 dataset contained 9,518 entries, with each row representing a
single user prompt or AI response. To facilitate analysis at the session
level---defined as a sequential series of requests and responses
constituting a single conversation---the data were grouped by Session Id
and ordered chronologically by Timestamp. This aggregation process
resulted in a final corpus of 1,024 unique sessions.

3.3 Data Analysis
-----------------

### 3.3.1 Overview 

This section details the methodology employed to operationalize the D1
chatbot trace data. Given that all three research questions required
trace data for empirical investigation, these logs served as a primary
instrument in the study. Categorical content analysis [(Neuendorf,
2017)](https://www.zotero.org/google-docs/?imAA0t) was utilized to
classify student-AI interactions into two broad categories based on
help-seeking theory: learning-supportive activities (adaptive
help-seeking) and learning-avoidance activities (executive help
seeking). The unit of analysis was defined as the participant's chat
session, spanning from login to logout. In addition, a session was reset
wherever a student switched contexts in the chat interface. The trace
data were coded at the session level (*n* = 1,024), and the resulting
codes were aggregated by participant to align with the higher-level unit
of analysis required for statistical modeling (*n* = 87).

Prior to performing the categorical content analysis, a codebook was
developed deductively. The categories were established based on a
synthesis of existing literature and pedagogical expertise acquired
through seven years of instruction in the course. A random sample of 50
sessions was selected for human coding to establish a baseline for
validation. Subsequently, the codebook was transformed into an LLM
prompt to facilitate the automated coding of the remaining sessions, a
technique consistent with the work of [Xiao et al.
(2023)](https://www.zotero.org/google-docs/?KqI6Sg).

Acknowledging findings by [Pilny et al.
(2024)](https://www.zotero.org/google-docs/?0N4LQE) that LLMs vary in
their efficacy for content analysis, four distinct models were evaluated
against the human-coded baseline. To ensure coding consistency and
mitigate the risk of temporal variability identified by [(Hackl et al.
2023)](https://www.zotero.org/google-docs/?166nDy), each candidate model
performed the classification task on the 50-session sample three times.
Krippendorff's alpha (𝛼) was utilized to validate inter-coder
reliability between the LLM and the human baseline, as well as the
model\'s internal consistency [(Krippendorff,
2011)](https://www.zotero.org/google-docs/?iDryVo). This evaluative
approach aligns with methodologies employed in recent studies of AI in
programming education ([Ghimire & Edwards,
2024)](https://www.zotero.org/google-docs/?xizpBk). Once the optimal
model was identified, all 1,024 sessions were classified and quantified
into categories of \"Learning\" (adaptive-help seeking) or \"Task
Completion\" (executive-help seeking) to support the subsequent
quantitative analysis.

### 3.3.2 Tools

Data analysis was conducted using the Python programming language
[(Python Software Foundation,
2023)](https://www.zotero.org/google-docs/?cchhAo), within Jupyter
notebooks [(Kluyver et al.,
2016)](https://www.zotero.org/google-docs/?kSKGFd). Quantitative
visualizations were generated using the matplotlib [(Hunter,
2007)](https://www.zotero.org/google-docs/?by065J) and seaborn [(Waskom,
2021)](https://www.zotero.org/google-docs/?Z5zeig) libraries.
Specialized diagrams like the sankey diagrams and forestplots used
sankeyflow [(Xu, 2024)](https://www.zotero.org/google-docs/?DcqBQt) and
forestplot [(Shen, 2024)](https://www.zotero.org/google-docs/?JoVZRx)
libraries respectively. Statistical computations and data manipulation
were facilitated by a suite of specialized libraries, including pandas
[(McKinney, 2010)](https://www.zotero.org/google-docs/?8AG8cQ), scipy
[(Virtanen et al., 2020)](https://www.zotero.org/google-docs/?6nIUGT),
statsmodels [(Seabold & Perktold,
2010)](https://www.zotero.org/google-docs/?DKVRTF), pingouin [(Vallat,
2018)](https://www.zotero.org/google-docs/?S2i1TN), and simpledorff
[(Holzäpfel, 2020)](https://www.zotero.org/google-docs/?KrZj0F).
Furthermore, Openrouter[^23] served as a unified API gateway to access
various Large Language Models across the OpenAI, xAI, Google, and
Anthropic platforms.

To ensure participant confidentiality and data security, all raw and
processed datasets were maintained alongside the source code in a
private Git repository. This repository was further secured via backups
to a personal storage device. Following the conclusion of the study, the
research materials were cleaned of all personally identifiable
information (PII) to prevent the linkage of data to individual
participants. The final code and anonymized datasets were published to a
public GitHub repository[^24].

### 3.3.3 Operationalizing D1 Chatbot Trace Data 

To perform the categorical content analysis of the 1,024 D1 chatbot
trace data sessions, a codebook was first developed deductively. An
initial set of categories was established based on existing literature
and pedagogical expertise derived from seven years of personal
instruction in the IST256 course. A random sub-sample of 50 sessions was
selected from the D1 dataset to identify initial classifications. Each
session in this sub-sample was classified according to the criteria
defined in *Table 3.4*. Furthermore, the classified activities were
summarized into representative examples to be incorporated into the LLM
coding prompt

+-------------+-------------+-------------+-------------+-------------+
| **P         | **D         | **Example** | **          | *           |
| articipant\ | efinition** |             | Classified\ | *Supported\ |
| Behavior**  |             |             | Activity**  | Citations** |
+=============+=============+=============+=============+=============+
| Seeking     | The         | \"Can you   | Task        | [(Fi        |
| Answers     | participant | code the    | Completion  | nnie-Ansley |
| (           | makes a     | solution    |             | et al.,     |
| Superficial | direct ask  | for         | (Executive  | 2022)]      |
| Learning)   | of the AI   | assignment  | He          | (https://ww |
|             | to complete | ABC?\"      | lp-Seeking) | w.zotero.or |
|             | their       |             |             | g/google-do |
|             | assignment  | \"How do I  |             | cs/?EeccHE) |
|             | or lab.     | complete    |             |             |
|             | There is no | section XYZ |             | [(Hassan et |
|             | co          | in the      |             | al.,        |
|             | nversation. | lab?\"      |             | 2025)]      |
|             |             |             |             | (https://ww |
|             |             |             |             | w.zotero.or |
|             |             |             |             | g/google-do |
|             |             |             |             | cs/?M8nObm) |
+-------------+-------------+-------------+-------------+-------------+
| O           | The         | \"Can you   | Task        | [(Prather,  |
| verreliance | participant | convert     | Completion\ | Reeves,     |
|             | asks the AI | this        | (Executive  | Leinonen,   |
| (Cognitive  | to complete | algorithm   | Help        | et al.,     |
| offloading  | a task and  | into        | Seeking)    | 2024)]      |
| for task    | does not    | code?\"     |             | (https://ww |
| completion) | further     |             |             | w.zotero.or |
|             | engage.     | \"Can you   |             | g/google-do |
|             | Thus there  | provide an  |             | cs/?b94RCp) |
|             | is no clear | approach to |             |             |
|             | intention   | start this  |             | [           |
|             | to          | as          |             | (Margulieux |
|             | understand  | signment?\" |             | et al.,     |
|             | their work  |             |             | 2024)]      |
|             | for them.   | \"Fix this  |             | (https://ww |
|             | Thus a deep | error for   |             | w.zotero.or |
|             | connection  | me.\"       |             | g/google-do |
|             | to the      |             |             | cs/?afJ6YN) |
|             | material is |             |             |             |
|             | not formed. |             |             |             |
+-------------+-------------+-------------+-------------+-------------+
| Scaffolding | AI provides | \"What does | Learning\   | [(Prather   |
|             | support /   | this error  | (Adaptive   | et al.,     |
| (AI as      | expertise   | mean?\"     | He          | 2019)]      |
| Expert)     | to the      |             | lp-Seeking) | (https://ww |
|             | learner to  | \"Can you   |             | w.zotero.or |
|             | a learner   | help me     |             | g/google-do |
|             | to help     | locate the  |             | cs/?wDe1Ck) |
|             | them        | error in my |             |             |
|             | achieve a   | code?\"     |             | [(Prather,  |
|             | task they   |             |             | Reeves,     |
|             | couldn\'t   | \"Can you   |             | Denny, et   |
|             | complete on | help me     |             | al.,        |
|             | their own.  | t           |             | 2024)]      |
|             |             | roubleshoot |             | (https://ww |
|             |             | my code?\"  |             | w.zotero.or |
|             |             |             |             | g/google-do |
|             |             |             |             | cs/?svZdyf) |
|             |             |             |             |             |
|             |             |             |             | [(Hassan et |
|             |             |             |             | al.,        |
|             |             |             |             | 2025)]      |
|             |             |             |             | (https://ww |
|             |             |             |             | w.zotero.or |
|             |             |             |             | g/google-do |
|             |             |             |             | cs/?vorDax) |
+-------------+-------------+-------------+-------------+-------------+
| Questioning | Asking the  | Can you     | Learning    | [(Fi        |
|             | AI to       | provide an  |             | nnie-Ansley |
| (AI as      | explain a   | example of  | (Adaptive   | et al.,     |
| Tutor)      | concept or  | a nested    | He          | 2022)]      |
|             | provide     | loop?       | lp-Seeking) | (https://ww |
|             | code        |             |             | w.zotero.or |
|             | examples of | Why would I |             | g/google-do |
|             | a concept.  | use a       |             | cs/?nTmux6) |
|             |             | nested IF   |             |             |
|             |             | versus      |             | [(Cambaz &  |
|             |             | elif?       |             | Zhang,      |
|             |             |             |             | 2024)]      |
|             |             | Can you     |             | (https://ww |
|             |             | help me     |             | w.zotero.or |
|             |             | understand  |             | g/google-do |
|             |             | di          |             | cs/?NzDiBi) |
|             |             | ctionaries? |             |             |
|             |             |             |             |             |
|             |             | When would  |             |             |
|             |             | I use a     |             |             |
|             |             | list versus |             |             |
|             |             | a           |             |             |
|             |             | dictionary? |             |             |
+-------------+-------------+-------------+-------------+-------------+
| In          | The         | \"When is   | I           |             |
| conclusive\ | transcript  | the         | nconclusive |             |
| (Unable to  | does not    | exam?\"     |             |             |
| Determine)  | provide     | \<br\>\"Can |             |             |
|             | enough      | you tell me |             |             |
|             | information | the         |             |             |
|             | to classify | weather?\   |             |             |
|             | the         | "\<br\>What |             |             |
|             | par         | did I ask   |             |             |
|             | ticipant\'s | you last    |             |             |
|             | behavior.   | week?       |             |             |
|             | Off topic   |             |             |             |
|             | question    |             |             |             |
|             | not about   |             |             |             |
|             | the subject |             |             |             |
|             | matter.     |             |             |             |
+-------------+-------------+-------------+-------------+-------------+

*Table 3.4: Codebook of Participant Behaviors in Trace Data (D1)*

The classification process is illustrated by an interaction from
Participant 119, who submitted a single prompt: *\"Write a function,
score\_sentiment() which given 3 inputs\... will return an integer
score\...\"*. Because the participant provided assignment instructions
to elicit code generation without further inquiry, the session was
classified as Seeking Answers, which is a form of Task Completion /
Executive Help-Seeking.

In contrast, an interaction from Participant 107 involved multiple
conceptual inquiries, such as asking for an explanation of boolean logic
(*\"Why \[is it\] false? a=0.1 b=0.2 bool(a+b==0.3)\"*) and operator
distinctions (*\"explain == vs =\"*). Since the participant sought to
understand programming concepts taught in the course, this interaction
was classified as Questioning behavior, which is a form of Learning /
Adaptive Help-Seeking. An AI prompt was subsequently formulated using
this codebook and observed interactions; the complete prompt is provided
in Appendix C.

### 3.3.4 Model Selection Reliability Testing

Utilizing a Large Language Model (LLM) for content analysis introduced
two primary methodological concerns: inter-coder reliability and
internal consistency. First, it was necessary for the LLM classifier to
align closely with the 50 human-coded baseline classifications. Second,
given that LLMs can exhibit stochastic behavior or \"hallucinations,\"
the selected model needed to demonstrate high internal reliability
across multiple classifications of the same dataset. The optimal model
was defined as the one achieving the highest degree of agreement with
the human baseline while remaining most internally consistent.

Four candidate models from different LLM providers were selected as
candidates for content analysis task: xAI's grok-4-fast[^25], OpenAI's
gpt-5-mini[^26], Google's gemini-2.5-flash[^27], and Anthropic's
claude-sonnet-4[^28]. Before these models could be formally evaluated, a
classification prompt was engineered based on the codebook presented in
*Table 3.4*.

The development of the prompt was an iterative process that involved
integrating specific instructions and few-shot examples. For each
iteration, a representative interaction was selected and used to elicit
generations from the four LLMs. These outputs were then verified against
the human-coded baseline in the prompt to ensure they met the
classification criteria. This refinement cycle was repeated for each of
the five classification types: Seeking Answers, Overreliance,
Scaffolding, Questioning, and Inconclusive. The prompt was finalized
only after it consistently elicited the correct classification across
all models and categories.

To assess inter-coder reliability, each model classified the 50-session
sub-sample, and the results were compared against the human baseline
classification using Krippendorff's alpha (𝛼). Krippendorff's alpha was
selected as the reliability coefficient due to its versatility across
different scales of measurement and its robustness in handling small
sample sizes. Following the benchmarks established by [Krippendorff
(2011)](https://www.zotero.org/google-docs/?Vh3T7i), a coefficient of 𝛼
\>= .800 was set as the threshold for highly reliable agreement, while
scores between .667 and .800 were considered acceptable for tentative
conclusions. This procedure was repeated three times to establish a
measure of internal consistency (stability) for each model, with a
target consistency of 1.000, indicating the model performed the
classification task identically across all iterations.

  ----------------------------------------------------------------------------------------
  **Model**                   **Agreement with Human** **𝛼**   **Internal Consistency 𝛼\
                                                               (3 runs)**
  --------------------------- -------------------------------- ---------------------------
  x-ai/grok-4-fast            0.873                            0.885

  openai/gpt-5-mini           0.789                            0.915

  google/gemini-2.5-flash     0.833                            1.000

  anthropic/claude-sonnet-4   0.873                            1.000
  ----------------------------------------------------------------------------------------

*Table 3.5: Krippendorff's Alpha for Inter-coder Reliability and
Internal Consistency*

As indicated in Table 4, x-ai/grok-4-fast and anthropic/claude-sonnet-4
demonstrated the highest level of agreement with the human baseline.
However, only google/gemini-2.5-flash and anthropic/claude-sonnet-4
exhibited perfect internal consistency (𝛼 = 1.000) across all runs.
Consequently, the anthropic/claude-sonnet-4 model was selected as the
final classifier due to its superior performance in both reliability
dimensions (Agreement 𝛼 = 0.873; Consistency 𝛼 = 1.000). For additional
context, the collective Krippendorff's alpha across all models and the
human rater for the three runs ranged from 𝛼 = .751 to 𝛼 = .772.

### 3.3.5 Categorical Content Analysis

Following the identification of the optimal Large Language Model (LLM)
for the classification task, Anthropic's Claude-sonnet-4 was utilized to
categorize all 1,024 sessions within the D1 chatbot trace dataset. The
automated content analysis identified 623 sessions as Learning, 336
sessions as Task Completion, and 35 sessions as Inconclusive.

Because the final unit of analysis for this study is the individual
student, session-level classifications were aggregated for each of the
*n* = 87 participants. For example, Participant 82 was associated with
33 Learning sessions, 7 Task Completion sessions, and 2 Inconclusive
sessions. In contrast, Participant 124 generated 5 Learning sessions, 25
Task Completion sessions, and 1 Inconclusive session. By aggregating the
data in this manner, the frequency of each interaction type could be
utilized as an independent variable to evaluate its impact on student
outcomes, specifically the E1 midterm exam and the C1/C2 computational
thinking assessments.

![](./publish/thesis2/md/media/image18.png){width="5.234375546806649in"
height="3.900122484689414in"}

*Figure 3.10: Distribution of Chat Session Classifications From the D1
Dataset*

3.4 Hypothesis Formulation and Methodology
------------------------------------------

With the dataset established, the statistical analysis commenced. This
section operationalizes the primary research questions into testable
hypotheses and details the methodological framework employed to
investigate each query.

### 3.4.1 RQ1 Hypothesis and Methodology

**Research Question 1 (RQ1):** How does Large Language Model (LLM)
influence student learning performance?

This question investigates the relationship between the frequency of
participant sessions classified as Learning and Task Completion (derived
from the D1 dataset) and their performance on the midterm exam (E1).

**Alternative Hypothesis (*H*~1~):** The quantity and classification of
participant sessions in the D1 dataset are significantly associated with
midterm exam scores (E1).

-   ***H*~1a~ :** There is a positive correlation between the quantity
    > of sessions classified as Learning and midterm exam scores.

-   ***H*~1b~ :**There is a negative correlation between the quantity of
    > sessions classified as Task Completion and midterm exam scores.

**Null Hypothesis (*H*~01~):** There is no statistically significant
relationship between the quantity of participant sessions (regardless of
classification) and midterm exam scores (E1).

**Methodology**

A hierarchical multiple regression analysis [(Raudenbush & Bryk,
2002)](https://www.zotero.org/google-docs/?xMt43p) was employed to test
the hypotheses. This approach allows for the evaluation of the unique
contribution of each independent variable in addition to their
collective impact on exam scores. The beta coefficients (𝛽) indicate the
direction (positive or negative) and magnitude of the relationship
between the predictors and the outcome variable.

The analysis followed a four-step model progression:

**Model 0 (E1 \~ Session Count):** E1 was regressed on Session Count
without classification into Learning or Task Completion.

**Model 1 (E1 \~ Task Completion Session Count):** E1 was regressed on
Task Completion session count session count to establish its individual
relationship.

**Model 2 (E1 \~ Learning Session Count):** E1 was regressed on the
Learning session count to establish its individual relationship.

**Model 3 (E1 \~ Task Completion Session Count + Learning Session
Count):** E1 was regressed simultaneously on both Task Completion
session and Learning session counts to examine their independent effects
while controlling for one another.

For each model, the following statistics were reported: standardized
beta coefficients (*β*), standard errors (*SE*), t-statistics (*t*),
p-values (*p*), 95% confidence intervals (*CI*), and overall model fit
statistics, including the coefficient of determination (*R^2^*),
adjusted r-squared (Adj. *R^2^*), and F-statistic (*F*). Changes in
*R^2\ ^* (*ΔR^2^*) were calculated to determine if the addition of a
second predictor explained unique variance.

**Criteria for Hypothesis Testing**

Statistical significance was defined at the 𝛼 = .05 level.

-   ***H*~1a~ Support:** A positive *β* coefficient for Learning
    > sessions with a *p* \< .05.

-   ***H*~1b~ Support:** A positive *β* coefficient for Task Completion
    > sessions with a *p* \< .05.

The null hypothesis (***H*~01~**) was rejected only if both conditions
were satisfied, indicating that the duality of LLM use (Learning vs.
Task Completion) significantly predicts academic outcomes.

### 3.4.2 RQ2 Hypothesis and Methodology

**Research Question 2 (RQ2):** When the prompt is adjusted to include
assignment instructions (in-context learning), what is the impact on
student learning performance?

This question investigated the impact of in-context learning (ICL) on
student performance as measured by midterm exam scores (E1). In this
study, ICL was operationalized by injecting assignment-specific
instructions and scaffolding into the LLM's context for participants in
the treatment group.

**Alternative Hypothesis (*H*~2~):** The mean student learning
performance score (E1) for the treatment group (context-aware AI) will
be statistically significantly higher than the mean score for the
control group.

**Null Hypothesis (*H*~02~):** There is no statistically significant
difference in the mean student learning performance scores (E1) between
the treatment and control groups.

**Methodology**

A between-subjects experimental design [(Creswell & Creswell, 2017,
Chapter 8)](https://www.zotero.org/google-docs/?rvvwq7) was employed.
Participants were randomly assigned to either the control group (T1) or
the treatment group (T2). The dependent variable was the E1 score,
measured on a continuous scale. The independent variable (group
assignment) was dummy coded (0 = control, 1 = treatment) for use in
regression models.

Statistical significance was assessed at the 𝛼 = .05 level. Following
the initial assessment of group differences, a multi-stage regression
approach was employed to identify suppression, mediation, and moderation
effects [(Edwards & Lambert,
2007)](https://www.zotero.org/google-docs/?xe6s9J).

**Model 1: Total Effect (E1 \~ Treatment):** E1 was regressed on the
dummy-coded treatment variable to identify the mean difference in exam
performance between the control and treatment groups.

**Model 2: Mediation Analysis:** This stage explored whether the
treatment effect operated through changes in student usage behaviors:

-   **Model 2a (Learning Session Count \~ Treatment )** This model
    > determined if group assignment predicts Learning engagement.

-   **Model 2b (Task Completion Session Count \~ Treatment)** This model
    > determined if group assignment predicts task-completion
    > engagement.

**Model 3: Moderation Analysis** This stage examined whether the
treatment condition altered the strength of the relationship between
usage patterns and exam performance (interaction effects):

-   **Model 3a (E1 \~ Treatment x Learning Session Count)** This model
    > tested if context-aware AI moderated the impact of Learning
    > engagement on E1.

-   **Model 3b (E1 \~ Treatment x Task Completion Count)** This model
    > tested if context-aware AI moderated the impact of task-completion
    > engagement on E1.

**Model 4: Suppression Analysis (E1 \~ Learning Session Count + Task
Completion Session Count)** This model examined whether the inclusion of
AI usage patterns altered the treatment effect observed in Model 0,
thereby identifying possible suppression.

### 3.4.3 RQ3 Hypothesis and Methodology

**Research Question 3 (RQ3)***:* What is the relationship between large
language model use and computational literacy?

This question investigates the relationship between the frequency of
participant sessions classified as Learning and Task Completio**n**
(from the D1 dataset) and their computational literacy scores as
measured by the CT-Test (C1 and C2).

**Alternate Hypothesis (*H*~3~):** The quantity and classification of
participant sessions in the D1 dataset are significantly associated with
computational literacy scores (C1, C2).

-   ***H*~3a~ :** There is a positive correlation between the quantity
    > of sessions classified as Learning and computational literacy
    > scores.

-   ***H*~3b~ :** There is a negative correlation between the quantity
    > of sessions classified as Task Completion and computational
    > literacy scores.

**Null Hypothesis for (*H*~03~):** There is no statistically significant
relationship between the quantity of participant sessions (regardless of
classification) and computational literacy scores (C1, C2).

**Methodology**

To establish the reliability of the assessment instrument across
administrations, a Pearson correlation (*r*) was calculated between the
pre-test (C1) and post-test (C2) scores [(Vaz et al.,
2013)](https://www.zotero.org/google-docs/?sedsAX).

**Model 1: ANCOVA (C2 \~ Learning Session Count + Task Completion
Session Count + C1)**

To account for baseline computational literacy and potential test-retest
effects, an Analysis of Covariance (ANCOVA) was employed using a linear
regression framework [(Huitema,
2011)](https://www.zotero.org/google-docs/?lwb3sB). In this model, the
post-test score (C2) served as the dependent variable. The baseline
score (C1) was included as a covariate to control for individual
differences in prior knowledge, while Task Completion and Learning
session counts served as the primary independent variables ([Maxwell et
al. 2017](https://www.zotero.org/google-docs/?2QVeNI)). This approach
allowed for the examination of whether LLM usage patterns predicted
learning outcomes beyond what would be expected from baseline ability
alone.

**Model 1a: (C2-C1 \~ Learning Session Count + Task Completion Session
Count)**

Additionally, a supplementary analysis was conducted using gain scores
(*ΔC = C2 - C1*) as the dependent variable to examine if usage patterns
predicted the magnitude of improvement. Recognizing that gain scores can
exhibit lower reliability when pre- and post-test correlations are high
[(Cronbach & Furby, 1970)](https://www.zotero.org/google-docs/?m6FKwM),
this was used as a complementary measure to ensure a comprehensive
understanding of the relationship between LLM usage and literacy
development.

**Criteria for Hypothesis Testing**

Statistical significance was defined at the 𝛼 = .05 level.

-   ***H*~3a~ Support:** A positive *β* coefficient for Learning
    > sessions with a *p* \< .05 in the ANCOVA model.

-   ***H*~3b~ Support:** A positive *β* coefficient for Task Completion
    > sessions with a *p* \< .05 in the ANCOVA model.

The null hypothesis (***H*~03~**) was rejected only if both conditions
were satisfied.

### 3.4.4 Satisfying Assumptions of Linear Regressions

For every linear regression model, formal diagnostic tests for
Gauss-Markov assumptions were conducted to ensure the validity and
reliability of the statistical inferences [(Cohen et al., 2013; Osborne
& Waters, 2002)](https://www.zotero.org/google-docs/?Z880H3). Linearity
was assessed through the visual inspection of residual and regression
plots. Residual plots and regression plots were observed for linearity.
To determine if the variance of the residuals were constant across all
levels of the independent variables, the Breusch-Pagan test for
homoscedasticity was used [(Breusch & Pagan,
1979)](https://www.zotero.org/google-docs/?8K0xlP).

The independence of observations was verified using the Durbin-Watson
statistic to check for potential autocorrelation [(Durbin & Watson,
1971)](https://www.zotero.org/google-docs/?uQj75M). To ensure the
residuals were normally distributed, the Shapiro-Wilk test was performed
[(Shaphiro & Wilk, 1965)](https://www.zotero.org/google-docs/?XBdLM8).
Finally, to identify potential multicollinearity among independent
variables, Variance Inflation Factor (VIF) metrics were calculated
[(Farrar & Glauber, 1967)](https://www.zotero.org/google-docs/?4mopcJ).

In instances where diagnostic testing revealed heteroscedasticity
(non-constant error variance), models were re-estimated using
heteroscedasticity-robust standard errors (MacKinnon & White, 1985).
This approach facilitated valid statistical inference by providing
accurate *p*-values and confidence intervals, ensuring that the
hypothesis tests remained robust even when the homoscedasticity
assumption was violated.

**4.0 Results**
===============

4.1 Introduction
----------------

This chapter presents the quantitative findings of this empirical
investigation into the influence of Large Language Model (LLM) usage on
student learning performance and computational literacy. The analysis is
structured around the three primary research questions:

-   **RQ1:**How does Large Language Model (LLM) influence student
    > learning performance?

-   **RQ2:** When the prompt is adjusted to include assignment
    > instructions (in-context learning), what is the impact on student
    > learning performance?

-   **RQ3:** What is the relationship between large language model use
    > and computational literacy?

As detailed in Chapter 3, the analysis utilized a categorical content
analysis of the student-LLM trace logs, classifying interactions as
either Learning (adaptive help-seeking) or Task Completion (executive
help-seeking). These classifications were aggregated to the participant
level to facilitate multivariate regression analyses, weighing the
relative impacts of these interaction types against academic outcomes.

The findings reveal a nuanced relationship between the mode of LLM
engagement and student performance. This relationship is characterized
by mutual suppression effects, necessitating the simultaneous
consideration of multiple engagement variables to uncover the underlying
statistical relationships.

For RQ1, a non-experimental, observational design was used to examine
associations between naturally occurring LLM engagement patterns and
midterm exam scores (E1). Utilizing hierarchical multiple regression,
this analysis revealed that Learning and Task Completion behaviors
provided unique, contrasting information regarding the variance in
student performance.

For RQ2, a between-subjects randomized controlled trial was employed to
evaluate the effects of the context-aware LLM treatment (T2). While the
treatment showed no initial main effect, a comprehensive multi-stage
analysis revealed a suppressive dynamic. This relationship became
statistically significant only when controlling for Learning and Task
Completion session counts, which served as concurrent measures of
participant engagement during the intervention. This finding suggests
that the impact of context-aware AI on learning performance is only
discernible when accounting for the variance introduced by students\'
specific interaction patterns as they occurred throughout the study.

For RQ3, a non-experimental pre-test/post-test design was utilized to
assess changes in computational literacy (C1, C2). While overall gains
in literacy were statistically significant, an Analysis of Covariance
(ANCOVA) revealed an asymmetrical relationship between usage types and
outcomes. A significant negative correlation was found between Task
Completion frequency and post-intervention literacy scores, while the
relationship with Learning sessions did not reach the threshold for
statistical significance.

The subsequent sections detail the results of these analyses and provide
a formal evaluation of each corresponding hypothesis.

4.2 Findings for RQ1
--------------------

### 4.2.1 Model Overview for RQ1

Research Question 1 (RQ1) investigated whether the frequency and
classification of student interactions with Large Language Models (LLMs)
predicted performance on the midterm exam (E1). Specifically, this
analysis examined the extent to which Learning session counts and Task
Completion session counts were differentially associated with academic
outcomes for the *N = 87* participants.

The primary analysis utilized a multiple linear regression model where
the frequency of each interaction type served as the independent
variables and the E1 score served as the dependent variable:

**Model 3: E1 \~ Learning Session Count + Task Completion Session
Count**

**Hypothesis for H1**

**Alternative Hypothesis (*H*~1~):** The quantity and classification of
participant sessions in the D1 dataset are significantly associated with
midterm exam scores (E1).

-   ***H*~1a~ :** There is a positive correlation between the frequency
    > of sessions Learning sessions and midterm exam scores.

-   ***H*~1b~ :**There is a negative correlation between the quantity of
    > Task Completion sessions and midterm exam scores.

**Null Hypothesis (*H*~01~):** There is no statistically significant
relationship between the quantity of participant sessions, regardless of
classification, and midterm exam scores (E1).

To reject the null hypothesis (***H*~01~**), both conditions
(***H*~1b\ ~**and ***H*~1b~**) must reach statistical significance at
the 𝛼 = .05 level.

### 4.2.2 Regression Assumption Tests of the Model for RQ1

Prior to interpreting the results for RQ1, a comprehensive assessment of
Ordinary Least Squares (OLS) regression assumptions was conducted to
ensure the validity and reliability of the model estimates.

Linearity was evaluated through the examination of partial regression
plots, which assess the relationship between the dependent variable (E1)
and each predictor while controlling for other variables in the model.
Visual inspection of these plots indicated approximate linear
relationships, supporting the application of linear regression. As is
common with session-oriented trace data, both independent variables
exhibited a right-skewed distribution, where the majority of
participants engaged in few sessions and a smaller subset engaged in
many.

![](./publish/thesis2/md/media/image20.png){width="6.5in"
height="4.486111111111111in"}\
*Figure 4.1: Partial regression plots when holding the other constant of
E1 \~ Task Completion Session Count + Learning Session Count.*

The assumption of independence was satisfied, as the Durbin-Watson
statistic (*DW* = 2.09) fell within the acceptable range near the ideal
value of 2.0. To evaluate homoscedasticity, the Breusch-Pagan test was
performed, yielding a non-significant result (*𝝌*^2^= 0.29, *p* = .867).
This indicates that the assumption of constant error variance was met.
These findings were corroborated by the plot of residuals versus fitted
values, which displayed a symmetrical, random scatter with a relatively
flat Locally Estimated Scatterplot Smoothing (LOESS) curve, suggesting
no discernible funneling or non-linear patterns. The end of the LOESS
curve does indicate a slight uptick likely due to lack of observations
in that region.

![](./publish/thesis2/md/media/image10.png){width="5.229166666666667in"
height="3.46875in"}\
*Figure 4.2: Residuals vs Fitted Values for E1 \~ Learning Session Count
+ Task Completion Session Count*

The residuals demonstrated close adherence to a normal distribution, as
evidenced by a non-significant Shapiro-Wilk test (*W* = 0.99, *p* =
.679). Visual inspection of the residuals histogram and the Q-Q plot
further confirmed normality, with data points closely following the
theoretical diagonal line.

![](./publish/thesis2/md/media/image16.png){width="6.5in"
height="2.3055555555555554in"}\
*Figure 4.3: Evidence of normality among the residuals of E1 \~ Task
Completion Session Count + Learning Session Count.*

Multicollinearity was assessed using the Variance Inflation Factor
(VIF). Both predictor variables yielded a *VIF* of 1.19, well below the
conventional threshold of concern (typically \> 5.0) and close to the
target value of 1.0. This indicates that Learning and Task Completion
session counts provide sufficiently unique information to the model.

Given that all diagnostic tests indicated the satisfaction of OLS
assumptions, the model was deemed appropriate for interpretation. The
overall model was statistically significant, *F(2, 84)* = 9.76, *p* \<
.001, and explained 18.9% of the variance in E1 (*R^2^* = .189,
*adjusted R^2^* = .169).

### 4.2.3 Hierarchical Regression Analysis for the RQ1 Model

Prior to evaluating the full multivariate model, bivariate relationships
between each predictor variable and midterm exam scores (*E1*) were
examined through simple linear regression. This preliminary analysis
allowed for the assessment of individual predictor effects and
established a baseline understanding of each independent variable's
isolated contribution to the model before accounting for their combined
influence.

#### 4.2.3.1 Model 0: E1 \~ Session Count

The initial stage of the analysis involved a simple linear regression of
the total session count on the dependent variable *E1*. This established
a baseline to determine if the raw quantity of AI usage, regardless of
classification, impacted exam performance.

A post-hoc power analysis revealed that the model did not achieve the
conventional target of .80 power at an *⍺* = .05 level (Actual Cohen's
*f^2^* = .012, Target *f^2^* = .092). The regression model was not
statistically significant, *F(1, 85)* = 1.01, *p* = .317, with the total
number of sessions explaining only 1% of the variance in *E1* scores
(*R^2\ ^*= .012, *adjusted R^2^* = .000). The regression coefficient was
negative but failed to reach statistical significance (*ꞵ* = -0.06, *SE*
= 0.06, *t* = -1.00, *p* = .317, 95% *CI* \[-0.17, 0.06\]).
Consequently, total session count was not a significant predictor of
exam performance.

![](./publish/thesis2/md/media/image13.png){width="6.5in"
height="4.125in"}\
*Figure 4.4: Forestplot of E1 \~ Session Count*

#### 4.2.3.2 Model 1: E1 \~ Task Complection Session Count

A simple linear regression revealed that Task Completion session count
was a significant negative predictor of E1, *F(1, 85)* = 12.35, *p* \<
.001. The model explained 12.7% of the variance in exam scores (*R^2^* =
.127, *adjusted R^2^* = .117). The model satisfied statistical power
requirements for a target of .80 at an *⍺* = .05 level, as the observed
effect size exceeded the required threshold (Actual Cohen's *f^2\ ^*=
.145, Target *f^2^*= .092).

The regression coefficient indicated that each additional Task
Completion session was associated with a 0.41-unit decrease in E1 score
(*ꞵ* = -0.41, *SE* = 0.12, *t* = -3.52, *p* = .001, 95% *CI* \[-0.65,
-0.18\]). This bivariate relationship confirmed that higher engagement
in behaviors categorized as Task Completion was independently associated
with lower exam performance.\
![](./publish/thesis2/md/media/image21.png){width="6.5in"
height="3.638888888888889in"}

*Figure 4.5: Forestplot of E1 \~Task Completion Session Count*

#### 4.2.3.3 Model 2: E1 \~ Learning Session Count

In contrast, the bivariate relationship between Learning session count
and E1 scores presented a different dynamic. This simple linear
regression model did not meet the assumptions of statistical power for a
target of .80 at an *⍺* = .05 level (Actual *Cohen's f^2\ ^*= .007 \<
Target *Cohen's f^2\ ^*= .092). The model was not statistically
significant, *F(1, 85)* = 0.62, *p* = .435, with sessions classified as
Learning explaining less than 1% of the variance in E1 (*R^2\ ^*= .007,
*adjusted R^2^* = -.004)

The regression coefficient was positive but failed to reach statistical
significance (*ꞵ*= 0.06, *SE* = 0.08, *t* = 0.79, *p* = .435, 95% *CI*
\[-0.10, 0.23\]). These results indicate that Learning session count,
when considered in isolation, was not a significant predictor of exam
performance.![](./publish/thesis2/md/media/image17.png){width="6.5in"
height="3.8472222222222223in"}\
*Figure 4.6: Forestplot of E1 \~ Learning Session Count*

#### 4.2.3.4 Model 3: E1 \~ Learning Session Count + Task Completion Session Count

A distinct and more robust pattern emerged when Task Completion and
Learning session counts were analyzed simultaneously within a multiple
regression framework. The full multivariate model was statistically
significant, *F(2, 84)* = 9.76, *p* \< .001, and satisfied the
requirements for statistical power for a target of .80 at an *⍺* = .05
level (Actual Cohen's *f^2^* = .233, Target *f^2^* = .115). This model
explained 18.9% of the total variance in *E1* scores (*R^2^* = .189,
Adjusted *R^2^* = .169), representing a 48.8% increase in explanatory
power over the Task Completion bivariate model alone (*R^2^*= .127).

A comparison of the bivariate and multivariate results reveals a mutual
suppression effect, where the predictive power of both variables was
enhanced when included together in the model.

-   Task Completion: The negative impact of Task Completion sessions
    > increased by 31% compared to Model 1 (*ꞵ* = -0.54, *SE* = 0.125,
    > *t* = -4.33, *p* \< .001, 95% *CI* \[-0.79, -0.29).

-   Learning: While Learning sessions were non-significant when
    > considered in isolation (Model 2), they became a significant
    > positive predictor of E1 in the full model (*ꞵ* = 0.21, *SE* =
    > 0.081, *t* = 2.53, *p* = .013, 95% *CI* \[0.04, 0.37\]). The
    > standardized coefficient increased from 0.06 to 0.21, representing
    > a magnitude increase of over 200%.

The change in *R^2^* from the Task Completion model to the full model
was statistically significant (*ΔR^2^* = .062), indicating that the
addition of Learning session counts provided 6% of unique explanatory
power beyond what was explained by Task Completion sessions alone. These
results suggest that the relationship between LLM usage and exam
performance is obscured unless both adaptive (Learning) and executive
(Task Completion) help-seeking behaviors are accounted for
simultaneously.

![](./publish/thesis2/md/media/image23.png){width="6.5in"
height="3.638888888888889in"}

*Figure 4.7: Forestplot of E1 \~ Task Completion Session Count +
Learning Session Count*

### 4.2.4 Summary of Findings for RQ1

The comparison across models revealed a mutual suppression effect
between Task Completion and Learning session counts when predicting
midterm exam scores (E1). The predictors shared variance that obscured
their individual relationships with the outcome when considered in
isolation. As demonstrated in the transition from bivariate to
multivariate analysis, the *ꞵ* coefficient for Task Completion sessions
increased in magnitude from -0.41 to -0.54. Simultaneously, Learning
sessions transformed from a non-significant predictor (*p* = .435) to a
significant one (*p* = .013), with the *ꞵ* coefficient increasing more
than threefold from 0.06 to 0.21.

This pattern indicates that each predictor accounted for irrelevant
variance in the other, effectively clearing the signal for their unique
predictive contributions to emerge. The significant increase in
explained variance, specifically *ΔR^2^* of .062 when adding Learning to
the Task Completion model, demonstrates that both session types provided
non-redundant information regarding exam performance.

  ------------------------------------------------------------------------------------------------------------------
  **Model**   **Independent\                     ***R*^2^**   **Adj. *R*^2^**   ***F***   ***p***    ***ΔR^2^**^\
              Variables**                                                                            ^***Model 1**
  ----------- ---------------------------------- ------------ ----------------- --------- ---------- ---------------
  0           Session Count (SC)                 0.012        0.000             1.011     0.317      ---

  1           Task Completion SC                 0.127        0.117             12.35     \< 0.001   ---

  2           Learning SC                        0.007        -0.004            0.62      = 0.435    ---

  3           Task Completion SC + Learning SC   0.189        0.169             9.76      \< 0.001   \+ 0.062
  ------------------------------------------------------------------------------------------------------------------

*Table 4.1: Hierarchical Model Comparison for RQ1*

The observed effects were in direct opposition: Learning sessions
exerted a positive influence ( *ꞵ* = 0.21, while Task Completion
sessions exerted a negative influence ( *ꞵ* = -0.54) that was more than
twice as influential. This suggests that these behaviors represent
competing strategies for academic engagement. The negative relationship
for Task Completion aligns with the theory that surface-level engagement
(executive help-seeking) is less effective for deep learning, while the
positive relationship for Learning sessions reflects the benefits of
adaptive help-seeking.

### 4.2.5 Conclusion for RQ1

The multivariate regression analysis of model 3: E1 \~ Task Completion
Count + Learning Session Count (*F(2, 84)* = 9.76, *p* \< .001) provided
sufficient statistical evidence to reject the null hypothesis
(***H*~01~**). Both hypothesized directional relationships were
confirmed: Learning sessions positively predicted exam performance (*ꞵ*
= 0.21, *p* = .013), while Task Completion sessions negatively predicted
performance (*ꞵ* = -0.54, *p* \< .001).

Consequently, the nature of LLM engagement, rather than the mere
frequency of use, is a significant predictor of academic performance.
Although the correlational nature of this study precludes causal claims,
such as the premise that task completion causes lower scores, the
opposing directional relationships combined with the mutual suppression
effect provide robust evidence that distinct modes of LLM interaction
are uniquely associated with learning outcomes.

4.3 Findings for RQ2
--------------------

### 4.3.1 Model Overview for RQ2

Research Question 2 (RQ2) utilized a between-subjects experimental
design to investigate the impact of in-context learning (ICL) on midterm
exam scores (E1). During the six-week intervention, participants were
randomly assigned to either the control group (*n* = 48) or the
treatment group (*n* = 39). The treatment group utilized an LLM
contextually aware of specific assignment instructions and thus was
capable of scaffolding dialog based on those instructions. The analysis
examined whether this treatment resulted in improved academic
performance on the summative assessment.

To evaluate the impact of the intervention, a linear regression model
was employed using a dummy-coded independent variable (*0 = control, 1 =
treatment*), with E1 scores as the dependent variable:

**Model 0: E1 \~ Treatment (Total Effect)**

**Hypothesis for RQ2**

-   **Alternative Hypothesis (*H*~2~):** The mean student learning
    > performance score (E1) for the treatment group (context-aware AI)
    > will be statistically significantly higher than the mean score for
    > the control group.

-   **Null Hypothesis (*H*~02~):** There is no statistically significant
    > difference in the mean student learning performance scores (E1)
    > between the treatment and control groups.

### 4.3.2 Regression Assumption Tests for the RQ2 Model

Prior to interpreting the results for the RQ2 total effect model, an
assessment of Ordinary Least Squares (OLS) regression assumptions was
conducted to ensure the validity and reliability of the model estimates.

Because the independent variable is binary *(0 = control, 1 =
treatment)*, the assumption of linearity is inherently satisfied. The
regression effectively estimates the difference in means between the two
groups, which is a linear relationship by definition. The Durbin-Watson
statistic (*DW* = 2.11) fell within the acceptable range near 2.0,
indicating no evidence of autocorrelation and confirming the
independence of residuals.

To evaluate the assumption of constant variance, the Breusch-Pagan test
was administered. The test yielded a non-significant result (*𝝌*^2^ =
0.081, *p* = .776), indicating that the residuals exhibited
homoscedasticity across the range of fitted values. This suggests that
the variance of exam scores (E1) remained constant across both the
control and treatment groups.

The Shapiro-Wilk test was utilized to verify the normality of residuals.
The result was non-significant (*W* = 0.98, *p* = .167), suggesting that
the residuals approximated a normal distribution. This finding was
corroborated visually through a histogram of residuals and a Q-Q plot,
both of which demonstrated close adherence to the theoretical normal
distribution line.

![](./publish/thesis2/md/media/image4.png){width="6.5in"
height="2.3055555555555554in"}\
*Figure 4.8: Evidence of normality among the residuals of E1 \~
Treatment*

The Variance Inflation Factor (VIF) for the treatment variable was 1.00.
This indicates a complete absence of multicollinearity, as expected in a
simple linear regression model with a single predictor.

Given that all diagnostic tests indicated the satisfaction of OLS
regression assumptions, the model was deemed appropriate for formal
interpretation.

### 4.3.3 Regression Analysis for the RQ2

#### 4.3.3.1 Model 1: Total Effect for RQ2

The total effect was for RQ2 was represented by the following Model:

**Model 1: E1 \~ Treatment**

The initial regression model examined the total effect of the treatment
on midterm exam performance. The control group (*n* = 48) achieved a
mean *E1* score of 30.23 points (*SE* = 0.87). Participants in the
treatment group (*n* = 39), who utilized the context-aware AI, scored an
average of 2.05 points higher than the control group (*ꞵ* = 2.05, SE =
1.30). However, this mean difference did not reach statistical
significance (*p* = .119, 95% *CI* \[-0.54, 4.64\]). The 95% confidence
interval crossed the zero boundary, indicating that the null hypothesis
of no difference between the population means could not be rejected at
this stage.

![](./publish/thesis2/md/media/image6.png){width="6.5in"
height="3.9722222222222223in"}\
*Figure 4.9: Forestplot of E1 \~ Treatment*

The overall model fit was weak, with group assignment accounting for
only 2.8% of the variance in E1 scores (*R^2^* = .028, Adjusted *R^2^* =
.017). The *F*-statistic was not significant, *F(1, 85)* = 2.49, *p* =
.119, indicating that the model did not explain a statistically
significant proportion of the variance in exam performance. Furthermore,
the model did not meet the conventional threshold for statistical power
(Actual Cohen's *f^2^* = .029, Target *f^2^* = .092). This effect size
falls below the threshold for a small effect, suggesting that the
practical significance of the group differences was minimal in
isolation.

These findings suggest that providing an AI assistant with
assignment-specific context did not immediately translate into
measurably improved exam performance. The lack of a significant main
effect may indicate that the in-context learning (ICL) manipulation did
not sufficiently alter learning outcomes in ways captured by the
summative assessment alone, potentially due to unaccounted factors such
as prior domain expertise or AI-prompting proficiency.

However, given the significant relationships established in RQ1 between
usage patterns and performance, a more granular examination of these
factors as process variables was warranted. The following sections
explore how the treatment interacted with Learning and Task Completion
behaviors through mediation and moderation analyses to reveal the
underlying impact of the intervention.

#### 4.3.3.2 Models 2 a/b: Mediation Analysis for RQ2

The findings from RQ1 established that AI-mediated help-seeking
behaviors, specifically Learning and Task Completion sessions,
significantly influence midterm exam performance (E1). To explore
whether the treatment effect operated through changes in these student
behaviors, a mediation analysis was conducted. This analysis sought to
determine if the context-aware intervention in the treatment influenced
exam scores by altering the frequency of Learning or Task Completion
interactions with the AI. This required two additional regression models
to test the \"a-path\" of the mediation framework:

-   **Model 2a: Learning Session Count \~ Treatment**

-   **Model 2b: Task Completion Session Count \~ Treatment**

For Model 2a, the linear regression revealed that treatment group
assignment did not significantly predict Learning session counts (*ꞵ* =
-1.79, *SE* = 1.73, *t(85)* = -1.04, *p* = .304, *R^2^* = .012).
Furthermore, the model did not achieve the target statistical power
(Actual Cohen's *f^2^* = .013 vs. Target *f^2^* = .092). Descriptively,
control group students engaged in more learning sessions (*M* = 7.79,
*SD* = 8.18) compared to treatment group students (*M* = 6.00, *SD* =
7.85), though this difference was not statistically significant.

Model 2b was also found to be statistically non-significant. Treatment
group assignment did not significantly predict Task Completion session
counts (*ꞵ* = 0.47, *SE* = 1.14, *t(85)* = 0.42, *p* = .678, *R^2^* =
.002). Descriptively, treatment group students demonstrated slightly
higher task-completion activity (*M* = 4.41, *SD* = 5.30) relative to
control group students (*M* = 3.93, *SD* = 5.24).

The absence of significant relationships between treatment assignment
and AI usage patterns in Models 2a and 2b precludes the existence of a
mediation effect. According to established mediation frameworks [(Hayes,
2009)](https://www.zotero.org/google-docs/?yKu1Fr) an indirect effect
requires the predictor to significantly influence the proposed
mediators. Therefore, these results indicate that the treatment's impact
on exam performance did not operate through a quantitative shift in
student usage behaviors.

#### 4.3.3.3 Models 3 a/b: Moderation Analysis for RQ2

To further investigate the intervention\'s mechanics, two moderation
analyses were conducted to determine whether the treatment condition
altered the strength or direction of the relationship between AI usage
patterns and exam performance. These models tested whether the
interaction between group assignment and session classification
significantly predicted E1 scores.

**Model 3a: Interaction of Treatment and Learning Sessions**

The first moderation model examined whether context-aware AI moderated
the relationship between Learning session frequency and exam
performance:

**E1 \~ Treatment + Learning Session Count + Treatment x Learning
Session Count**

The overall model was not statistically significant, *F(3, 83)* = 1.29,
*p* = .284, *R^2^* = .045. The interaction term (Treatment x Learning)
was non-significant (*ꞵ* = 0.11, *SE* = 0.17, *t(83)* = 0.68, *p* =
.502, 95% *CI* \[-0.22, 0.44\]), indicating that the treatment did not
moderate the impact of learning behaviors. Additionally, neither the
main effect of treatment (*ꞵ* = 1.44, *p* = .407) nor the main effect of
Learning sessions (*ꞵ* = 0.03, *p* = .769) reached significance in this
specific model.

**Model 3b: Interaction of Treatment and Task Completion Sessions**

The second moderation model examined whether the treatment moderated the
relationship between Task Completion frequency and exam performance:

**E1 \~ Treatment + Task Completion Session Count + Treatment x Task
Completion Session Count**

While the overall model was statistically significant (*F(3, 83)* =
5.35, *p* = .002, *R^2^* = .162), the interaction term (Treatment x Task
Completion) remained non-significant (*ꞵ* = -0.07, *SE* = 0.24, *t(83)*
= -0.32, *p* = .753, 95% *CI* \[-0.54, 0.39\]). The model confirmed a
significant negative main effect for Task Completion sessions (*ꞵ* =
-0.39, *SE* = 0.16, *t(83)* = -2.47, *p* = .016), consistent with RQ1
findings. The main effect for treatment approached but did not reach
statistical significance (*ꞵ* = 2.56, *SE* = 1.57, *p* = .107).

The lack of significant interaction effects in both models suggests that
the treatment condition did not alter the fundamental relationship
between usage patterns and academic outcomes. Learning sessions appear
to support exam performance, and Task Completion sessions appear to
hinder exam performance, with consistent intensity across both the
control and treatment groups.

#### 4.3.3.4 Model 4: Identification of RQ2 Treatment Effect via Suppression Analysis

Having established that the intervention did not significantly shift the
volume of AI usage (Mediation) or the nature of the relationship between
usage and grades (Moderation), a final analysis was conducted to examine
the treatment\'s impact while accounting for concurrent usage patterns.
In this model, Learning and Task Completion sessions are treated as
process variables. Because these behaviors occurred simultaneously with
the intervention, they represent noise or confounding variance that may
obscure the direct impact of the context-aware treatment. This analysis
sought to determine if the treatment was effective when comparing
students with equivalent levels of AI engagement.

**E1 \~ Treatment + Task Completion Session Count + Learning Session
Count**

A multiple regression analysis was conducted including Treatment,
Learning session count, and Task Completion session count as predictors
of E1 performance. The model was statistically significant, *F(3, 83)* =
8.64, *p* \< .001, and explained 23.8% of the variance in exam scores
(*R^2^* = .238, Adjusted *R^2^* = .210). This represents a substantial
increase in explanatory power over the baseline Model 1 (*R^2^* = .028).
The observed effect size (Cohen's *f^2^* = .312) indicates a
medium-to-large effect and exceeded the threshold for a statistical
power of .80 (Target *f^2^* = .131).

When controlling for the frequency of Learning and Task Completion
sessions, the treatment effect became statistically significant (*ꞵ* =
2.74, *SE* = 1.18, *t(83)* = 2.32, *p* = .023, 95% *CI* \[0.39, 5.09\]).
On average, participants in the treatment group scored 2.74 points
higher on the midterm exam than control group students with identical
LLM usage patterns.

This finding carries an important caveat: the 2.74-point advantage is a
*conditional effect.* For example, if two participants---one from the
control group and one from the treatment group---exhibited the exact
same counts of learning and task-completion behaviors, the student in
the treatment group would be predicted to score approximately 2.74
points higher due to the context-aware enhancement of the AI.

Both session types maintained significant relationships with exam
performance after accounting for the treatment. Consistent with the
findings in RQ1, Learning session counts remained a significant positive
predictor (*ꞵ* = 0.23, *SE* = 0.08, *t(83)* = 2.90, *p* = .005\$), while
Task Completion counts demonstrated a significant negative relationship
(*ꞵ* = -0.57, *SE* = 0.12, *t(83)* = -4.65, *p* \< .001).

![](./publish/thesis2/md/media/image8.png){width="6.5in"
height="3.5833333333333335in"}\
*Figure 4.10: Forestplot of E1 \~ Treatment + Learning Session Count +
Task Completion Session Count*

The emergence of statistical significance only after the inclusion of
covariates indicates a suppression effect. Although the treatment did
not significantly alter student usage volume, those usage patterns
accounted for a large portion of the variance in exam scores. By
including them in the model, the noise associated with individual
student strategy (adaptive vs. executive help-seeking) was partitioned
out, allowing the true signal of the treatment effect to be identified.
The results indicate that the context-aware treatment (T2) provides a
performance advantage that is independent of the frequency of
engagement. While the intervention did not alter the quantity of
student-AI interactions, it enhanced the efficacy of those interactions.
This implies that the treatment\'s value lies in the quality of the
scaffolding provided rather than in a fundamental shift in student
help-seeking volume.

### 4.3.4 Summary of Findings for RQ2

The following table summarizes the analytical findings for RQ2.

+-----------+-----------------+-----------------+-----------------+
| **Model** | **Analysis      | **Key Finding** | **Conclusion**  |
|           | Type**          |                 |                 |
+===========+=================+=================+=================+
| 1         | Total Effect\   | Treatment not   | Initial null    |
|           | E1 \~ Treatment | significant     | finding. This   |
|           |                 | p=0.119         | led to further  |
|           |                 |                 | investigations. |
+-----------+-----------------+-----------------+-----------------+
| 2a        | Mediation\      | No mediation    | Treatment       |
|           | Learning SC\~   | path\           | doesn't change  |
|           | Treatment       | p = 0.304       | Learning SC     |
+-----------+-----------------+-----------------+-----------------+
| 2b        | Mediation       | No mediation    | Treatment       |
|           |                 | path\           | doesn't change  |
|           | Task Completion | p = 0.678       | Task Completion |
|           | SC \~ Treatment |                 | SC              |
+-----------+-----------------+-----------------+-----------------+
| 3a        | Moderation\     | No moderation\  | Treatment       |
|           | E1 \~ Treatment | p = 0.502       | doesn't amplify |
|           | + Learning SC+\ |                 | learning SC     |
|           | Treatment x     |                 |                 |
|           | Learning SC     |                 |                 |
+-----------+-----------------+-----------------+-----------------+
| 3b        | Moderation\     | No moderation\  | Treatment       |
|           | E1 \~ Treatment | p = 0.753       | doesn't amplify |
|           | +\              |                 | task completion |
|           | Task Completion |                 | SC              |
|           | SC +\           |                 |                 |
|           | Treatment x     |                 |                 |
|           | Task Completion |                 |                 |
|           | SC              |                 |                 |
+-----------+-----------------+-----------------+-----------------+
| 4         | Suppression\    | Treatment       | Suppression     |
|           | E1 \~ Treatment | significant     | effect revealed |
|           | + Learning SC + | when            | when            |
|           | Task Completion | controlling for | controlling for |
|           | SC              | usage (beta =   | patterns of     |
|           |                 | 2.74, p =       | usage.          |
|           |                 | 0.023)          |                 |
+-----------+-----------------+-----------------+-----------------+

*Table 4.2: Analytical Findings for RQ2. Note: SC is an abbreviation for
Session Count*

The initial assessment of the treatment effect (Model 1) revealed a null
result. While the treatment group demonstrated a mean increase of 2.05
points over the control group, this difference failed to reach
statistical significance (*p* = .119). In the subsequent exploratory
analysis (Model 4), which controlled for the Learning and Task
Completion session counts identified in RQ1, the model's precision
increased substantially. This multivariate approach accounted for 23.8%
of the variance in *E1* scores, a significant improvement over the 2.8%
explained by the baseline model.

However, because these usage patterns were observed and measured after
the random assignment of treatment conditions, controlling for them
introduces complexity regarding causal interpretation. While the
mediation analysis confirmed that the treatment did not significantly
influence the volume of Learning or Task Completion sessions, the
inclusion of these post-treatment variables may still introduce bias.

Controlling for post-randomization variables can lead to post-treatment
bias, which complicates the isolation of a pure causal link. In this
analysis, however, accounting for the massive variance in student
help-seeking behaviors was necessary to identify the underlying signal
of the intervention. Rather than providing a pure causal estimate of the
\"Intent-to-Treat,\" Model 4 offers an estimate of the treatment's
intrinsic efficacy when behavioral noise is partitioned out. Therefore,
these findings are most responsibly interpreted as a conditional effect
rather than a definitive causal one.

### 4.3.5 Conclusion for RQ2

The multi-stage analysis of Research Question 2 (RQ2) provides the
statistical basis to reject the null hypothesis (***H*~02~**). Although
the initial baseline model 1 indicated no significant mean difference
between groups, the inclusion of Learning and Task Completion session
counts as process variables revealed a significant treatment effect. The
multivariate regression *F(3, 83)* = 8.64, *p* \< .001) confirmed that
when accounting for the variance in student usage patterns, participants
in the treatment group outperformed those in the control group by an
average of 2.74 points (*ꞵ* = 2.74, *p* = .023).

These findings suggest that the impact of the context-aware intervention
in this study was conditional upon usage behavior. Because the
intervention did not significantly change the frequency of student
interactions (Mediation) or the relationship between those interactions
and E1 grades (Moderation), the treatment\'s value appears to be
intrinsic to the quality of the AI\'s responses. Specifically, the
treatment improved exam performance independently of how often a student
used the tool; for any given level of engagement, the context-aware LLM
provided a more effective learning support than the standard LLM.

Consequently, while the raw treatment effect was obscured by the high
degree of variability in student engagement strategies, partitioning out
that behavioral noise revealed that in-context learning (ICL)
significantly improved exam scores when controlling for identical
patterns of AI usage. Therefore, this effect should be interpresented as
conditional instead of causal.

4.4 Findings for RQ3 
--------------------

### 4.4.1 Model Overview for RQ3

Research Question 3 (RQ3) investigated the relationship between the
frequency of Learning and Task Completion sessions and participants\'
computational literacy outcomes (*N* = 87). This analysis sought to
determine if AI engagement patterns predicted post-intervention literacy
scores (C2) while controlling for baseline literacy levels (C1).

To isolate the impact of AI engagement from prior knowledge and
potential test-retest effects, an Analysis of Covariance (ANCOVA)
approach was utilized. In this model, the pre-test score (C1) served as
a covariate, with Learning and Task Completion session counts as the
primary independent variables:

**Model 1: C2 \~ Learning Session Count + Task Completion Session Count
+ C1**

In addition to the ANCOVA, a supplementary analysis was conducted using
the change score (ΔC = C2 - C1) as the dependent variable to examine
whether LLM usage patterns predicted the magnitude of literacy
improvement. Because change scores can exhibit lower reliability when
pre- and post-test scores are highly correlated [(Cronbach & Furby,
1970)](https://www.zotero.org/google-docs/?2wjkP7), this was treated as
a complementary validation of the primary model:

**Model 1a: C2-C1 \~ Learning Session Count + Task Completion Count**

**Hypothesis FOR RQ3**

**Alternate Hypothesis (*H*~3~):** The frequency and classification of
participant sessions are significantly associated with computational
literacy outcomes.

-   ***H*~3a~ :** There is a positive association between the quantity
    > of sessions classified as Learning and computational literacy
    > scores.

-   ***H*~3b~ :** There is a negative association between the quantity
    > of sessions classified as Task Completion and computational
    > literacy scores.

**Null Hypothesis for (*H*~03~):** There is no statistically significant
relationship between the frequency of participant sessions, regardless
of classification, and computational literacy outcomes.

To reject the null hypothesis (***H*~03~**), both directional conditions
(***H*~3a\ ~**and ***H*~3b\ ~**) must reach statistical significance at
the *⍺* = .05 level.

### 4.4.2 Regression Assumption Tests for the RQ3 Model

Prior to interpreting the findings for RQ3, a comprehensive assessment
of Ordinary Least Squares (OLS) regression assumptions was conducted to
ensure the validity and reliability of the model estimates.

Preliminary diagnostic testing revealed a violation of the
homoscedasticity assumption. The Breusch-Pagan test was significant
(*𝝌*^2^ = 12.58, *p* = .006), indicating non-constant error variance
across the range of fitted values. This was confirmed visually by the
cone-like distribution of residuals in the diagnostic plots. To ensure
valid statistical inference, heteroscedasticity-consistent (HC) robust
standard errors were used for all regression results. This approach
provides robust hypothesis tests and accurate *p*-values and confidence
intervals, even when error variance is not constant.

![](./publish/thesis2/md/media/image9.png){width="6.5in"
height="4.486111111111111in"}\
*Figure 4.11: Partial regression plots when holding the other constant
of C2 \~ Task Completion Session Count + Learning Session Count. + C1
with Visual Confirmation of Heteroscedasticity.*

Linearity was evaluated via partial regression plots, which assess the
relationship between the dependent variable (C2) and each predictor
while controlling for others in the model. Visual inspection indicated
approximate linear relationships, though heteroscedasticity remained
visually apparent. As observed in previous models, the session-oriented
independent variables exhibited a right-skewed distribution, with fewer
observations at higher session counts.

The plot of residuals versus fitted values showed symmetrical, randomly
scattered points. Heteroscedasticity can be observed on the right end of
the graph. The Locally Estimated Scatterplot Smoothing (LOESS) curve was
relatively flat and hovering about horizontal.

![](./publish/thesis2/md/media/image24.png){width="5.166666666666667in"
height="3.46875in"}\
*Figure 4.12: Residuals vs Fitted Values for C2 \~ Learning Session
Count + Task Completion Session Count + C1*

The Durbin-Watson statistic (*DW* = 2.22) fell within the acceptable
range near 2.0, indicating no substantial autocorrelation and satisfying
the assumption of independence. The residuals demonstrated close
adherence to a normal distribution, as evidenced by a non-significant
Shapiro-Wilk test (*W* = 0.99, *p* = .551). This finding was
corroborated visually by a histogram of residuals and a Q-Q plot, both
of which showed the data points closely following the theoretical normal
line.

![](./publish/thesis2/md/media/image11.png){width="6.5in"
height="2.2777777777777777in"}\
*Figure 4.13: Evidence of normality among the residuals of C2 \~ Task
Completion Session Count + Learning Session Count + C1*

Multicollinearity was assessed using the Variance Inflation Factor
(VIF). All independent variables reported VIF values below 1.27, with
the C1 covariate at 1.07. These values are well below the conventional
threshold of concern, indicating that the predictors provide unique
information to the model without problematic redundancy.

### 4.4.3 Model 1: ANCOVA for RQ3 Accounting for Baseline Literacy

Descriptive statistics indicated that computational literacy scores
increased significantly from pre-test (C1: *M* = 20.57, *SD* = 4.71) to
post-test (C2: *M* = 21.44, *SD* = 4.78), paired *t(86)* = -2.67, *p* =
.009, Cohen\'s *d* = 0.29. These results reflect modest yet
statistically significant learning gains over the intervention period.
As expected for a repeated measures instrument, C1 and C2 scores were
strongly correlated (*r* = .79, *p* \< .001), suggesting high
test-retest reliability. This combination of significant improvement and
strong correlation justifies the Analysis of Covariance (ANCOVA)
approach, which preserves individual trajectories while controlling for
baseline differences.

**Model 1: C2 \~ Task Completion + Learning+ C1**

This model was highly significant, *F(3, 83)* = 54.66, *p* \< .001, and
explained 65.8% of the variance in post-test scores (*R^2^* = .658\$,
Adjusted *R^2^* = .646). The effect size was large (Cohen's *f^2^* =
1.93) and exceeded the target threshold for .80 statistical power
(*f^2^* = .131).

As anticipated, baseline computational literacy was the strongest
predictor of post-test performance (*ꞵ* = 0.76, *SE* = 0.08, *z* =
10.07, *p* \< .001, 95% *CI* \[0.61, 0.91\]). For every 1-point increase
in C1, post-test scores increased by an average of 0.76 points when
holding session counts constant.

After controlling for baseline ability (C1), Task Completion session
count remained a significant negative predictor (*ꞵ* = -0.17, *SE* =
0.07, *z* = -2.52, *p* = .012, 95% *CI* \[-0.30, -0.04\]). Each
additional task completion session was associated with a 0.17-point
decrement in final computational literacy scores, suggesting that
executive help-seeking behaviors predicted lower final achievement than
would be expected based on initial competency levels. This effect
remained significant after the application of heteroscedasticity-robust
standard errors, confirming the stability of the finding.

Learning session count demonstrated a positive relationship that
approached but did not achieve conventional statistical significance
(*ꞵ* = 0.07, *SE* = 0.04, *z* = 1.76, *p* = .078, 95% *CI* \[-0.01,
0.14\]). While this directional relationship aligns with the findings in
RQ1 and RQ2, the marginal *p*-value suggests that the beneficial impact
of learning-oriented LLM usage on computational literacy may require a
larger sample size or more granular measurement to confirm
statistically.

![](./publish/thesis2/md/media/image19.png){width="6.5in"
height="3.5972222222222223in"}\
*Figure 4.14: Forestplot of C2 \~ Learning Session Count + Task
Completion Session Count + C1*

#### 4.4.3.1 Model 1a: Supplementary Analysis Change in Scores

A supplementary regression analysis was conducted to examine whether LLM
usage patterns predicted the absolute magnitude of improvement rather
than final performance adjusted for baseline standing. In this model,
the change score (ΔC = C2 - C1) served as the dependent variable, with
Learning and Task Completion session counts as the predictors. Unlike
the ANCOVA approach in Model 1, this analysis focuses on the raw
variance in student gains without adjusting for initial baseline
differences.

**Model 1a: C2 - C1 \~ Learning Session Count + Task Completion Count**

Model 1a satisfied all OLS regression assumptions, including
homoscedasticity (Breusch-Pagan: (*𝝌*^2^ = 0.56, *p* = .752),
independence of residuals (Durbin-Watson: *DW* = 1.97), and normality of
residuals (Shapiro-Wilk: *p* = .643\$). Multicollinearity was not a
concern, with VIF scores remaining at 1.19. However, the overall model
was not statistically significant, *F(2, 84)* = 1.57, *p* = .214,
accounting for only 3.6% of the variance in gain scores (*R^2^* = .036,
Adjusted *R^2^* = .013).

Neither Task Completion session count (*ꞵ* = -0.11, *SE* = 0.07, *t* =
-1.67, *p* = .099, 95% *CI* \[-0.25, 0.02\]) nor Learning session count
(*ꞵ* = 0.05, *SE* = 0.04, *t* = 1.22, *p* = .225, 95% *CI* \[-0.03,
0.14\]) significantly predicted the change in computational literacy
scores. While the direction of these relationships remained consistent
with the findings in Model 1---with task completion trending negatively
and learning sessions trending positively---neither effect reached
statistical significance in this absolute-change framework.

The objective of this supplementary analysis was to determine if usage
patterns impacted absolute improvement differently than relative
standing. The results suggest that while Task Completion sessions were
significantly associated with lower post-test outcomes when adjusting
for baseline ability (Model 1), they did not significantly predict the
raw magnitude of score changes from C1 to C2. The lack of significance
in Model 1a highlights the importance of the ANCOVA approach in Model 1,
as controlling for baseline variance was necessary to identify the
subtle relationships between AI interaction types and literacy
development.

### 4.4.4 Summary of Findings for RQ3

The findings for Research Question 3 (RQ3) demonstrate that the
relationship between LLM engagement and computational literacy is highly
dependent on the nature of the interaction. While Model 1 (ANCOVA)
provided significant insights by controlling for baseline ability, the
supplementary change-score model (Model 1a) was non-significant,
suggesting that usage patterns primarily influenced relative final
standing rather than absolute growth magnitude.

  ------------------------------------------------------------------------------------------------------------------------------------------------------------
  **Model**               **Independent Variables**            **Dependent Variables**   **Findings**
  ----------------------- ------------------------------------ ------------------------- ---------------------------------------------------------------------
  1 (ANCOVA)              Learning Session Count +\            C2                        Statistical significance except for Learning Session Count p = 0.08
                          Task Completion Session Count + C1                             

  1a (Change in Scores)   Learning Session Count +\            C2-C1                     Not statistically significant.
                          Task Completion Session Count                                  
  ------------------------------------------------------------------------------------------------------------------------------------------------------------

Table 4.3: Summary of Findings for RQ3

The analysis from Model 1 reveals that Task Completion sessions have a
robust negative association with computational literacy (*ꞵ* = -0.17,
*p* = .012\$). Participants who engaged in higher frequencies of
executive help-seeking achieved lower C2 scores than predicted by their
baseline competency. This suggests that instrumental or
shortcut-oriented LLM use may constrain the development of computational
literacy relative to a student\'s potential.

Conversely, Learning session counts exhibited a positive trend (*ꞵ* =
0.07, *p* = .078) but did not reach the threshold for statistical
significance. While this finding is statistically inconclusive, the
direction of the effect aligns with theoretical expectations and the
results from RQ1 and RQ2, suggesting that exploratory engagement may
support literacy development in ways that instrumental use does not.

### 4.4.5 Conclusion for RQ3

The alternative hypothesis (*H*~3~) proposed that LLM usage patterns
would significantly correlate with computational literacy scores,
specifically predicting a negative correlation for Task Completion
sessions and a positive correlation for Learning sessions. Based on the
results of Model 1, *H*~3~ was partially supported.

The predicted negative relationship between Task Completion session
frequency and computational literacy was confirmed (*ꞵ* = -0.17, *p* =
.012). This effect remained significant after controlling for baseline
ability (C1) and utilizing heteroscedasticity-robust standard errors.
Therefore, the null hypothesis regarding Task Completion sessions is
rejected.

However, the predicted positive relationship between Learning sessions
and computational literacy did not achieve statistical significance at
the conventional *⍺* = .05 threshold (*ꞵ* = 0.07, *p* = .078). Although
the direction of the relationship was consistent with the experimental
findings in RQ1 and RQ2, the marginal *p*-value precludes the rejection
of the null hypothesis for Learning sessions.

In summary, because the overall multivariate model was highly
significant (*F(3, 83)* = 54.66, *p* \< .001) and Task Completion
demonstrated a robust predictive relationship, it can be concluded that
LLM usage patterns are significantly related to computational literacy
outcomes. However, the strength and direction of these associations are
contingent upon whether the student utilizes the AI for executive task
completion or adaptive learning.

4.5 Overall Summary of Findings
-------------------------------

This chapter presented the results of a multi-method investigation into
the relationships between LLM interaction types, experimental
context-aware interventions, and learning outcomes. By partitioning AI
usage into Learning (adaptive) and Task Completion (executive) sessions,
this study identified distinct pathways through which Generative AI
influences academic performance.

RQ1 explored the dual nature of AI engagement and its impact on
learning, as measured by the midterm exam (E1). The analysis established
that usage classification---specifically the intent behind the
help-seeking behavior---rather than aggregate usage volume, is the
primary driver of learning outcomes.

The comprehensive model (Model 3), which included both Learning and Task
Completion session counts as independent variables, demonstrated strong
statistical significance (*F(2, 84)* = 9.76, *p* \< .001), providing
sufficient evidence to reject the null hypothesis. With a medium effect
size (Cohen's *f^2^* = 0.23), the model explained 18.9% of the variance
in midterm exam performance (*R^2^* = .189).

Both hypothesized relationships were confirmed:

-   Learning sessions positively predicted exam performance (*ꞵ* = 0.21,
    > *p* = .013), indicating that adaptive help-seeking supports
    > knowledge acquisition.

-   Task Completion sessions negatively predicted performance (*ꞵ* =
    > -0.54, *p* \< .001), suggesting that executive help-seeking (e.g.,
    > shortcutting) hinders academic achievement.

Hierarchical regression revealed a mutual suppression effect, where the
inclusion of both independent variables together yielded the most
precise model for explaining midterm exam performance compared to models
analyzing each variable independently. By accounting for the
countervailing effects of these usage types, the analysis isolated the
unique contribution of each to student success. Ultimately, these
findings provided the necessary behavioral framework to interpret the
subsequent experimental results in RQ2 and RQ3.

RQ2 investigated the impact of a context-aware AI intervention on
midterm performance through a randomized controlled trial. While the
initial \"Intent-to-Treat\" analysis (Model 1) demonstrated a null
result, the subsequent suppression analysis (Model 4) identified a
significant treatment effect (*ꞵ* = 2.74, *p* = .023) once student usage
behaviors were included as covariates. This suggests that the treatment
did not fundamentally alter the *volume* of AI engagement, but rather
enhanced the *quality* and efficacy of those interactions.

The suppression pattern indicates that usage behaviors as materialized
through Learning and Task Completion session counts, accounted for a
large portion of the variance in exam scores without being influenced by
the treatment itself. By controlling for these variables, the noise of
individual student help-seeking strategies was partitioned out,
revealing the treatment\'s underlying benefit. In addition, the fact
that these variables did not function as mediators (the treatment
didn\'t change the amount of use) or moderators (the treatment didn\'t
change the nature of the relationship between use and grades) strongly
supports the interpretation that the treatment provided an independent,
qualitative benefit.

Ultimately, Model 4 should be interpreted as a conditional effect rather
than a pure causal one. Because Learning and Task Completion counts were
measured post-randomization, standard causal inference is subject to
potential post-treatment bias. Consequently, the finding is best
understood as an estimate of the treatment's intrinsic
efficacy---demonstrating that for any given level of AI engagement, the
context-aware version resulted in superior academic performance.

RQ3 confirmed that the dual nature of AI usage patterns extends beyond
immediate exam performance to the broader development of computational
literacy. Using an ANCOVA approach (Model 1), the analysis demonstrated
that Task Completion sessions have a robust negative relationship with
literacy outcomes (*ꞵ* = -0.17, *p* = .012), even when adjusting for
participants\' baseline ability (C1).

While Learning sessions trended positively, the effect was marginal (*ꞵ*
= 0.07, *p* = .078) and did not reach statistical significance. This
suggests that in the short term, maladaptive AI use (executive
help-seeking) may be a more potent inhibitor of literacy development
than adaptive use is a facilitator. Although the positive relationship
for learning sessions remains suggestive and warrants further
investigation with larger samples, the overall regression model was
highly significant, *F(3, 83)* = 54.66, *p* \< .001.

In conclusion, these findings indicate that LLM usage patterns are
significantly related to computational literacy development, with the
crucial caveat that the direction and strength of this relationship are
contingent upon the specific type of AI engagement.

In summary, an important finding was the importance of Collectively,
these results suggest that the integration of LLMs in education is a
\"double-edged sword.\" The benefit of advanced features, such as
in-context learning and assignment-awareness, can be identified only
when accounting for the student\'s help-seeking strategy. While the
technology provides a significant performance advantage for any given
level of use, the persistent negative impact of shortcut-oriented
behaviors remains a critical challenge for instructional

Chapter 4 demonstrated that aggregate LLM usage volume is an inadequate
predictor of academic success, as the impact of AI engagement is
fundamentally determined by the type of interaction rather than the
quantity. Across all three research questions, the distinction between
Learning (adaptive) and Task Completion (maladaptive) sessions served as
the essential mechanism for uncovering significant results: in RQ1, this
classification revealed the opposing effects of AI on exam performance;
in RQ2, it acted as a vital suppressor that unmasked a significant
treatment effect for the context-aware intervention; and in RQ3, it
identified executive help-seeking as a specific inhibitor of
computational literacy development. Collectively, these findings
establish that the educational value of Generative AI is a conditional
phenomenon, requiring a granular understanding of student help-seeking
intent to accurately measure its influence on learning outcomes.

**5.0 Summary**
===============

5.1 Introduction
----------------

This chapter provides an interpretive analysis of the study's findings,
synthesizing the statistical results into a cohesive narrative. The
discussion first contextualizes these results within the existing
theoretical literature, identifying areas where this research supports,
contradicts, or extends the current academic landscape. Particular
attention is paid to the causal implications of the findings and their
contribution to the broader discourse on Generative AI in education.

The latter portion of the chapter focuses on the practical application
of this research. It includes a critical evaluation of the study's
limitations, followed by a discussion of the practical and theoretical
implications for researchers, educators, and students**.** Finally,
these insights are used to formulate suggestions for future research,
concluding with a final summary of the thesis's salient points and
overarching themes.

### 5.1.1 Research and Key Findings At a Glance

This thesis investigated the impact of **L**arge Language Model (LLM)
integration on student performance and computational literacy within an
introductory Python programming course. Utilizing a multi-methods
approach, student-AI interactions were captured and classified via
categorical content analysis into two competing strategies: Learning
sessions (adaptive help-seeking characterized by scaffolding and
questioning) and Task Completion sessions (executive help-seeking
characterized by cognitive offloading and delegation).

These categorized interactions served as the primary independent
variables for assessing academic outcomes, specifically midterm exam
scores (*E1*) and post-intervention computational literacy (*C2*).
Additionally, a randomized controlled trial assessed the efficacy of a
context-aware LLM enhancement. The empirical findings of this research
can be distilled into four key conclusions:

**Finding 1: The Essentiality of Usage Classification.** A mutual
suppression effect established that aggregate AI use is an inadequate
predictor of success. The true relationship between AI engagement and
academic outcomes was only revealed when accounting for the
countervailing effects of adaptive and executive help-seeking.

**Finding 2: The Negative Impact of Executive Help-Seeking**
.Participants who utilized the LLM for Task Completion (seeking direct
answers or delegating cognitive labor) exhibited a statistically
significant negative correlation with both midterm exam scores and
computational literacy gains.

**Finding 3: The Positive Impact of Adaptive Help-Seeking.**
Participants who engaged in Learning-focused sessions (utilizing the AI
for scaffolding and conceptual clarification) demonstrated a
statistically significant positive correlation with midterm exam
performance.

**Finding 4: The Efficacy of Context-Aware Scaffolding.** The
context-aware AI significantly improved student learning performance,
representing a meaningful advantage that was conditional upon usage
patterns. Specifically, when holding the frequency of learning and task
completion sessions constant, participants in the treatment group
achieved higher exam scores than those in the control group.

5.2 Finding 1: The Essentiality of Usage Classification
-------------------------------------------------------

### 5.2.1 Discussion of Finding 1

The mutual suppression effect between Learning session count and Task
Completion count is a critical statistical finding that emerged from the
analysis of RQ1. This effect indicates that the actual, independent
relationship of each predictor was obscured when their individual
associations with the dependent variable (*E1*) were examined in
isolation. Theoretically, the two predictors share variance that is
irrelevant to the dependent variable, yet each also possesses unique
variance that is highly predictive. When both variables are included in
a multiple regression model, they statistically cancel out this shared,
irrelevant variance, allowing their true, independent contributions to
emerge.

For RQ1, the inclusion of both variables resulted in a more complete and
accurate explanatory model. The multiple regression (Model 3) explained
18.9% of the variance in E1, a substantial increase over the best
single-predictor model (Model 1), which explained only 12.7%. This
demonstrates that both session types contribute non-redundant
information. Critically, this statistical adjustment transformed the
Learning session count from a non-significant predictor (*p* = .435) to
a significant one (*p* = .013), highlighting the divergent effects of
different help-seeking strategies. This finding underscores that the
*type* of LLM engagement is a far more influential predictor of academic
performance than the simple *frequency* of use.

The interpretation of mutual suppression in this context suggests that
students who engaged in frequent task completion sessions also tended to
engage in learning sessions in ways that were initially noisy or
irrelevant to the outcome. This noise might have manifested as
individual differences in general LLM usage frequency, varying levels of
experience with prompt engineering, or differing degrees of comfort with
the technology. Only by modeling both patterns simultaneously could the
analysis isolate their independent effects on performance.

Regarding the behaviors themselves, the data reveals that Task
Completion (*ꞵ* = -0.54) had approximately 2.6 times the impact on
learning performance compared to Learning-oriented behaviors (*ꞵ* =
0.21). The negative effect of task completion was remarkably potent,
despite accounting for only 35% of all sessions in the dataset. Students
using LLMs for task completion are likely bypassing cognitive activities
crucial for knowledge and skill development. This pattern is also
evident in the RQ3 findings, where Task Completion exhibited a negative
relationship (*ꞵ* = -0.17) to computational literacy gains (C2) although
the magnitude of this impact was not as substantial as that observed for
exam performance.

Conversely, learning-oriented interactions (such as asking the LLM to
explain code or clarify computing concepts) appeared to foster a deeper
understanding that manifested as improved midterm exam scores. The fact
that the positive relationship was less profound than the negative one
may be attributed to several factors. First, the \"Learning\" label does
not account for whether a student critically evaluated the LLM\'s
response or simply read it passively. Second, dominant predictors of
academic success---such as prior knowledge, intrinsic motivation, and
study habits---were not included in the RQ1 model. The importance of
these factors was confirmed in RQ3, where baseline scores (C1) accounted
for 65.8% of the variance in post-test scores, suggesting that while AI
usage is significant, it operates within a broader ecosystem of student
ability and habit.

### 5.2.2 Contextualization of Finding 1

The findings regarding the essentiality of usage classification extend
the current literature by addressing a significant methodological gap in
Educational Technology (EdTech) and Learning Analytics research. Many
early studies on Generative AI in programming have relied on aggregate
metrics such as total prompt count [(Jošt et al., 2024b; Sheese et al.,
2024)](https://www.zotero.org/google-docs/?FXiIl7) or time on task
[(Peng et al., 2023; Vaithilingam et al.,
2022)](https://www.zotero.org/google-docs/?e2Hso4) to determine the
efficacy of these tools. However, as demonstrated by the mutual
suppression effect in this study, aggregate usage volume is a noisy and
often misleading predictor of success. By successfully classifying
interactions into adaptive and executive strategies, this research
aligns with the Self-Regulated Learning (SRL) framework, which posits
that the *intent* behind help-seeking is the primary determinant of
whether a resource supports or hinders learning [(Zimmerman,
2002)](https://www.zotero.org/google-docs/?ISXFup).

This finding corroborates and extends the work of researchers who have
cautioned against the black-box approach to AI interaction. For
instance, the negative impact of Task Completion sessions (executive
help-seeking) provides empirical weight to the concerns raised by
researchers like [Abbas et al.
(2024)](https://www.zotero.org/google-docs/?M4DOyH) and [(Pons,
(2023)](https://www.zotero.org/google-docs/?aWRdgR), who theorized that
LLMs could become cognitive crutches or reinforce task-completion
behaviors [(Becker, 2023)](https://www.zotero.org/google-docs/?mn4Aoq).

Furthermore, the consistency of these findings across both midterm
performance (E1) and computational literacy gains (C2) suggests a robust
behavioral pattern. While the impact on literacy in RQ3 (*ꞵ* = -0.17)
was less substantial than the impact on exam scores in RQ1 (*ꞵ* =
-0.54), the negative direction remained constant. This implies that
executive help-seeking doesn\'t just lower immediate performance; it may
also subtly degrade the development of foundational mental models
necessary to becoming a self-regulated learner.

The mutual suppression finding provides strong empirical support for the
central theme that the manner in which we use the LLM matters more than
the frequency of use. This study demonstrated that the overall quantity
of use lacked statistical significance regarding midterm exam scores,
which contradicts findings by [Sheese et al.,
(2024)](https://www.zotero.org/google-docs/?k2F7JI). In their study of
an introductory programming course (*N* = 52), they established a
statistically significant positive correlation between the quantity of
AI tool use and course performance (*r* = .35, p = .0147). The results
of this thesis suggest that such contradictions in the literature may
stem from methodological differences in how researchers account or fail
to account for specific answer-seeking behaviors.

Furthermore, the discovery of the mutual suppression effect
significantly extends existing research on LLM engagement by providing a
methodological framework that accounts for competing behavioral
patterns. These findings suggest that when studying complex learning
behaviors, researchers should account for all countervailing effects
within their models, rather than focusing solely on the hypothesized
effect. Scoping a study to a single task or behavior in isolation may
produce unexplainable results due to the confounding interdependence
among independent variables.

5.3 Finding 2: The Negative Impact of Executive Help-Seeking
------------------------------------------------------------

### 5.3.1 Discussion of Finding 2

Task completion session counts were a statistically significant negative
predictor of both immediate academic outcomes and the long-term
development of computational literacy. This was demonstrated by the
distinct, deleterious effects observed on midterm exam performance
(*E1*) and post-midterm computational literacy scores (*C2*).

The correlational analysis in RQ1 explored the effects of Learning and
Task Completion session counts on midterm exam scores. Task Completion
session count was a statistically significant negative predictor of exam
scores (*ꞵ* = -0.54 *p* \< .001) when modeled alongside Learning session
counts. This represents a 31% increase in the magnitude of the
coefficient compared to the single-predictor mode (*ꞵ* = -0.41, p =
.001). The observed mutual suppression effect implies that these two
usage patterns are competing strategies, and this finding aligns with
pedagogical intuition regarding help-seeking. Furthermore, the
multivariate model demonstrated a higher degree of explanatory power
(*R^2^* = .189) compared to the model containing only task completion
(*R^2^* = .127), representing a 49% increase in explained variance.

In the Analysis of Covariance (ANCOVA) model for RQ3, Task Completion
session count remained a significant negative predictor of post-test
computational literacy scores (*C2*). This relationship proved robust
(*ꞵ* = -0.17 *p* = .012), even after controlling for baseline
computational literacy (*C1*) and Learning session counts. This finding
suggests that task-oriented LLM use predicted lower final computational
literacy gains than would be expected given participants\' initial
competency levels.

When distilled into performance indicators, the data show that while
holding Learning session counts constant and accounting for baseline
computational literacy, each additional task completion session was
associated with a decrease of 0.54 units in the midterm exam score
(*E1*) and a decrease of 0.17 units in the post-test computational
literacy score (*C2*).

### 5.3.2 Contextualization of Finding 2

The negative correlation between Task Completion behaviors and academic
outcomes aligns with a growing body of literature across several
domains, specifically regarding the risks of cognitive offloading.
Researchers have noted that an overreliance on AI capabilities can lead
to a significant reduction in critical thinking, which subsequently
impairs learning performance [(Abbas et al., 2024; Pons, 2023; Rahman &
Watanobe, 2023)](https://www.zotero.org/google-docs/?JYUH2A). When
students engage in superficial interactions, such as generating direct
answers to assignments, they actively circumvent the cognitive struggle
necessary for knowledge encoding. The task-completion behaviors
identified in this study and their subsequent negative outcomes mirror
the findings of other recent studies in computing education [(Becker et
al., 2023; Margulieux et al.,
2024)](https://www.zotero.org/google-docs/?GsB0Ng).

Theoretically, the task-completion behavior observed in this study is a
digital manifestation of executive help-seeking. In this mode, the
learner's intention is to have an external agent (in this case, the LLM)
achieve a goal on their behalf rather than acquiring the skills to
complete the task independently. Within the framework of help-seeking
theory, this is considered a maladaptive characteristic with documented
negative long-term effects on learning [(Nelson-Le Gall, 1981; Newman,
1994)](https://www.zotero.org/google-docs/?glHcr2). These theoretical
predictions were empirically validated in this study's findings
regarding both the decline in midterm exam scores and the suppression of
computational literacy gains.

Furthermore, early investigations into LLMs for novice programmers often
reported inconclusive evidence regarding the benefits of these tools
[(Moradi Dakhel et al., 2023; Peng et al.,
2023)](https://www.zotero.org/google-docs/?o0CfW5). This study
encountered similar ambiguity in its initial analysis (Model 1 of RQ1),
which failed to account for the specific nature of participant
interactions. However, by isolating usage types, this research provides
empirical evidence that task-oriented LLM use is fundamentally
detrimental to learning. These seemingly contradictory findings in the
literature point back to the necessity of Finding 1: interpreting the
impact of AI on education requires a granular characterization of *how*
the tool is used, as neither usage frequency alone, nor isolation of
behavioral usage, fails to capture the full narrative of the student
experience.

5.4 Finding 3: The Positive Impact of Adaptive Help-Seeking
-----------------------------------------------------------

### 5.4.1 Discussion of Finding 3

Learning session counts were a statistically significant positive
predictor of academic learning outcomes as measured by midterm exam
scores (*E1*). However, this finding carries the same critical caveat as
the previous analysis: the mutual suppression effect mandated that to
isolate this relationship, Task Completion activity had to be controlled
within the model.

The correlational analysis in RQ1, which examined the effects of both
Learning and Task Completion session counts on midterm scores, is the
foundation for this finding. When controlling for task completion
sessions, the learning session count emerged as a statistically
significant positive predictor of exam performance (*ꞵ*= 0.21 *p* =
.013). In contrast, when the model accounted only for learning session
counts in isolation, the relationship was not significant (*ꞵ* = 0.06,
*p* = .435, *R^2\ ^*= .007). This further validates the pattern of
mutual suppression, as the positive impact of adaptive behaviors only
became statistically visible when the countervailing variance of
executive behaviors was partitioned out. Practically, this implies that
when holding Task Completion constant, a greater number of sessions
classified as Learning was associated with higher midterm scores. These
Learning session behaviors embodied such behaviors as scaffolding,
seeking code explanations, and questioning conceptual foundations.

When Findings 1, 2, and 3 are considered together, a clear divergent
strategy emerges. Learning sessions are characterized by a positive
effect on midterm performance, while Task Completion sessions contribute
to a significant negative effect. This confirms the fundamental
assumption that these represent competing strategies for achieving
academic success.

Furthermore, the fact that these variables suppress one another
indicates they share considerable variance that is irrelevant to the
dependent variable (*E1*). A potential explanation for this mutual
suppression is the presence of unmeasured shared irrelevant variance.
This may manifest as a general propensity to use AI or a digital fluency
factor; students who are more active users of the tool might naturally
accumulate higher counts in both categories regardless of their
effectiveness, creating a statistical baseline that obscures the
specific educational impact of each behavior. Only by modeling them
simultaneously can the regression filter this general usage noise to
reveal the true directional effect of each intent-based strategy.

### 5.4.2 Contextualization of Finding 3

This finding is strongly supported by research highlighting the
beneficial roles of LLM engagement for adaptive help-seeking activities,
such as active learning, seeking explanations, and requesting
clarification of complex concepts. The positive correlation observed in
Finding 3 supports the theoretical view that LLMs can function as
persistent, on-demand, subject-matter experts, acting as tutors or
coding assistants [(Cambaz & Zhang, 2024; Finnie-Ansley et al., 2022;
Prather et al., 2019)](https://www.zotero.org/google-docs/?R9pmHo). The
learning sessions in this study included behaviors such as scaffolding,
seeking code explanations, debugging aids, and questioning concepts,
which align with the characterization of LLMs as a source of expertise
that assists students in understanding and applying programming
principles [(Hassan et al., 2025; Prather, Reeves, Denny, et al.,
2024)](https://www.zotero.org/google-docs/?5bAV6Y).

From a theoretical lens, the learning sessions, which embody behaviors
such as scaffolding and inquisitive questioning, represent instrumental
help-seeking. This concept is rooted in the foundational work of
[Nelson-Le Gall (1981)](https://www.zotero.org/google-docs/?A1n4l4) and
[Newman (1994)](https://www.zotero.org/google-docs/?VHsgXy), which
distinguishes between seeking a solution (executive) and seeking the
tools to reach a solution (instrumental). In this context, the LLM
serves as an intelligent tutoring system [(Aleven et al.,
2016)](https://www.zotero.org/google-docs/?ZBocMn), utilizing adaptive
constructs similar to those found in specialized pedagogical tools like
CodeAid [(Kazemitabaar et al.,
2024)](https://www.zotero.org/google-docs/?0q2OHH).

By reinforcing the connection between instrumental help-seeking and
improved exam performance, this finding suggests that LLMs can
successfully fulfill their pedagogical promise when used as a cognitive
partner. Unlike traditional search engines or static documentation, the
conversational and context-aware nature of the LLM allows it to provide
the precise level of scaffolding required for a student to bridge their
knowledge gaps without delegating the underlying cognitive labor.

5.5. Finding 4: The Efficacy of Context-Aware Scaffolding
---------------------------------------------------------

### 5.5.1 Discussion of Finding 4

The fourth key finding of this study is that context-aware AI
significantly improved student learning performance, though this benefit
was obscured by student engagement variability. While the initial
comparison between the control and treatment groups showed no
statistically significant difference in exam scores, a suppression
analysis revealed that the context-aware treatment (T2) provided an
advantage when controlling for student usage patterns. Specifically,
when the frequency of Learning and Task Completion sessions remained
constant, participants in the treatment group achieved midterm exam
scores an average of 2.74 points higher than their peers in the control
group.

The emergence of a significant treatment effect only after controlling
for usage patterns highlights the phenomenon of statistical suppression.
However, because Learning and Task Completion session counts were
measured after treatment assignment, this finding does not represent a
direct causal link. In other words, providing students with the
treatment does not cause higher grades; rather, higher grades are a
conditional estimate of the tool's efficacy when usage is factored out.

The suppression analysis (RQ2 Model 4) successfully partitioned out this
behavioral variance, revealing the treatment as a conditional effect.
This implies that the context-aware feature functioned as a performance
multiplier intrinsic to the tool's quality rather than a mechanism that
altered student behavior. Mediation analyses confirmed that the
treatment did not cause students to engage in more Learning sessions or
fewer Task Completion sessions. Instead, the benefit was qualitative:
For any given level of engagement, the context-aware LLM provided
superior support compared to the standard model.

These results indicate that the treatment effectively raised the
baseline of the educational interaction. By automatically injecting
assignment instructions into the LLM's context, the treatment group did
not require students to prompt the AI expertly with background
information. Consequently, a student in the treatment group asking a
vague question likely received a relevant, scaffolded response based on
the assignment data, whereas a student in the control group asking the
same question likely received a generic or less helpful response. The
statistical significance of the treatment (*p* = .023) in the final
model confirms that technology design matters, but its impact is
conditional upon and often masked by the student\'s intent.

### 5.5.2 Contextualization of Finding 4

Finding 4 addresses a significant barrier identified in the literature:
Novice programmers often struggle to formulate effective prompts [(Hsu,
2025; Wang et al., 2024)](https://www.zotero.org/google-docs/?EEwupU).
Recent research has highlighted that without precise prompting, students
risk receiving unhelpful generations or misinterpretations of their
intent, requiring students to learn prompt engineering alongside coding
[(Denny, Leinonen, et al.,
2024)](https://www.zotero.org/google-docs/?1MstNe). The results of this
study suggest that in-context learning (ICL) can serve as an automated
technological solution to this deficit.

By shifting the burden of context provision from the student to the
system, the treatment effectively democratized the utility of the large
language model (LLM). This aligns with the foundational work on ICL by
[Brown et al.
(2020[)]{.underline}](https://www.zotero.org/google-docs/?qd2uyN), which
demonstrated that providing examples and context improves model
reasoning. In this educational setting, context injection ensured that
the AI acted as a more informed tutor, capable of providing scaffolding
without requiring the student to first provide the necessary background
information.

Furthermore, this finding refines the narrative regarding AI in
education. Findings 2 and 3 emphasized that student intent (adaptive
versus maladaptive) is the primary driver of success, while Finding 1
provided evidence that both intentions must be considered concurrently.
Finding 4 demonstrates that system design plays a crucial, complementary
role. The context-aware intervention did not prevent students from
engaging in harmful Task Completion behaviors, nor did it force them
into beneficial Learning behaviors. However, it ensured that when
interactions occurred, they were more pedagogically effective. This
supports the argument for institutional adoption of tailored,
context-aware AI tutors over generic, commercial models, as the former
can be engineered to compensate for novice limitations and maximize the
value of student-AI interactions.

5.5 Implications and Recommendations 
------------------------------------

The findings offer crucial insights for instructors, course designers
and students as to how LLMs should be used to foster positive learning
outcomes and mitigate negative ones for novice programmers.

### 5.5.1 Theoretical Implications

The results of this study contribute to the theoretical understanding of
help-seeking behavior, computational literacy development, and
methodological approaches in the context of generative AI. The
categorical content analysis used to classify usage patterns provided
empirical evidence supporting the distinction between beneficial and
detrimental forms of help solicitation within LLM interactions.
Participant LLM usage patterns demonstrating task completion sessions,
where students asked the AI to complete assignments or generate answers,
align with executive or maladaptive help-seeking. As predicted by
foundational help-seeking literature, this undesirable behavior
demonstrated a robust negative correlation with academic performance
(*E1*) and computational literacy skill development (*C2*).

Conversely, learning sessions, which encompass questioning and
scaffolding behaviors, align with adaptive help-seeking. Adaptive
help-seeking behaviors assist learners in becoming more self-sufficient
and lead to a greater understanding of the material. The resulting
significant positive correlation with *E1* scores confirms that when
LLMs serve as a form of intelligent tutoring system, they facilitate
adaptive learning strategies. This research extends the applicability of
the help-seeking framework (Nelson-Le Gall, 1981; Newman, 1994) to the
domain of human-AI interaction in programming education.

The strong negative correlation found between task completion sessions
and posttest computational literacy scores (*C2*) (*ꞵ*= -0.17, *p* =
.012), when controlling for baseline *C1*, highlights a crucial
theoretical risk of LLM use on long-term skill acquisition. Task
completion constitutes a form of cognitive offloading. This study
suggests that regularly outsourcing problem-solving via task completion
denies learners the mental effort required to build the abstract
problem-solving abilities essential to computational literacy. Since
computational literacy is defined as the ability to formulate and solve
problems systematically and independently from a specific programming
language, this finding reinforces the concern that instrumental LLM use
may constrain the development of core skills in computing education.

The analysis of RQ1 yielded a critical methodological finding: a mutual
suppression effect among participants engaged in Learning sessions
versus Task Completion sessions. This effect obscured the true
relationship until both types of sessions were accounted for in the
statistical model. This finding provides a necessary methodological
caution, suggesting that research designs focusing solely on one facet
of LLM use, such as perceived benefits or risks, may yield inconclusive
or misleading results due to the confounding interdependence among usage
types. Researchers should account for all potentially competing
behaviors within their models to achieve statistical clarity in complex
LLM behavioral analysis.

Finally, Finding 4 provides empirical validation for the application of
In-Context Learning (ICL) within educational settings. Theoretically,
this challenges the assumption that students must master prompt
engineering to benefit from AI tools. By separating the domain skills of
the subject from the interaction skills necessary to use AI efficiently,
ICL allows learners to focus on core concepts rather than the nuances of
prompt construction. Additionally, the conditional nature of Finding 4
implies that the theoretical value of ICL lies in the quality of the
response rather than its capacity to modify help-seeking habits. In
summary, these findings illustrate that LLMs are not passive tools whose
impact is determined solely by frequency; rather, the intent behind
their use plays the primary role in learning outcomes.

### 5.5.2 Practical Implications for Instructors

This study empirically demonstrated the negative repercussions of
task-completion behaviors and the benefits of learning behaviors when
utilizing Large Language Models (LLMs) in an introductory programming
course. Because it is no longer practical to prohibit the use of AI in
the classroom, educators must adapt to this evolving landscape. The
following three practical implications are proposed for instructors.

First, course instructors should actively identify and discourage
task-completion behaviors among their students. These behaviors
undermine the cognitive effort essential for knowledge and skill
development. Because LLMs are sufficiently advanced to complete
introductory programming assignments, superficial learning often
manifests as high-quality assignment submissions contrasted with poor
summative exam performance. Instructors who permit AI use should employ
frequent knowledge checks, such as diagnostic quizzes or short formative
assessments, to allow students to self-identify when they are delegating
cognitive labor to the AI.

Second, to encourage learning-oriented AI engagement---which
demonstrated a positive correlation with exam scores---instructors
should dedicate instructional time to teaching effective AI usage. This
training should include demonstrations or lab activities that model how
to scaffold learning with AI, such as requesting concept explanations,
seeking illustrative examples, and confirming the student\'s own
understanding of a topic. For example, during a debugging lab, the LLM
could be utilized as a guide to help students not only to diagnose a
syntax error but also to understand its underlying cause. Using the LLM
in this capacity builds constructive habits, positioning the tool as a
persistent, 24/7 tutor that supports and justifies the student\'s
reasoning.

Finally, instructors should teach students the importance of framing
inquiries within a specific context. LLMs are trained on vast, general
datasets, and the prompts provided by users require framing to scope the
generative output effectively. For instance, the prompt, \"Help me write
a factorial function in Python,\" typically generates a direct solution.
Conversely, the prompt, \"Help me write a factorial function in Python:
Do not write the code for me; instead, explain the steps I should take
and why,\" provides instructions for the student to follow as they write
the code independently. This approach encourages conceptual scaffolding
and assists the learner in forming deeper connections with foundational
programming principles.

### 5.5.3 Practical Implications for Institutions

There are two key implications for educational institutions. First,
context-aware large language models (LLMs) that are knowledgeable of the
specific subject matter being taught should be deployed. Finding 4
revealed that, for any given level of student engagement, a
context-aware tool provided superior support regardless of whether the
student employed adaptive or executive help-seeking behaviors.
Institutional deployment of an LLM democratizes access to high-quality
assistance, facilitates the generation of more pedagogically sound
content, and ensures that AI interactions are more effective for the
learner.

Second, institutionally deployed LLMs should be configured to support
adaptive help-seeking behavior while discouraging executive
help-seeking. For example, recent developments in AI research have
prioritized the creation of Socratic models, such as Google's
LearnLM[^29]. This type of AI is designed to utilize the Socratic method
and does not support direct answer-seeking behaviors. At the time of
this research, these capabilities were becoming integrated into
commercial models, making it possible for institutions to develop custom
chatbot interfaces utilizing these frameworks.

To discourage students from migrating to non-specialized, off-the-shelf
AI, it is recommended that institutions avoid banning executive
help-seeking or disabling the feature within the LLM. Instead,
institutions should focus on pedagogical strategies that encourage
students to make the correct choice for self-directed learning. By
providing a superior, specialized tool that balances support with
cognitive challenge, institutions can better guide students toward
productive academic habits.

### 5.5.4 Practical Implications for Students

Several implications established for instructors are equally applicable
to students. Students must remain cognizant of the risks associated with
cognitive offloading and the practice of delegating learning tasks to
large language models (LLMs). Learners must develop the metacognitive
awareness necessary to identify when they are engaging in
task-completion behaviors and proactively self-correct. Frequent
self-assessment is an effective strategy to maintain this awareness;
LLMs are particularly useful in this regard when utilized to formulate
conceptual questions for self-testing.

A primary theme across the findings of this study is that the mode of
engagement is a more significant predictor of academic success than the
aggregate frequency of LLM use. Students should recognize that while
LLMs offer immediate convenience, superficial use for task completion
undermines long-term learning. Context remains a critical factor in this
interaction. For example, requesting \"example midterm questions\" from
an LLM often fails to be helpful because the request lacks the specific
course context necessary to generate relevant results.

This highlights the necessity of comprehensive AI education.
Understanding the underlying mechanisms of generative AI unravels the
mystery of the technology, assisting students in avoiding the
anthropomorphization of the tool. By viewing the LLM as a statistical
engine rather than a sentient source of truth, students can better
position themselves as self-regulated learners who use AI as a scaffold
for their own cognitive development rather than a replacement for it.

5.6 Limitations
---------------

This study presents several limitations that future research should
address. Although the findings appear impactful and applicable to the
broader educational landscape concerning the impacts of LLM use on
learning, I caution against broad generalization to other academic
disciplines or student populations. This study was conducted over a
six-week period with a population of non-computer science majors
enrolled in an introductory Python course for information professionals.
The study was limited to six weeks because only the first half of the
curriculum covers the foundational computational literacy constructs
common to most introductory programming courses; the remainder of the
course focused on data analytics.

Furthermore, the CT-Test utilized in RQ3 only evaluates computational
concepts, such as program flow and data structures. It is not an
appropriate instrument for measuring broader computational literacy
constructs, such as problem framing or task decomposition. The current
scarcity of validated instruments in this domain presents a distinct
opportunity for future inquiry.

Unlike RQ3, the analysis for RQ1, which examined the relationship
between LLM usage and midterm exam scores (*E1*), omitted a
pre-intervention assessment of baseline ability. Consequently, the study
design could not control for prior knowledge or other initial
differences in student understanding of the material. This omission
makes it difficult to isolate true learning gains from preexisting
competency. Additionally, RQ1 did not account for other recognized
predictors of academic success, such as student motivation or
established study habits.

The categorical content analysis of the initial coding sample was
performed by a single human rater. Although the subsequent LLM
classification achieved high inter-coder reliability (Krippendorff's *⍺*
= .873), utilizing multiple independent human raters would have
strengthened the validation of the human baseline and further reduced
the risk of potential rater bias. Regarding RQ3, the marginal
statistical significance found for *Learning* session counts (*p* =
.078) indicates the possibility of a Type II error, or a false negative.
This suggests that with a larger sample size, the model might reach
statistical significance, and the potential benefits of this finding
warrant further investigation.

Finally, the significant treatment effect in RQ2 was only revealed after
controlling for AI usage patterns. These usage variables were measured
post-randomization but prior to the outcome measurement. Conditioning on
post-treatment variables introduces uncertainty and potential bias in
causal interpretation. As a result, the findings from RQ2 must be
interpreted as conditional rather than strictly causal.

5.7 Future Research
-------------------

Based on the implications and limitations outlined in the previous
sections, these suggestions for future research are organized into three
primary domains. The first involves exploring how LLM designs might
promote adaptive help-seeking behavior to improve learning outcomes. The
second seeks to deepen the current understanding of student usage
patterns. The final domain considers refinements to strengthen
methodological rigor in AI-education research.

This thesis established that the type of engagement is a critical factor
in learning performance. This highlights an immediate area for future
research: the design of interventions to study how specific LLM
configurations impact learning. Similar to the methodology of RQ2,
controlled experiments could be conducted where the experimental
treatment involves LLMs designed to mitigate or discourage
task-completion behaviors. This could be achieved through the use of
Socratic models, such as LearnLM, or through the implementation of
extensive pedagogical guardrails within system prompts. Such research
could identify whether specific LLM designs foster adaptive help-seeking
behaviors that, in turn, facilitate deeper learning. Furthermore, these
investigations should be extended to academic disciplines beyond
computer programming.

A second area of future research focuses on the findings regarding the
mutual suppression effect (RQ1) and the marginal significance of
computational literacy gains (RQ3). These results point toward necessary
methodological extensions. First, incorporating a pre-test for E1 to
control for initial differences in baseline understanding and prior
knowledge would allow researchers to better isolate learning gains and
account for the significant influence of initial ability.

To further understand the implications of task-completion and learning
sessions on exam performance, future research designs should account for
other known predictors of academic success, such as motivation and
self-efficacy. Motivation remains a critical factor in self-regulated
learning [(Pintrich, 2003)](https://www.zotero.org/google-docs/?9XmRoS).
To measure participant motivation, standardized instruments such as the
Intrinsic Motivation Inventory may be utilized [(Ryan,
1982)](https://www.zotero.org/google-docs/?MwDVFj). Additionally, a
recognized gap in the literature is the relationship between
overconfidence and self-efficacy as it relates to AI usage. The General
Self-Efficacy Scale could be established as a baseline measure of
participant self-efficacy prior to intervention [(Schwarzer & Jerusalem,
1995)](https://www.zotero.org/google-docs/?RSRsLy). This would allow
future researchers to observe the impacts of usage patterns on learning
while controlling for these influential psychological characteristics.

Finally, future research should focus on strengthening methodological
rigor and expanding the scope of the current study. The categorical
content analysis in this study relied on a single human rater. Future
studies should aim for higher internal validation by utilizing multiple
independent human raters to strengthen the human baseline and reduce the
risk of individual rater bias during the chat-log coding process.

The *CT-Test* utilized in RQ3 measured only algorithmic thinking, such
as program flow and data structures. Future research should seek to use
or develop validated instruments that measure broader computational
literacy constructs, such as problem framing and task decomposition.
While validated surveys exist for computational thinking, such as the
Computational Thinking Scale [(Tsai et al.,
2021)](https://www.zotero.org/google-docs/?qyMsei), these are not
performance assessments. Researchers might also consider non-validated
assessments, such as the Bebras challenges, which have been used
effectively in the literature [(Araujo et al., 2019; Dagienė & Sentance,
2016; Zapata-Cáceres et al.,
2024)](https://www.zotero.org/google-docs/?qV2IN8).

Because LLM usage in education is not isolated to computer programming,
future studies should investigate these phenomena in other academic
disciplines and among different student populations. Replicating the
methodology of RQ1 in diverse fields would help identify if these
findings regarding adaptive versus maladaptive help-seeking are
transferable to different academic contexts.

5.8 Conclusion
--------------

This thesis investigated the impact of large language model (LLM) use on
student learning performance and computational literacy within an
introductory Python programming course. The LLM represents a disruptive
innovation in education, capable of serving as both a legitimate
learning aid and a means to circumvent the learning process entirely.
The core objective of this research was to move beyond the binary debate
of prohibition versus acceptance and instead identify which specific LLM
usage patterns are beneficial to learning and which are detrimental.

To address these questions, the study employed a multi-method approach,
utilizing quantitative correlational and experimental designs based on
systematically categorized student interaction data. Student
interactions with a course-provided LLM (GPT-4o-mini) were captured and
classified via categorical content analysis into two primary, competing
strategies: Learning sessions, which incorporated adaptive help-seeking
behavior, and Task Completion sessions, characterized by executive help-
seeking behaviors. These usage patterns were quantified and analyzed for
their correlation with academic outcomes, specifically midterm exam
scores (*E1*) and computational literacy scores (*C2*).

The findings revealed a complex relationship between LLM engagement and
academic success, demonstrating that the type of engagement is a far
more significant predictor than the aggregate frequency of use.
Task-completion activities revealed a robust negative correlation with
both midterm exam and computational literacy scores, whereas
learning-oriented sessions demonstrated a positive correlation with
midterm exam performance. Statistical analysis identified a powerful
mutual suppression effect between these two usage patterns, confirming
the necessity of modeling both interaction types simultaneously to
isolate their true, independent effects.

The influence of these usage patterns was so pronounced that they
functioned as suppressors in the controlled experiment measuring the
impacts of in-context learning (ICL) on student performance. The results
were conditional, demonstrating that the treatment was effective only
when controlling for the two distinct usage patterns. This suggests that
the intervention does not act as a universal solution that improves
performance regardless of behavior; rather, it enhances the quality of
engagement only when accounting for similar student usage patterns
within the system.

This research validates help-seeking theory within the domain of
human-AI interaction. Task-completion behaviors align with executive
help-seeking, representing the undesirable intent to have the LLM
achieve a goal on the learner\'s behalf. Conversely, learning sessions
represent adaptive help-seeking, positioning the LLM as an effective
intelligent tutoring system that supports academic success.

Given the demonstrated negative repercussions of task-completion, the
primary takeaway of this study is the urgent need for pedagogical
adaptation. Because AI integration is an enduring reality, educators
must shift their focus from policing the technology to teaching students
how to use AI effectively and constructively. While creating custom LLMs
to mitigate maladaptive help-seeking offers some benefits, it is not
practical to control all off-the-shelf AI tools. Therefore, the
essential next step in computing education must involve empowering
students to become sophisticated, adaptive users of this technology,
ensuring that AI serves as a scaffold for cognitive development rather
than a replacement for it.

**References**
==============

> [Abbas, M., Jam, F. A., & Khan, T. I. (2024). Is it harmful or
> helpful? Examining the causes and consequences of generative AI usage
> among university students. *International Journal of Educational
> Technology in Higher Education*, *21*(1), 10.
> https://doi.org/10.1186/s41239-024-00444-7](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Akyürek, E., Schuurmans, D., Andreas, J., Ma, T., & Zhou, D. (2022).
> What learning algorithm is in-context learning? Investigations with
> linear models. *arXiv Preprint
> arXiv:2211.15661*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Aleven, V., McLaren, B., Roll, I., & Koedinger, K. (2006). Toward
> Meta-cognitive Tutoring: A Model of Help Seeking with a Cognitive
> Tutor. *International Journal of Artificial Intelligence in
> Education*, *16*,
> 101--128.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Aleven, V., Roll, I., McLaren, B. M., & Koedinger, K. R. (2016). Help
> Helps, But Only So Much: Research on Help Seeking with Intelligent
> Tutoring Systems. *International Journal of Artificial Intelligence in
> Education*, *26*(1), 205--223.
> https://doi.org/10.1007/s40593-015-0089-1](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Aleven, V., Stahl, E., Schworm, S., Fischer, F., & Wallace, R.
> (2003). Help Seeking and Help Design in Interactive Learning
> Environments. *Review of Educational Research*, *73*(3), 277--320.
> https://doi.org/10.3102/00346543073003277](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Allam, H., Dempere, J., Akre, V., Parakash, D., Mazher, N., & Ahamed,
> J. (2023). Artificial Intelligence in Education: An Argument of
> Chat-GPT Use in Education. *2023 9th International Conference on
> Information Technology Trends (ITT)*,
> 151--156.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Andrej Karpathy \[\@karpathy\]. (2025, February 2). *There's a new
> kind of coding I call "vibe coding", where you fully give in to the
> vibes, embrace exponentials, and forget that the code even exists.
> It's possible because the LLMs (e.g. Cursor Composer w Sonnet) are
> getting too good. Also I just talk to Composer with SuperWhisper*
> \[Tweet\]. Twitter.
> https://x.com/karpathy/status/1886192184808149383](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Araujo, A. L. S. O., Andrade, W. L., Guerrero, D. D. S., & Melo, M.
> R. A. (2019). How Many Abilities Can We Measure in Computational
> Thinking?: A Study on Bebras Challenge. *Proceedings of the 50th ACM
> Technical Symposium on Computer Science Education*, 545--551.
> https://doi.org/10.1145/3287324.3287405](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Baidoo-Anu, D., & Owusu Ansah, L. (2023). Education in the era of
> generative artificial intelligence (AI): Understanding the potential
> benefits of ChatGPT in promoting teaching and learning. *Available at
> SSRN 4337484*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Bandura, A. (1977). *Self-efficacy: Toward a Unifying Theory of
> Behavioral Change*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Bang, K., & Dang, M. (2024). *Impact of Generative AI on Learning
> Programming* \[Master's Thesis\]. Chalmers University of Technology,
> University of Gothenburg.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Becker, B. A. (2023). *Generative AI in Introductory
> Programming*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Becker, B. A., Denny, P., Finnie-Ansley, J., Luxton-Reilly, A.,
> Prather, J., & Santos, E. A. (2023). Programming is hard-or at least
> it used to be: Educational opportunities and challenges of ai code
> generation. *Proceedings of the 54th ACM Technical Symposium on
> Computer Science Education V. 1*,
> 500--506.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Brennan, K., & Resnick, M. (2012). *New frameworks for studying and
> assessing the development of computational
> thinking*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Breusch, T. S., & Pagan, A. R. (1979). A simple test for
> heteroscedasticity and random coefficient variation. *Econometrica:
> Journal of the Econometric Society*,
> 1287--1294.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Brown, T. B., Mann, B., Ryder, N., Subbiah, M., Kaplan, J., Dhariwal,
> P., Neelakantan, A., Shyam, P., Sastry, G., Askell, A., Agarwal, S.,
> Herbert-Voss, A., Krueger, G., & Henighan, T. (2020). *Language Models
> are Few-Shot Learners*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Cambaz, D., & Zhang, X. (2024). Use of AI-driven Code Generation
> Models in Teaching and Learning Programming: A Systematic Literature
> Review. *Proceedings of the 55th ACM Technical Symposium on Computer
> Science Education V. 1*, 172--178.
> https://doi.org/10.1145/3626252.3630958](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Chen, M., Tworek, J., Jun, H., Yuan, Q., Pinto, H. P. de O., Kaplan,
> J., Edwards, H., Burda, Y., Joseph, N., & Brockman, G. (2021).
> Evaluating large language models trained on code. *arXiv Preprint
> arXiv:2107.03374*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Chinthapatla, S. (2024). Unleashing the Future: A Deep Dive into
> AI-Enhanced Productivity for Developers. *Int. J. Sci. Technol. Eng.
> Math*, *13*(03).](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Christensen, C. M. (1997). *The innovator's dilemma: When new
> technologies cause great firms to fail*. Harvard Business School
> Press.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Christensen, C. M., McDonald, R., Altman, E. J., & Palmer, J. E.
> (2018). Disruptive Innovation: An Intellectual History and Directions
> for Future Research. *Journal of Management Studies*, *55*(7),
> 1043--1078.
> https://doi.org/10.1111/joms.12349](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Cohen, J., Cohen, P., West, S. G., & Aiken, L. S. (2013). *Applied
> multiple regression/correlation analysis for the behavioral sciences*.
> Routledge.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Collins. (2025). *Collins---The Collins Word of the Year 2025 is\...*
> https://www.collinsdictionary.com/woty](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Compeau, D. R., & Higgins, C. A. (1995). Computer Self-Efficacy:
> Development of a Measure and Initial Test. *MIS Quarterly*, *19*(2),
> 189.
> https://doi.org/10.2307/249688](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Creswell, J. W., & Creswell, J. D. (2017). *Research design:
> Qualitative, quantitative, and mixed methods approaches*. Sage
> publications.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Cronbach, L. J. (1951). Coefficient alpha and the internal structure
> of tests. *Psychometrika*, *16*(3),
> 297--334.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Cronbach, L. J., & Furby, L. (1970). How we should measure\"
> change\": Or should we? *Psychological Bulletin*, *74*(1),
> 68.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Dagienė, V., & Sentance, S. (2016). It's Computational Thinking!
> Bebras Tasks in the Curriculum. In A. Brodnik & F. Tort (Eds.),
> *Informatics in Schools: Improvement of Informatics Knowledge and
> Perception* (Vol. 9973, pp. 28--39). Springer International
> Publishing.
> https://doi.org/10.1007/978-3-319-46747-4\_3](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Denny, P., Kumar, V., & Giacaman, N. (2023). Conversing with Copilot:
> Exploring Prompt Engineering for Solving CS1 Problems Using Natural
> Language. *Proceedings of the 54th ACM Technical Symposium on Computer
> Science Education V. 1*, 1136--1142.
> https://doi.org/10.1145/3545945.3569823](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Denny, P., Leinonen, J., Prather, J., Luxton-Reilly, A., Amarouche,
> T., Becker, B. A., & Reeves, B. N. (2024). Prompt Problems: A New
> Programming Exercise for the Generative AI Era. *Proceedings of the
> 55th ACM Technical Symposium on Computer Science Education V. 1*,
> 296--302.
> https://doi.org/10.1145/3626252.3630909](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Denny, P., Prather, J., Becker, B. A., Finnie-Ansley, J., Hellas, A.,
> Leinonen, J., Luxton-Reilly, A., Reeves, B. N., Santos, E. A., &
> Sarsa, S. (2023). Computing Education in the Era of Generative AI.
> *arXiv Preprint
> arXiv:2306.02608*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Denny, P., Prather, J., Becker, B. A., Finnie-Ansley, J., Hellas, A.,
> Leinonen, J., Luxton-Reilly, A., Reeves, B. N., Santos, E. A., &
> Sarsa, S. (2024a). Computing Education in the Era of Generative AI.
> *Communications of the ACM*, *67*(2), 56--67.
> https://doi.org/10.1145/3624720](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Denny, P., Prather, J., Becker, B. A., Finnie-Ansley, J., Hellas, A.,
> Leinonen, J., Luxton-Reilly, A., Reeves, B. N., Santos, E. A., &
> Sarsa, S. (2024b). Computing Education in the Era of Generative AI.
> *Communications of the ACM*, *67*(2), 56--67.
> https://doi.org/10.1145/3624720](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Dinan, Stephen. (2023, May 29). *Confidently incorrect: For ChatGPT,
> the truth isn't always out there---Washington Times*.
> https://www.washingtontimes.com/news/2023/may/29/confidently-incorrect-chatgpt-truth-isnt-always-ou/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [DuBoulay, Benedict. (1989). Some Difficulties of Learning to Program.
> In E. Soloway & J. C. Spohrer (Eds.), *Studying the novice programmer*
> (pp. 283--299). L. Erlbaum
> Associates.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Durbin, J., & Watson, G. (1971). Testing for serial correlation in
> least squares regression. III. *Biometrika*, *58*(1),
> 1--19.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Edwards, J. R., & Lambert, L. S. (2007). Methods for integrating
> moderation and mediation: A general analytical framework using
> moderated path analysis. *Psychological Methods*, *12*(1),
> 1.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Farrar, D. E., & Glauber, R. R. (1967). Multicollinearity in
> regression analysis: The problem revisited. *The Review of Economic
> and Statistics*, 92--107.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Finnie-Ansley, J., Denny, P., Becker, B. A., Luxton-Reilly, A., &
> Prather, J. (2022). The robots are coming: Exploring the implications
> of openai codex on introductory programming. *Proceedings of the 24th
> Australasian Computing Education Conference*,
> 10--19.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Ghimire, A., & Edwards, J. (2024). Coding with AI: How Are Tools Like
> ChatGPT Being Used by Students in Foundational Programming Courses. In
> A. M. Olney, I.-A. Chounta, Z. Liu, O. C. Santos, & I. I. Bittencourt
> (Eds.), *Artificial Intelligence in Education* (Vol. 14830, pp.
> 259--267). Springer Nature Switzerland.
> https://doi.org/10.1007/978-3-031-64299-9\_20](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Gillioz, A., Casas, J., Mugellini, E., & Khaled, O. A. (2020).
> *Overview of the Transformer-based Models for NLP Tasks*. 179--183.
> https://doi.org/10.15439/2020F20](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Github, I. G. (2023, June 13). Survey reveals AI's impact on the
> developer experience. *The GitHub Blog*.
> https://github.blog/news-insights/research/survey-reveals-ais-impact-on-the-developer-experience/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Gorson, J., & O'Rourke, E. (2020). Why do CS1 Students Think They're
> Bad at Programming?: Investigating Self-efficacy and Self-assessments
> at Three Universities. *Proceedings of the 2020 ACM Conference on
> International Computing Education Research*, 170--181.
> https://doi.org/10.1145/3372782.3406273](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hackl, V., Müller, A. E., Granitzer, M., & Sailer, M. (2023). Is
> GPT-4 a reliable rater? Evaluating consistency in GPT-4's text
> ratings. *Frontiers in Education*, *8*,
> 1272229.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Halevy, A., Norvig, P., & Pereira, F. (2009). The Unreasonable
> Effectiveness of Data. *IEEE Intelligent Systems*, *24*(2), 8--12.
> https://doi.org/10.1109/MIS.2009.36](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hassan, M., Chen, Y., Denny, P., & Zilles, C. (2025). On Teaching
> Novices Computational Thinking by Utilizing Large Language Models
> Within Assessments. *Proceedings of the 56th ACM Technical Symposium
> on Computer Science Education V. 1*, 471--477.
> https://doi.org/10.1145/3641554.3701906](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hayes, A. F. (2009). Beyond Baron and Kenny: Statistical mediation
> analysis in the new millennium. *Communication Monographs*, *76*(4),
> 408--420.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hertz, M. (2010). What do "CS1" and "CS2" mean?: Investigating
> differences in the early courses. *Proceedings of the 41st ACM
> Technical Symposium on Computer Science Education*, 199--203.
> https://doi.org/10.1145/1734263.1734335](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Holmes, W., & Tuomi, I. (2022). State of the art and practice in AI
> in education. *European Journal of Education*, *57*(4),
> 542--570.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Holzäpfel, M. (2020). *Simpledorff* (Version 0.0.3) \[Computer
> software\].
> https://pypi.org/project/simpledorff/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Horn, M. B. (2024, June 3). *What does Disruptive Innovation Theory
> have to say about AI? - Christensen Institute*.
> https://www.christenseninstitute.org/blog/what-does-disruptive-innovation-say-about-ai/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hou, W., & Ji, Z. (2025). Comparing Large Language Models and Human
> Programmers for Generating Programming Code. *Advanced Science*,
> *12*(8), 2412279.
> https://doi.org/10.1002/advs.202412279](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hsu, H.-P. (2025). From Programming to Prompting: Developing
> Computational Thinking through Large Language Model-Based Generative
> Artificial Intelligence. *TechTrends*.
> https://doi.org/10.1007/s11528-025-01052-6](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Huitema, B. (2011). *The analysis of covariance and alternatives:
> Statistical methods for experiments, quasi-experiments, and
> single-case studies*. John Wiley &
> Sons.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Hunter, J. D. (2007). Matplotlib: A 2D graphics environment.
> *Computing in Science & Engineering*, *9*(3), 90--95.
> https://doi.org/10.1109/MCSE.2007.55](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Jacob, S. R., Warschauer, M., University of California, Irvine, &
> University of California, Irvine. (2018). Computational Thinking and
> Literacy. *Journal of Computer Science Integration*, *1*(1).
> https://doi.org/10.26716/jcsi.2018.01.1.1](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Jošt, G., Taneski, V., & Karakatič, S. (2024a). The Impact of Large
> Language Models on Programming Education and Student Learning
> Outcomes. *Applied Sciences*, *14*(10), 4115.
> https://doi.org/10.3390/app14104115](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Jošt, G., Taneski, V., & Karakatič, S. (2024b). The Impact of Large
> Language Models on Programming Education and Student Learning
> Outcomes. *Applied Sciences*, *14*(10), 4115.
> https://doi.org/10.3390/app14104115](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Kasneci, E., Sessler, K., Küchemann, S., Bannert, M., Dementieva, D.,
> Fischer, F., Gasser, U., Groh, G., Günnemann, S., Hüllermeier, E.,
> Krusche, S., Kutyniok, G., Michaeli, T., Nerdel, C., Pfeffer, J.,
> Poquet, O., Sailer, M., Schmidt, A., Seidel, T., ... Kasneci, G.
> (2023). ChatGPT for good? On opportunities and challenges of large
> language models for education. *Learning and Individual Differences*,
> *103*, 102274.
> https://doi.org/10.1016/j.lindif.2023.102274](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Kazemitabaar, M., Chow, J., Ma, C. K. T., Ericson, B. J., Weintrop,
> D., & Grossman, T. (2023). Studying the effect of AI Code Generators
> on Supporting Novice Learners in Introductory Programming.
> *Proceedings of the 2023 CHI Conference on Human Factors in Computing
> Systems*, 1--23.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Kazemitabaar, M., Ye, R., Wang, X., Henley, A. Z., Denny, P., Craig,
> M., & Grossman, T. (2024). CodeAid: Evaluating a Classroom Deployment
> of an LLM-based Programming Assistant that Balances Student and
> Educator Needs. *Proceedings of the CHI Conference on Human Factors in
> Computing Systems*, 1--20.
> https://doi.org/10.1145/3613904.3642773](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Kinnunen, P., & Simon, B. (2012). My program is ok -- am I? Computing
> freshmen's experiences of doing programming assignments. *Computer
> Science Education*, *22*(1), 1--28.
> https://doi.org/10.1080/08993408.2012.655091](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Kluyver, T., Ragan-Kelley, B., Pérez, F., Granger, B., Bussonnier,
> M., Frederic, J., Kelley, K., Hamrick, J., Grout, J., Corlay, S.,
> Ivanov, P., Avila, D., Abdalla, S., & Willing, C. (2016). Jupyter
> Notebooks -- a publishing format for reproducible computational
> workflows. *Positioning and Power in Academic Publishing: Players,
> Agents and Agendas*, 87--90.
> https://doi.org/10.3233/978-1-61499-649-1-87](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Korkmaz, Ö., Çakir, R., & Özden, M. Y. (2017). A validity and
> reliability study of the computational thinking scales (CTS).
> *Computers in Human Behavior*, *72*, 558--569.
> https://doi.org/10.1016/j.chb.2017.01.005](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Krippendorff, K. (2011). *Computing Krippendorff's
> alpha-reliability*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Krippendorff, K. (2018). *Content analysis: An introduction to its
> methodology*. Sage
> publications.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Lau, S., & Guo, P. (2023). From\" Ban It Till We Understand It\" to\"
> Resistance is Futile\": How University Programming Instructors Plan to
> Adapt as More Students Use AI Code Generation and Explanation Tools
> such as ChatGPT and GitHub Copilot. *Proceedings of the 2023 ACM
> Conference on International Computing Education Research-Volume 1*,
> 106--121.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Leinonen, J., Denny, P., MacNeil, S., Sarsa, S., Bernstein, S., Kim,
> J., Tran, A., & Hellas, A. (2023). Comparing code explanations created
> by students and large language models. *arXiv Preprint
> arXiv:2304.03938*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Lishinski, A., & Rosenberg, J. (2021). All the Pieces Matter: The
> Relationship of Momentary Self-efficacy and Affective Experiences with
> CS1 Achievement and Interest in Computing. *Proceedings of the 17th
> ACM Conference on International Computing Education Research*,
> 252--265.
> https://doi.org/10.1145/3446871.3469740](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Lohr, S. (2025, June 30). How Do You Teach Computer Science in the
> A.I. Era? *The New York Times*.
> https://www.nytimes.com/2025/06/30/technology/computer-science-education-ai.html](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Lu, J. J., & Fletcher, G. H. L. (2009). Thinking About Computational
> Thinking. *Association for Computing
> Machinery*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Maes, S. (2025). *The  Gotchas of AI Coding and Vibe Coding. It's All
> About Support And Maintenance*.
> https://doi.org/10.5281/ZENODO.15343349](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Manna, Z., & Waldinger, R. J. (1971). Toward automatic program
> synthesis. *Communications of the ACM*, *14*(3), 151--165.
> https://doi.org/10.1145/362566.362568](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Margulieux, L. E., Prather, J., Reeves, B. N., Becker, B. A., Cetin
> Uzun, G., Loksa, D., Leinonen, J., & Denny, P. (2024).
> Self-Regulation, Self-Efficacy, and Fear of Failure Interactions with
> How Novices Use LLMs to Solve Programming Problems. *Proceedings of
> the 2024 on Innovation and Technology in Computer Science Education V.
> 1*, 276--282.
> https://doi.org/10.1145/3649217.3653621](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Maxwell, S. E., Delaney, H. D., & Kelley, K. (2017). *Designing
> experiments and analyzing data: A model comparison perspective*.
> Routledge.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [McGill, T. J., & Volet, S. E. (1997). A Conceptual Framework for
> Analyzing Students' Knowledge of Programming. *Journal of Research on
> Computing in Education*, *29*(3), 276--297.
> https://doi.org/10.1080/08886504.1997.10782199](https://www.zotero.org/google-docs/?q7bqaa)
>
> [McKinney, W. (2010). Data structures for statistical computing in
> Python. *Proceedings of the 9th Python in Science Conference*, *445*,
> 51--56.
> https://doi.org/10.25080/Majora-92bf1922-00a](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Min, S., Lyu, X., Holtzman, A., Artetxe, M., Lewis, M., Hajishirzi,
> H., & Zettlemoyer, L. (2022). Rethinking the role of demonstrations:
> What makes in-context learning work? *arXiv Preprint
> arXiv:2202.12837*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Moradi Dakhel, A., Majdinasab, V., Nikanjam, A., Khomh, F.,
> Desmarais, M. C., & Jiang, Z. M. (Jack). (2023). GitHub Copilot AI
> pair programmer: Asset or Liability? *Journal of Systems and
> Software*, *203*, 111734.
> https://doi.org/10.1016/j.jss.2023.111734](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Nelson-Le Gall, S. (1981). Help-seeking: An understudied
> problem-solving skill in children. *Developmental Review*, *1*(3),
> 224--246.
> https://doi.org/10.1016/0273-2297(81)90019-8](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Neuendorf, K. A. (2017). *The content analysis guidebook*.
> sage.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Newman, R. S. (1994). *Adaptive help seeking: A strategy of
> self-regulated learning.* Lawrence Erlbaum Associates,
> Inc.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Olga, A., Saini, A., Zapata, G., Searsmith, D., Cope, B., Kalantzis,
> M., Castro, V., Kourkoulou, T., Jones, J., da Silva, R. A., & others.
> (2023). Generative AI: Implications and Applications for Education.
> *arXiv Preprint
> arXiv:2305.07605*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Osborne, J. W., & Waters, E. (2002). Four assumptions of multiple
> regression that researchers should always test. *Practical Assessment,
> Research, and Evaluation*,
> *8*(1).](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Păvăloaia, V.-D., & Necula, S.-C. (2023). Artificial Intelligence as
> a Disruptive Technology---A Systematic Literature Review.
> *Electronics*, *12*(5), 1102.
> https://doi.org/10.3390/electronics12051102](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Pearce, H., Ahmad, B., Tan, B., Dolan-Gavitt, B., & Karri, R. (2022).
> Asleep at the keyboard? Assessing the security of github copilot's
> code contributions. *2022 IEEE Symposium on Security and Privacy
> (SP)*, 754--768.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Peng, S., Kalliamvakou, E., Cihon, P., & Demirer, M. (2023). *The
> Impact of AI on Developer Productivity: Evidence from GitHub Copilot*
> (No. arXiv:2302.06590). arXiv.
> http://arxiv.org/abs/2302.06590](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Perry, N., Srivastava, M., Kumar, D., & Boneh, D. (2023). Do Users
> Write More Insecure Code with AI Assistants? *Proceedings of the 2023
> ACM SIGSAC Conference on Computer and Communications Security*,
> 2785--2799.
> https://doi.org/10.1145/3576915.3623157](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Pilny, A., McAninch, K., Slone, A., & Moore, K. (2024). From manual
> to machine: Assessing the efficacy of large language models in content
> analysis. *Communication Research Reports*, *41*(2),
> 61--70.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Pintrich, P. R. (2003). A motivational science perspective on the
> role of student motivation in learning and teaching contexts. *Journal
> of Educational Psychology*, *95*(4),
> 667.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Pons, A. (2023). *Generative AI in the classroom: From hype to
> reality?*](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Prather, J., Denny, P., Leinonen, J., Becker, B. A., Albluwi, I.,
> Craig, M., Keuning, H., Kiesler, N., Kohn, T., Luxton-Reilly, A.,
> MacNeil, S., Petersen, A., Pettit, R., Reeves, B. N., & Savelka, J.
> (2023). The Robots Are Here: Navigating the Generative AI Revolution
> in Computing Education. *Proceedings of the 2023 Working Group Reports
> on Innovation and Technology in Computer Science Education*, 108--159.
> https://doi.org/10.1145/3623762.3633499](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Prather, J., Pettit, R., Becker, B. A., Denny, P., Loksa, D., Peters,
> A., Albrecht, Z., & Masci, K. (2019). First Things First: Providing
> Metacognitive Scaffolding for Interpreting Problem Prompts.
> *Proceedings of the 50th ACM Technical Symposium on Computer Science
> Education*, 531--537.
> https://doi.org/10.1145/3287324.3287374](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Prather, J., Reeves, B., Leinonen, J., MacNeil, S., Randrianasolo, A.
> S., Becker, B., Kimmel, B., Wright, J., & Briggs, B. (2024). *The
> Widening Gap: The Benefits and Harms of Generative AI for Novice
> Programmers* (No. arXiv:2405.17739). arXiv.
> http://arxiv.org/abs/2405.17739](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Prather, J., Reeves, B. N., Denny, P., Becker, B. A., Leinonen, J.,
> Luxton-Reilly, A., Powell, G., Finnie-Ansley, J., & Santos, E. A.
> (2024). "It's Weird That it Knows What I Want": Usability and
> Interactions with Copilot for Novice Programmers. *ACM Transactions on
> Computer-Human Interaction*, *31*(1), 1--31.
> https://doi.org/10.1145/3617367](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Python Software Foundation. (2023). *Python Programming Language*
> (Version 3.12) \[Computer software\].
> https://www.python.org](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Qian, Y., & Lehman, J. (2018). Students' Misconceptions and Other
> Difficulties in Introductory Programming: A Literature Review. *ACM
> Transactions on Computing Education*, *18*(1), 1--24.
> https://doi.org/10.1145/3077618](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Rahman, Md. M., & Watanobe, Y. (2023). ChatGPT for Education and
> Research: Opportunities, Threats, and Strategies. *Applied Sciences*,
> *13*(9), 5783.
> https://doi.org/10.3390/app13095783](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Raudenbush, S. W., & Bryk, A. S. (2002). *Hierarchical linear models:
> Applications and data analysis methods* (Vol. 1).
> sage.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Robins, A., Rountree, J., & Rountree, N. (2003). Learning and
> Teaching Programming: A Review and Discussion. *Computer Science
> Education*, *13*(2), 137--172.
> https://doi.org/10.1076/csed.13.2.137.14200](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Román-González, M., Pérez-González, J.-C., & Jiménez-Fernández, C.
> (2017). Which cognitive abilities underlie computational thinking?
> Criterion validity of the Computational Thinking Test. *Computers in
> Human Behavior*, *72*, 678--691.
> https://doi.org/10.1016/j.chb.2016.08.047](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Rudolph, J., Tan, S., & Tan, S. (2023). ChatGPT: Bullshit spewer or
> the end of traditional assessments in higher education? *Journal of
> Applied Learning & Teaching*, *6*(1).
> https://doi.org/10.37074/jalt.2023.6.1.9](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Ryan, R. M. (1982). Control and information in the intrapersonal
> sphere: An extension of cognitive evaluation theory. *Journal of
> Personality and Social Psychology*, *43*(3),
> 450.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Sarsa, S., Denny, P., Hellas, A., & Leinonen, J. (2022). Automatic
> generation of programming exercises and code explanations using large
> language models. *Proceedings of the 2022 ACM Conference on
> International Computing Education Research-Volume 1*,
> 27--43.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Savelka, J., Agarwal, A., An, M., Bogart, C., & Sakr, M. (2023).
> Thrilled by Your Progress! Large Language Models (GPT-4) No Longer
> Struggle to Pass Assessments in Higher Education Programming Courses.
> *Proceedings of the 2023 ACM Conference on International Computing
> Education Research V.1*, 78--92.
> https://doi.org/10.1145/3568813.3600142](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Savelka, J., Agarwal, A., Bogart, C., & Sakr, M. (2023). From gpt-3
> to gpt-4: On the evolving efficacy of llms to answer multiple-choice
> questions for programming classes in higher education. *International
> Conference on Computer Supported Education*,
> 160--182.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Schwarzer, R., & Jerusalem, M. (1995). Generalized self-efficacy
> scale. *J. Weinman, S. Wright, & M. Johnston, Measures in Health
> Psychology: A User's Portfolio. Causal and Control Beliefs*, *35*(37),
> 82--003.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Seabold, S., & Perktold, J. (2010). Statsmodels: Econometric and
> statistical modeling with Python. *Proceedings of the 9th Python in
> Science Conference*, 92--96.
> https://doi.org/10.25080/Majora-92bf1922-011](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Shanahan, M. (2024). Talking about Large Language Models.
> *Communications of the ACM*, *67*(2), 68--79.
> https://doi.org/10.1145/3624724](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Shaphiro, S., & Wilk, M. (1965). An analysis of variance test for
> normality. *Biometrika*, *52*(3),
> 591--611.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Sheese, B., Liffiton, M., Savelka, J., & Denny, P. (2024). Patterns
> of Student Help-Seeking When Using a Large Language Model-Powered
> Programming Assistant. *Proceedings of the 26th Australasian Computing
> Education Conference*, 49--57.
> https://doi.org/10.1145/3636243.3636249](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Shein, E. (2024). The Impact of AI on Computer Science Education.
> *Communications of the ACM*, *67*(9), 13--15.
> https://doi.org/10.1145/3673428](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Shen, L. (2024). *Forestplot* (Version 0.3) \[Computer software\].
> https://pypi.org/project/forestplot/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Shute, V. J., Sun, C., & Asbell-Clarke, J. (2017). Demystifying
> computational thinking. *Educational Research Review*, *22*, 142--158.
> https://doi.org/10.1016/j.edurev.2017.09.003](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Stiffler, L. (2025, July 10). Coding is dead: UW computer science
> program rethinks curriculum for the AI era. *GeekWire*.
> https://www.geekwire.com/2025/coding-is-dead-uw-computer-science-program-rethinks-curriculum-for-the-ai-era/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Tsai, M.-J., Liang, J.-C., & Hsu, C.-Y. (2021). The Computational
> Thinking Scale for Computer Literacy Education. *Journal of
> Educational Computing Research*, *59*(4), 579--602.
> https://doi.org/10.1177/0735633120972356](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Vaithilingam, P., Zhang, T., & Glassman, E. L. (2022). Expectation
> vs. Experience: Evaluating the Usability of Code Generation Tools
> Powered by Large Language Models. *CHI Conference on Human Factors in
> Computing Systems Extended Abstracts*, 1--7.
> https://doi.org/10.1145/3491101.3519665](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Vallat, R. (2018). Pingouin: Statistics in Python. *Journal of Open
> Source Software*, *3*(31), 1026.
> https://doi.org/10.21105/joss.01026](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Vaz, S., Falkmer, T., Passmore, A. E., Parsons, R., & Andreou, P.
> (2013). The case for using the repeatability coefficient when
> calculating test--retest reliability. *PloS One*, *8*(9),
> e73990.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Virtanen, P., Gommers, R., Oliphant, T. E., Haberland, M., Reddy, T.,
> Cournapeau, D., Burovski, E., Peterson, P., Weckesser, W., Bright, J.,
> & others. (2020). SciPy 1.0: Fundamental algorithms for scientific
> computing in Python. *Nature Methods*, *17*(3), 261--272.
> https://doi.org/10.1038/s41592-019-0686-2](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Wang, T., Zhou, N., & Chen, Z. (2024). *Enhancing computer
> programming education with LLMs: A study on effective prompt
> engineering for Python code generation* (No. arXiv:2407.05437). arXiv.
> https://doi.org/10.48550/arXiv.2407.05437](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Waskom, M. L. (2021). seaborn: Statistical data visualization.
> *Journal of Open Source Software*, *6*(60), 3021.
> https://doi.org/10.21105/joss.03021](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Wei, J., Bosma, M., Zhao, V. Y., Guu, K., Yu, A. W., Lester, B., Du,
> N., Dai, A. M., & Le, Q. V. (2022). *Finetuned Language Models Are
> Zero-Shot Learners* (No. arXiv:2109.01652). arXiv.
> http://arxiv.org/abs/2109.01652](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Wei, J., Wang, X., Schuurmans, D., Bosma, M., Ichter, B., Xia, F.,
> Chi, E. H., Le, Q. V., & Zhou, D. (2022). *Chain-of-Thought Prompting
> Elicits Reasoning in Large Language
> Models*.](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Weisz, J. D., Kumar, S. V., Muller, M., Browne, K.-E., Goldberg, A.,
> Heintze, K. E., & Bajpai, S. (2025). Examining the Use and Impact of
> an AI Code Assistant on Developer Productivity and Experience in the
> Enterprise. *Proceedings of the Extended Abstracts of the CHI
> Conference on Human Factors in Computing Systems*, 1--13.
> https://doi.org/10.1145/3706599.3706670](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Wing, J. M. (2008). Computational thinking and thinking about
> computing. *Philosophical Transactions of the Royal Society A:
> Mathematical, Physical and Engineering Sciences*, *366*(1881),
> 3717--3725.
> https://doi.org/10.1098/rsta.2008.0118](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Wing, J. M. (2011). Research Notebook: Computational Thinking---What
> and Why? *Unpublished Manuscript*.
> https://www.cs.cmu.edu/\~CompThink/resources/TheLinkWing.pdf](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Xiao, Z., Yuan, X., Liao, Q. V., Abdelghani, R., & Oudeyer, P.-Y.
> (2023). *Supporting Qualitative Analysis with Large Language Models:
> Combining Codebook with GPT-3 for Deductive Coding*. 75--78.
> https://doi.org/10.1145/3581754.3584136](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Xu, R. (2024). *Sankeyflow* (Version 0.4.1) \[Computer software\].
> https://pypi.org/project/sankeyflow/](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Yilmaz, R., & Karaoglan Yilmaz, F. G. (2023). Augmented intelligence
> in programming learning: Examining student views on the use of ChatGPT
> for programming learning. *Computers in Human Behavior: Artificial
> Humans*, *1*(2), 100005.
> https://doi.org/10.1016/j.chbah.2023.100005](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Zapata-Cáceres, M., Marcelino, P., El-Hamamsy, L., & Martín-Barroso,
> E. (2024). A Bebras Computational Thinking (ABC-Thinking) program for
> primary school: Evaluation using the competent computational thinking
> test. *Education and Information Technologies*.
> https://doi.org/10.1007/s10639-023-12441-w](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Zhao, W. X., Zhou, K., Li, J., Tang, T., Wang, X., Hou, Y., Min, Y.,
> Zhang, B., Zhang, J., Dong, Z., Du, Y., Yang, C., Chen, Y., Chen, Z.,
> Jiang, J., Ren, R., Li, Y., Tang, X., Liu, Z., ... Wen, J.-R. (2023).
> *A Survey of Large Language Models* (No. arXiv:2303.18223). arXiv.
> http://arxiv.org/abs/2303.18223](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Ziegler, A., Kalliamvakou, E., Li, X. A., Rice, A., Rifkin, D.,
> Simister, S., Sittampalam, G., & Aftandilian, E. (2022). Productivity
> assessment of neural code completion. *Proceedings of the 6th ACM
> SIGPLAN International Symposium on Machine Programming*, 21--29.
> https://doi.org/10.1145/3520312.3534864](https://www.zotero.org/google-docs/?q7bqaa)
>
> [Zimmerman, B. J. (2002). Becoming a Self-Regulated Learner: An
> Overview. *Theory Into Practice*, *41*(2), 64--70.
> https://doi.org/10.1207/s15430421tip4102\_2](https://www.zotero.org/google-docs/?q7bqaa)
> stensen, C. M., McDonald, R., Altman, E. J., & Palmer, J. E. (2018).
> Disruptive Innovation: An Intellectual History and Directions for
> Future Research. *Journal of Management Studies*, *55*(7), 1043--1078.
> https://doi.org/10.1111/joms.12349

[^1]: [[https://base44.com]{.underline}](https://base44.com)

[^2]: [[https://cursor.com]{.underline}](https://cursor.com)

[^3]: [[https://lovable.dev]{.underline}](https://lovable.dev)

[^4]: [[https://replit.com]{.underline}](https://replit.com)

[^5]: [[https://github.com/features/copilot]{.underline}](https://github.com/features/copilot)

[^6]: [[https://kiro.dev/]{.underline}](https://kiro.dev/)

[^7]: [[https://antigravity.google/]{.underline}](https://antigravity.google/)

[^8]: [[https://code.claude.com/]{.underline}](https://code.claude.com/)

[^9]: [[https://openai.com/codex/]{.underline}](https://openai.com/codex/)

[^10]: [[https://ist256.com/spring2025/syllabus]{.underline}](https://ist256.com/spring2025/syllabus)

[^11]: [[https://ai.ist256.com]{.underline}](https://ai.ist256.com)

[^12]: [[https://ai.ist256.com]{.underline}](https://ai.ist256.com)

[^13]: [[https://streamlit.io]{.underline}](https://streamlit.io)

[^14]: [[https://github.com/cent-ischool/ist256-chatapp]{.underline}](https://github.com/cent-ischool/ist256-chatapp)

[^15]: [[https://chatgpt.com/]{.underline}](https://chatgpt.com/)

[^16]: [[https://claude.ai/]{.underline}](https://claude.ai/)

[^17]: [[https://ollama.com/library/dolphin3]{.underline}](https://ollama.com/library/dolphin3)

[^18]: [[https://ollama.com/library/llama3]{.underline}](https://ollama.com/library/llama3)

[^19]: [[https://ollama.com/library/codellama]{.underline}](https://ollama.com/library/codellama)

[^20]: [[https://ollama.com/library/qwen2.5]{.underline}](https://ollama.com/library/qwen2.5)

[^21]: [[https://platform.openai.com/docs/models/gpt-4o-mini]{.underline}](https://platform.openai.com/docs/models/gpt-4o-mini)

[^22]: [[https://platform.openai.com/docs/models/gpt-4o]{.underline}](https://platform.openai.com/docs/models/gpt-4o)

[^23]: [[https://openrouter.ai]{.underline}](https://openrouter.ai)

[^24]: [[https://github.com/mafudge/dps-thesis]{.underline}](https://github.com/mafudge/dps-thesis)

[^25]: [[https://openrouter.ai/x-ai/grok-4-fast]{.underline}](https://openrouter.ai/x-ai/grok-4-fast)

[^26]: [[https://openrouter.ai/openai/gpt-5-mini]{.underline}](https://openrouter.ai/openai/gpt-5-mini)

[^27]: [[https://openrouter.ai/google/gemini-2.5-flash]{.underline}](https://openrouter.ai/google/gemini-2.5-flash)

[^28]: [[https://openrouter.ai/anthropic/claude-sonnet-4]{.underline}](https://openrouter.ai/anthropic/claude-sonnet-4)

[^29]: [[https://cloud.google.com/solutions/learnlm]{.underline}](https://cloud.google.com/solutions/learnlm)
