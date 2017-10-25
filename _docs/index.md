---
title: Empirical Study
permalink: /docs/home/
redirect_from: /docs/index.html
---

## Contributions
1. **A manual study of online code clones:**  
We used
two clone detection tools to discover 2,302 similar code snippet pairs between
72,365 Java code snippets obtained from Stack Overflow's accepted answers and
111 Java open source projects from the curated Qualitas
corpus. We manually
classified all of them.

2. **An investigation of toxic code snippets on Stack Overflow:**  
Our study shows that from
the 2,302 online clones, at least 330 have been copied from open source
projects or external online sources to Stack Overflow, potentially violating
software licenses. For 154 of them, we found evidence that they have been copied
from a specific open source project. 101 of them we found to be outdated.

3. **Awareness of Stack Overflow answerers to toxic code snippets:**  
We
performed an online survey and collected answers from 201 highly-ranked Stack
Overflow users. We found that they cloned code snippets from open source
projects to Stack Overflow answers. While Stack Overflow answerers are aware of
their outdated code snippets, 19% of the participants rarely
or never fix the code. 99% of the answerers never include a software
license in their snippets and 69% never check for licensing conflicts between the
cloned code snippets and Stack Overflow's CC BY-SA 3.0.

4. **An online code clone oracle:**
The 2,302 manually investigated and validated online clone pairs
are available for download [here](../../downloads.html) and
can be used as a clone oracle.

## Research Questions

1. **RQ1 (Online code clones)**:  

   *To what extent is source code cloned between Stack Overflow and open source projects?*

    We quantitatively measured the number of online code clones between Stack
  	Overflow and open source projects to understand the scale of the
  	problem.
2. **RQ2 (Patterns of online code clones):**  

   *Why do online code clones occur?*  

   We categorised online clones into seven categories allowing insights to why online code clones are created.
3. **RQ3 (Outdated online code clones):**  

    *Are
		online code clones up-to-date compared to their counterparts in the
		original projects?*  

    We were interested in the outdated Stack
	Overflow code examples since users are potentially reusing
	them.
4. **RQ4 (Software licensing violation):**  

    *How often do
		licensing conflicts occur between Stack Overflow clones and their
		originals?*  

    We investigated whether the reuse of online code clones
	can cause software developers to violate licenses.
5. **RQ5 (Stack Overflow answerers' awareness):**

	*1) How often are Stack Overflow
		answerers aware of the outdated code when
		they answer a question on Stack Overflow?*

	*2) How often are Stack Overflow
			answerers aware of licensing conflicts when
			they answer a question on Stack Overflow?*

	We surveyed 607 high reputation Stack Overflow users to study their
	awareness of the two issues.
