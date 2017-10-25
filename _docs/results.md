---
title: Results
permalink: /docs/results/
---

### RQ1: Online Code Clones
#### *To what extent is source code cloned between Stack Overflow and open source projects?*

<p style="text-align: center;">Table 1: Investigated online clone pairs and corresponding snippets and Qualitas projects</p>

Set | Pairs | Snippets | Projects | Cloned ratio
--- | ----: | -------: | -------: | -----------:
Reported clones | 2,302 | 460 | 59 | 53.10%
--- | ----- | -------- | -------- | ------------
TP from manual validation | 2,076 | 443 | 59 | 53.89%

> We found more than half (53%) of Qualitas projects to share
	similar code with Stack Overflow code snippets. In the manually confirmed
	data set of 2,302 clone pairs, we found 2,076 pairs as true positives which
	account for 59 Qualitas projects and
	443 Stack Overflow code snippets.

***

### RQ2: Patterns of Online Code Cloning
#### *Why do online code clones occur?*

<p style="text-align: center;">Table 2: Classifications of online clone pairs</p>

Set | QS | SQ | EX | UD | BP | IN | AC | Total
--- | --: | --: | --: | --: | --: | --: | --: | -----:
Before consolidation | 248 | 1 | 199 | 107 | 1,505 | 16 | 226 | 2,302
After consolidation | 154 | 1 | 111 | 65 | 217 | 9 | 53 | 560

> We found 154 pairs with
	strong evidences to be cloned from 23 Qualitas projects to Stack Overflow, 1 pair
	was cloned from Stack Overflow to Qualitas, and
	111 pairs were found to be cloned to Stack Overflow from external
	sources. However, the largest amount of the clone pairs
	between Stack Overflow and Qualitas projects are boiler-plate code
	(217), followed by 65 clone pairs with no evidence that the code has actually been copied,
	and 16 pairs of clones due to implementing the same interface or inheriting the same class.

***

### RQ3: Outdated Online Code Clones
#### *Are online code clones up-to-date compared to their counterparts in the original projects?*

<p style="text-align: center;">Figure 1: Outdated QS online clone pairs group by projects</p>

![outdated code](../../img/outdated.png "Outdated Code")

<p style="text-align: center;">Table 3: Six code modification types found when comparing the outdated clone pairs to their latest versions</p>

Modification | Occurrences
------------ | -----------:
Statement modification | 50
Statement addition | 28
Statement removal | 18
Method signature change | 16
Method rewriting | 15
File deletion | 15

<p style="text-align: center;">Table 4: Examples of the outdated QS online clones (see full results in the Interactive menu)</p>

Post | Date | Project | File | Start | End | Date | Issue ID | Type* | Date
---- | ---- | ------- | ---- | ----: | --: | ---- | -------- | ----- | ----
2513183 | 25/3/10 | eclipse | GenerateTo<br />StringAction.java | 113 | 166 | 5/6/13 | Bug 439874 | *S* | 17/3/15
22315734 | 11/3/314 | hadoop | Writable<br />Comparator.java | 44 | 54 | 25/8/11 | HADOOP-11323 | *S* | 20/11/14
23520731 | 7/5/14 | hibernate | Schema<br />Update.java | 115 | 168 | 22/5/13 | HHH-10458 | *S* | 5/2/16
18232672 | 14/8/13 | log4j | SMTP<br />Appender.java | 207 | 228 | 31/3/10 | Bug 44644 | *R* | 18/10/08
17697173 | 17/7/13 | lucene | SlowSynonym<br />FilterFactory.java | 38 | 52 | 6/4/13 | LUCENE-4095 | *D* | 31/5/12
21734562 | 12/2/14 | tomcat | Form<br />Authenticator.java | 51 | 61 | 4/8/10 | BZ 59823 |*R* | 4/8/16
12593810 | 26/9/12 | poi | Workbook<br />Factory.java | 49 | 60 | 7-Dec-09 | 57593 | *R* | 30/4/15
8037824 | 7/11/11 | jasper<br />reports | JRVerifier.java | 1221 | 1240 | 31/5/10 | N/A | *D* | 20/5/11
3758110 | 21/9/10 | spring | Default<br />Annotation<br />Handler<br />Mapping.java | 78 | 92 | 20/10/10 | SPR-14129 | *D* | 20/1/12
14019840 | 24/12/12 | struts | Default<br />ActionMapper.java | 273 | 288 | 17-Jul-10 | WW-4225 | *S* | 18/10/13

Note: *S*: modified/added/deleted statements, *D*: file has been deleted,  *R*: method has been rewritten completely

> Our results show that 66% (101) of QS clone pairs on Stack
	Overflow are outdated. 86 pairs differ from their newest versions by
	modifications applied to variable names or method names, added or deleted
	statements, to a fully rewritten code with new method signatures. 15 pairs are
	dead snippets.

***

### RQ4: Software Licensing Violation
#### *Do licensing conflicts occur between Stack Overflow clones and their originals?*

<p style="text-align: center;">Table 5: License mapping of online clones (file-level)</p>

Type | Qualitas | Stack Overflow (CC BY-NC-SA)| QS | EX | UD
---- | -------- | --------------------------- | --: | --: | --:
Compatible | Apache-2 | Apache-2 | 1 | |
			| EPLv1 | EPLv1 | 2 | | 1
			| Proprietary | Proprietary | | 2 |
			| Sun Microsystems | Sun Microsystems | | 3 |
			| No license | No license | 20 | 9 | 2
			| No license | CC BY-SA 3.0 | | 1 |
**Total** | | | **23** | **15** | **3**
Incompatible | AGPLv3/3+ | No license | 1 | | 4
			| Apache-2 | No license | 46 | 14 | 12   
			| BSD/BSD3 | No license | 4 | | 1
			| CDDL or GPLv2 | No license | | | 6
			| EPLv1 | No license | 10 | | 6
			| GPLv2+/3+ | No license | 8 | 48 | 7
			| LesserGPLv2.1+/3+ | No license | 16 | | 9  			
			| MPLv1.1 | No license | | | 1
			| Oracle | No license | | 3
			| Proprietary | No license | | 1 | 2
			| Sun Microsystems | No license | | 1 | 2
			| Unknown | No license | | 11 |
			| LesserGPLv2.1+ | New BSD3 | 1 | |
**Total** | | | **86** | **78** | **50**

> We found 214 code snippets on Stack Overflow that
	could violate the license of their original software. The majority of them
	do not contain licensing statements after they have been copied to
	Stack Overflow. For 164 of them, we were able to identify,
        with evidence, where the code snippet has been copied from.

***

### RQ5: Stack Overflow Answerers' Awareness

#### General information

<p style="text-align: center;">Table 6: Stack Overflow answerers taken the survey</p>

Reputation | Sent emails | Answers | Rate
---------- | ----------: | ------: | ---:
963,731-6,999 | 607 | 201 | 33%

<p style="text-align: center;">Table 7: Experience of Stack Overflow answerers</p>

Experience | Amount | Percent
---------- | -----: | -------:
Less than a year | 1 | 0.5%
1 -- 2 years | 1 | 0.5%
3 -- 5 years | 30 | 14.9%
5 -- 10 years | 58 | 28.9%
More than 10 years	| 111 | 55.2%

#### Code Snippets in Answers

<p style="text-align: center;">Table 8: Frequency of including code snippets in answers</p>

Include code snippets | Amount | Percent
--------------------- | -----: | ------:
Very Frequently (81--100% of the time)	| 84 | 42%
Frequently (61--80% of the time) |	63 | 31%
Occasionally (41--60% of the time) | 40 | 20%
Rarely (21--40% of the time) | 11 | 6%
Very Rarely (1--20% of the time) | 2 | 1%
Never (0% of the time) | 1 | 1%
Total | 201 | 100%

<p style="text-align: center;">Figure 2: The sources of code snippets in Stack Overflow answers</p>

![snippet sources](../../img/snippet_source.png "Snippet Sources")

***
