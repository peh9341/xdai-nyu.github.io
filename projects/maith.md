# **Solve For WHY**

### **An AI-powered mathematics “playground” for user-directed discovery learning and recreation.**

## **Bair \+ Penny Hays**

### **Table of Contents**

[Abstract](#abstract)

[Educational Assessment Methods Steer Math Learning Off-Track](#educational-assessment-methods-steer-math-learning-off-track)

[Solve For WHY | Users, Objectives, and Strategies](#solve-for-why--users-objectives-and-strategies)

[Mathematics *Recreation?*](#mathematics-recreation)

[Solve For WHY | System Overview](#solve-for-why--system-overview)

[Solve For WHY | Prototypes \+ Development](#solve-for-why--prototypes--development)

[Evaluating Solve For WHY](#evaluating-solve-for-why)

[Detailed Evaluation Plan | click to access](#detailed-evaluation-plan-click-to-access)

[Early Evaluation Findings](#early-evaluation-findings)

[Ethical Implications](#ethical-implications)

[Future Work | Penny Hays](#future-work--penny-hays)

[Future Work | Bair](#future-work--bair)

[Appendix 1 | Second Prompt For Replit | click to access](#appendix-1--second-prompt-for-replit-click-to-access)

[References](#references)

## 

---

### Abstract 

American students are struggling in math. Steep declines in competency scores recorded between 2019 \- 2023 are partially attributable to disruptions associated with COVID19, but are part of a larger trend traceable to how current assessment methods shape school pedagogy. High-stakes testing effectively obviates the very strategies and features shown to be effective for math learning, such as exploratory discovery learning, mastery goal orientation, intellectual risk-taking, mistake-making and disequilibrium, and strips math of the context and relevance that makes it meaningful, interesting, rewarding and intrinsically motivating for students. A **counter-tool** is proposed \- a tech-based platform to support a different set of *learning values* and comprise a wholly different learning context outside of the traditional K-12 space. *Solve For WHY* uses a low-stakes, curriculum-free *recreational context* to offer active, self-directed discovery learning; reconnect math content to context, meaning, history, and real-world relevance; support the intellectual risk-taking and disequilibrium that feed intrinsic motivation, deep conceptual understanding and a mastery goal orientation. **AI provides** access to unlimited content and inquiry for any level of learner, significant flexibility and customization, and just-in-time support, on demand and at low/no cost. An evaluation framework and potential future work are discussed.

---

### **Educational Assessment Methods Steer Math Learning Off-Track**
<br>

Education requires assessment. We need to know how teaching and instructional designs are working, what problems may be occurring, and whether students have the knowledge and skills they need for the future \- their individual futures, and our shared future as a society (Jimenez & Modaffari, 2021\). **But impacts of our current means of assessment \- usually the last step in a learning process \- are boomeranging back into our pedagogy and warping the student experience of mathematics learning** (Jimenez & Modaffari, 2021\)**.**

Standardized assessment is the easiest, most scalable, seemingly most direct way to gather student competency data; when we want to know what students know \- nationwide, or in an individual classroom \- we test them on it.  
**Current standardized assessment methods for mathematics tend to operationalize *procedural fluency*** \- students learn a procedure, and are tested on their ability to accurately reproduce and apply that procedure in various situations. But is procedural fluency the same as deep understanding the mathematical concepts that animate that procedure, give it meaning, or compelled its invention in the first place? Not necessarily. And data shows that those aspects of math learning that give it life and meaning \- contexts that intrigue and fascinate, concepts that express the beauty of math, historical origins and real-world applications that proves its relevance \- are inevitably, if unintentionally, sacrificed from math pedagogy due to limited time and enormous pressure on students, teachers, schools and districts to perform well on procedure-based assessments. 

> “The tests result in teaching to the test. Is this claim true or false? It is true. A 2007 review of 49 studies found that 80 percent of the studies saw a change in curriculum and increased focus on teacher-led instruction (McMurrer, 2007). Generally, “teaching to the test” means “teaching in a manner that is not considered optimal for learning standard content or skills, but is believed to improve test performance” (Phelps, 2016).”					
> 
> \- Jimenez & Modaffari, 2021
<br>

What we operationalize in assessments ends up informing what we teach, and *how*. For example, active discovery learning may be a good way to teach conceptual understanding. But it’s not a good way to teach procedural fluency. So we trade **bottom-up activities** \- conjecture, discussion, diverse strategizing \- that cultivate conceptual understanding, creativity, critical thinking and collaboration \- skills that are vital in real world situations where solutions often aren’t clear \- for **top-down procedural learning largely untethered from context, meaning or relevance** (Boaler & LeBlanc, 2025). There’s also evidence that while current K-12 math curricula remains relevant for some professions it’s increasingly irrelevant for most students and is not serving them well (Boaler & LeBlanc, 2025): 

> “I'm still kind of perplexed as to why we still teach trigonometry and calculus as opposed to data science in  
in high schools….
>
> The argument is given that it is inequitable to offer kids a different pathway. It will stop black and brown kids from doing well in life because it will pull them off the calculus pathway and the calculus pathway is what is so important. So they share that argument \- that this is an inequitable set of affairs, offering kids data science. And people believe it. But actually what you see is when data science pathways are in high schools, they bring in a lot more kids who are more diverse, who haven't been traditionally successful \- they take a course in data science and they start to see that maths can be really relevant and they get really into it and they go into STEM. So, it's frustrating.”	
>
> \- Jo Boaler, on unSILOed podcast with Gregory LaBlanc, Episode 551, Jun 11, 2025, 28:40
<br>

We believe this learning context is directly linkable to data that shows **students are disinterested in mathematics and feel it’s not relevant to their lives.** 49% of middle and high school respondents to 2025 American Youth Panel surveys reported losing interest in math about half or more of the time, and 75% reported losing interest for at least some class time (Schwartz, et al, 2025). This loss of interest is consistent across genders and racial and ethnic groups (Schwartz et al, 2025). A few direct quotes from this research surface key additional details: 

> “Students who are the most likely to maintain interest in math are the same ones who comprehend math, feel supported in math, are confident in their ability to do well in math, enjoy math, believe in the need to learn math, and see themselves as a math person.” (Schwartz et al, 2025, pp. 1\)
> 
> “Thirty percent of middle and high school students said that they have never considered themselves a “math person.” Those who did identify as math people developed this view during elementary school.” (Schwartz et al, 2025, press release)
<br>

Data also shows that **American students lack basic math competency.** The Trends in International Mathematics and Science Study (TIMSS) revealed “sharp, steep declines” in math competency between 2019 and 2023 (Carr, 2024, in Schwartz, 2024). Competency scores of 4th graders dropped 18 points during this period, while 8th graders dropped 27 \- the largest drop since the U.S. joined the study in 1995 (Schwartz, 2024). These losses are partially attributable to disruptions associated with COVID19, but declines were seen prior to the pandemic (Schwartz, 2024\) and studies conducted post-pandemic show minimal recovery (NAEP, 2024).

It’s also been shown that math learning is powered by **risk-taking, mistake-making, and disequilibrium** (Boaler, 2015\), tricky states and emotions that are, in fact, *intrinsic motivators* \- they **make math learning rewarding and help develop positive self-concept** in math learners, who gain hard-won “satisfaction of learning something new and knowing they can do it” ([Gray, 2013](https://kgmathminds.com/2013/04/18/embracing-disequilibrium/#:~:text=Disequilibrium%20in%20the%20way%20students,to%20see%20teachers%20teaching%20students.)). Satisfactions related to Self Determination Theory such as autonomy and competence (Samuelsson, 2021\) take time to achieve, requiring an appropriate, safe, supportive context conducive to risk-taking and ‘graceful failure’ be sustained over time. But high-stakes testing exerts pressure to perform, infusing every pedagogical ‘beat’ that comes before with pressure to *prepare* to perform, which can spark anxiety, discourage risk-taking, and turn mistake-making and disequilibrium from constructive into destructive experiences (Boaler, 2015; [Singh, 2025](https://sunilsingh-42118.medium.com/the-joy-of-teaching-mathematics-without-a-curriculum-69c7ea589028)). Perhaps the most extreme outcome of a stressful math learning environment is **math anxiety**, which is increasing worldwide (Schwartz, 2024). 

<br>

<figure>
    <img src="https://drive.google.com/uc?export=view&id=/file/d/10L5wmWF2FNAldbEhIZ29FL22OmI7zEwn"
    <figcaption>Table: increase in self-reports of math anxiety in the U.S. (Schwartz, 2024)</figcaption>
</figure>

<figure>
    <img src="https://drive.google.com/file/d/10L5wmWF2FNAldbEhIZ29FL22OmI7zEwn/view"
    <figcaption>Table: increase in self-reports of math anxiety in the U.S. (Schwartz, 2024)</figcaption>
</figure>

1_mathAnxiety_tracking.png

2_mathAnxiety_US.png

<br>

The following passages detail the significant, widespread, lasting impacts of this condition:
<br>
<br>

>“Mathematics anxiety is a negative emotional reaction towards mathematics that can be described as ‘feelings of tension, apprehension, or fear that interfere with mathematical performance’ (Richardson & Suinn, [1972](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#), p. 551). The consistency of the individual effects of mathematics anxiety across countries (Lau et al., [2022](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#)) is concordant with the idea that mathematics anxiety is a ‘global phenomenon’ (Foley et al., [2017](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#), p. 52\) and highlights the universality of the adverse effects of mathematics anxiety which can manifest in various ways including feelings of tension, apprehension or even fear. These negative emotional responses can occur in both academic and non-academic situations (Ashcraft, [2002](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#)), and have been shown to cause emotional, psychological and even physical pain (Lyons & Beilock, [2012](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#)). A further consequence of mathematics anxiety would be the development of negative attitudes and limiting beliefs about the subject which can lead to apathy, defined as a motivation and a lack of interest, and the manifestation of further stronger negative emotions towards the subject like ‘I hate mathematics and I would rather die’ (Brown et al., [2008](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#), p. 6\) than study mathematics.”
>
>“Mathematics anxiety is therefore significantly associated with mathematics avoidance behaviours and a wide spectrum of self-motivation measures (Hembree, [1990](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#)). For example, self-efficacy and self-concept are two widely used self-motivation measures which are both negatively associated with mathematics anxiety (Ahmed et al., [2012](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#); Li et al., [2021](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#)). The relationship between mathematics anxiety and mathematics ability has been studied since the 1950s, with numerous meta-analyses showing a negative association between mathematics anxiety and mathematics ability in all levels of education (e.g. Barroso et al., [2021](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#); Hembree, [1990](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#); Ma, [1999](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#); Namkung et al., [2019](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#)).”
>
>\- Smith, Fotou, & Sharpe, 2025, p. 1-2
<br>

Still, learning requires motivation. So current K-12 math tends to rely on extrinsic motivators like placements, scores and grades, and lauds external indicators like “performance” and “achievement”. Yet a 2011 study by Maltese and Tai found that interest in math and belief in its usefulness, rather than achievement or placement, was more predictive of students’ future pathways (Leyva et al., 2022). This suggests **intrinsic motivators make a stronger impression on math learners than extrinsic ones.** Other promising factors are **positive early experiences with math**, including sheer enjoyment and experiences of autonomy and competence (Ryan & Deci, 2017), which can promote a **positive attitude and positive self-concept with regard to math, including coming to consider oneself “a math person”** (Schwartz et al, 2025). This, in turn, has been shown to have a strong positive impact on later math engagement, resilience and performance (Schwartz et al, 2025). 

## 
---

### ***Solve For WHY*** **| Users, Objectives, and Strategies** 
<br>

Data shows that positive math experiences and experiences of self-efficacy are critically important for young math learners (Schwartz et al, 2025). But **in addition to serving math learners, a core goal of *Solve For WHY* is to investigate what AI, particularly evolving LLMs, may contribute to math learning environments and outcomes.** The novel opportunity LLMs make available is *rich content exploration*. Thus we have chosen to focus on a slightly older learner, who’ll have sufficient prior knowledge to engage all that AI-assisted content exploration can offer. We’ll revisit the needs of younger learners in a later section detailing intended future work. Our current design of *Solve For WHY* has **two specific users** in mind:

<br>

**1\) High schoolers (\~age 14-18) with lots of questions, frustrated by limits of school math.** 

3_persona1image.jpg

This learner may be frustrating their teacher, pushing their class “off course”, or “wasting time” with “off-topic” questions. They’re curious, driven to understand the larger context of what they’re learning in class \- underlying concepts, real-world relevance, connections to the broader world of math. They’re motivated to engage in self-directed learning. Edge cases include anyone from precocious middle schoolers to college undergraduates, and interested adults of all ages.

<br>

**2\) High schoolers (age 14-18) who’ve developed aversion, anxiety, or poor self-concept regarding math.**

4_persona2image.jpg

Past experiences and feedback from others (even passive) have informed negative schemas and limiting beliefs that shape these learners’ motivation and behavior. Neurological stress responses further derail their cognitive capacity to learn and perform, forming a feedback loop and reinforcing schemas. They’ll likely avoid educational, career, and retraining pathways that involve math, but positive experiences and support *if applied longitudinally* can improve things significantly (Weir, 2023). 

<br>

It would be reasonable to expect our **learning objectives** for these students to align with current high school math curricula. Indeed, the internet is loaded with applications that promise to enhance student performance in current K-12 math: 

>**Examples:** [Khan Academy](https://www.khanacademy.org/math), [Khanmigo](https://www.khanmigo.ai/), [DeltaMath](https://www.deltamath.com/), [IXL](https://www.ixl.com/high-school?_gl=1*lufk1w*_up*MQ..*_gs*MQ..&gclid=Cj0KCQiArt_JBhCTARIsADQZayka26lZUscwZBgJhnpf2O9qE3lb4nenUbpJ7yVuu5o2VxKc816JtREaAnZOEALw_wcB&gbraid=0AAAAADrr3AoAtApBqHKz5c6UdNje7650R), [PurpleMath](https://www.purplemath.com/), [Dreambox](https://www.dreambox.com/), [AdaptED](https://www.adaptedmind.com/Math-Worksheets.html?utm_medium=cpc&utm_source=google&campaignid=710817961&campaign_type=search&placement=g&utm_content=responsivesearchad&adid=680318766888&adset_id=37775542060&utm_term=adapted%20math&ad_position=&device=c&gad_source=1&gad_campaignid=710817961&gbraid=0AAAAADyJuNNY7IC4_Ry1JlD8tT31m9dVe&gclid=Cj0KCQiArt_JBhCTARIsADQZaymX2cCabpi4_vtfu6hH5VeKrmOioVQNrGfUbVAQ_njxIHvUponhEzYaAv3DEALw_wcB), [Prodigy](https://www.prodigygame.com/main-en), [Synthesis Tutor](https://www.synthesis.com/tutor)   
>**Core Goal:** Procedural fluency  
>**Sub-goals / learner goals:**
>
>* complete an assignment  
>* be able to replicate a specific skill or procedure at will  
>* prepare for assessment, meet a standard  
>* “catch up”   “get/stay ahead”  
>* obtain a score, grade, placement
>
>**Key activities:** practice, review, re-teach, remediate
<br>

But our needs assessment revealed that the learning environments these applications “serve”, as they aim to produce students who perform well on standardized assessments, don’t always reflect or promote (and may even discourage) specific skills, attitudes, metacognitive habits, real-world connections and deep conceptual understandings shown to be effective or even essential for building competent, real-world practitioners of mathematics.

In response, we aim to create a **wholly different learning context** that supports a specific set of **learning *values***, rather than a set of learning objectives.

<br>

For Persona 1, this alternative learning context would **provide** **access to a rich environment of explore-able math knowledge \- with AI performing the role of helpful guide and source of just-in-time support \-** that realizes what this student already suspects is true of the field of mathematics beyond their everyday classroom experience; this learning context *expresses* that math…

* Is interconnected  
* Is purposeful \- various aspects were “discovered” or “invented” for good reason  
* Is useful and omnipresent in the real world  
* Is fascinating and beautiful  
* Offers rich intrinsic rewards for going deep and spending time

<br>

For Persona 2, this same alternative learning context \- which lies beyond social scrutiny and maintains no goals beyond the student’s own \- would **gradually help reduce and remediate…**

* Negative attitudes toward math  
* Low self-concept as a math learner  
* Maladaptive strategies that have developed in their actual practice of math   
* Maladaptive metacognitive habits that inform how they meet challenges and interpret/manage disequilibrium during math learning  
* In cases of math anxiety, with appropriate longitudinal therapeutic application, amygdala activation and neurological and neurochemical stress responses 

And, as a possible secondary benefit, it would gradually increase the student’s positive experiences with math in a way that supports development of skills, attitudes, metacognitive habits, real-world connections and deep conceptual understanding that characterize competent, real-world math practitioners. 

<br>

**For Persona 1**, **the main need being tackled is the learner’s experience of friction between their own intrinsic interest in math and the pedagogical space where most of their math engagement takes place.** The “playground” aspect of *Solve For WHY* is what’s important here. A child who wants to explore and play in a playground in a self-directed way experiences “diminished returns” if their experience is heavily constrained by top-down structures, rules, directions, restrictions, and programmed ways-of-doing. Our design of *Solve For WHY* intends to set Persona 1 loose in the world of math to “play” to their heart’s content.

5_playgrounds.png

**Strategy for Persona 1 |Exploratory, self-directed, playful, and recreational learning:** Build skills and learn new concepts through self-directed exploration and discovery, with less overt focus on a specific external outcome.

<br>

**For Persona 2, the main need being tackled is the learner’s *acquired* negative personal orientation toward, and self-experience in, math.** When students struggle in high-stakes, top-down learning environments they can develop aversion to intellectual disequilibrium, risk-taking and mistake-making, and a fatalistic view of “how things will go” for them in math. An internal voice or sense develops, designed by the individual’s own subconscious to limit or curtail engagement as a form of self-protection against what the affective systems perceive as harm: “I’m not good at this.” “I don’t belong here.” “I can’t bear this.” “It’s never going to get better.” Negative behavioral responses and ongoing negative self-talk can develop into self-fullfilling negative engagements, creating a feedback loop that takes the learner further and further from positive engagement with math \- away from *even the possibility* of positive engagement with math.   
   
**Strategy for Persona 2 |Exploratory, self-directed, playful, and recreational learning:** A low/no-stakes learning environment that is as much a polar opposite of the conventional learning space as possible \- so much to be unrecognizable, with no triggers \- to “cool” internal resistance, anxiety and negativity, and basically move the barrier to entry all the way to the floor. The learner is in control, with a focus on fun and whatever the learner finds intrinsically interesting. No time or performance pressure. No peers or authority figures watching. No scores or goals or rubrics or means to measure oneself and find oneself lacking. All steps are taken to quiet negative affective response and self-talk, and liberate cognitive space to engage with math in a wholly different way. 

<br>

As we see, a common strategy is applied to both sets of learner needs. *Solve For WHY* aims to explore the potential of ***recreational mathematics*** to serve both sets of needs \- to fire intrinsic motivation, power persistence, support graceful failure, encourage risk-taking and mistake-making, contextualize disequilibrium as positive and even pleasurable, and restore the context, relevance, and mastery goal orientation that’ve been stripped away from current K-12 mathematics learning environments. *Solve For WHY* can be used in any setting, formal or informal, but **exists wholly outside of the traditional K-12 pedagogical context.** We hypothesize that this **novel learning environment** will generate **positive math experiences** that, over time, improve **math attitudes** and **learner self-concept**, extend time spent engaged with mathematics, and cultivate willingness to take intellectual risks and persist through disequilibrium. 

6_valuesCard.jpg

<br>

### **Mathematics *Recreation?***

>“It is more than mathematics done as a diversion, or playing games that involve mathematics. Recreational mathematics is inspired by deep ideas that are hidden in puzzles, games, and other forms of play.” 
>
>\- Mathematical Association of America, 2013

“Deep ideas” are the attraction of recreational mathematics. They’re fascinating, fun to explore, and key to the competence and autonomy satisfactions that fire intrinsic motivation and enhance learning (Ryan & Deci, 2017\). The pull of “deep ideas” inspires a self-directed, self-motivated exploratory process, while a recreational context preserves a playful valence. This kind of exploration can be geared toward any age or level of sophistication, and can inspire further study of mathematics in general or of a specific subject or content area within mathematics (Kulkarni, 2013). Learners of all ages have engaged in self-teaching, exploration, play and recreation with mathematics throughout recorded history, and a variety of online and offline tools are available to support, but…

* Many have **high barriers of entry,** or are **limited to** **early math concepts**  
* Videos \+ podcasts **lack interactability and participatory engagement**  
* Stand-alone puzzles offer **no opportunity to expand exploration \+ learning**  
* Most **lack any learner support functionality**. If you get stuck, your fun and learning are done.
<br>

Our design responds to the **need for a self-guided exploratory learning platform that offers positive experiences with math that have a low barrier to entry and are interactive, offering just-in-time learner support and the opportunity to progress, grow or learn new concepts and skills in math.** We believe that **AI contributes important, impactful features**, such as access to unlimited content and inquiry for any level of learner, significant flexibility, customization, and just-in-time support, on demand, at significantly less cost to learners than if these were provided person-to-person. This new learning environment **may not directly improve math competency**. But we hypothesize that it **will improve underlying factors that drive effective learning** \- attitudes, learner self-concept, willingness to sustain engagement, and view challenge and disequilibrium as positive conditions \- and that these improvements will thus ultimately drive improved math learning outcomes on a longitudinal scale. 

<br>

### 
---
### ***Solve For WHY*** **| System Overview** 
<br>

The *Solve For WHY*  interface includes four main features, three of which are shown in this early prototype:

<figure>
    <img src="add image link here"
    <figcaption>Early prototype of the Solve For WHY interface (Replit, Nov 9, 2025)</figcaption>
</figure>

7_earlyPrototype.png

<br>

**CHAT is the primary mode of interaction.** You might start by asking a specific question. If you did this with a standard chat bot \- say, Gemini Study Mode \- you’d simply get an answer.

<figure>
    <img src="add image link here"
    <figcaption>Example chat with Gemini “Study Mode”</figcaption>
</figure>

8_sampleGeminiChat.png

<br>

This is useful \- you’re informed \- but it’s not recreational, nor does it cultivate any of the learning states or processes that align with our *learning values.*  

*Solve For WHY* instead asks **guiding questions** that invite the user to consider what they may already know, and engage in a dialogue of inference- and connection-making, encouraging the user to identify, apply or extend what they may already know to the new concept they wish to explore. This is *mathematical reasoning.* As the user responds, the bot affirms any correct inferences and offers new guiding questions to help redirect incorrect ones. 

The interface also includes a **VISUAL DISPLAY** where either user or bot can post and manipulate any relevant or clarifying visuals that support the conversation or the user’s emerging understanding. It offers links to related **RESOURCES** where users can connect to new activities or communities that further feed knowledge or interests developed via engagement with *Solve For WHY*. And as the learner constructs their own mental models via the text exchange, *Solve For WHY* relates these to the broader world of mathematics by building a **CONCEPT MAP OF MATHEMATICS** originating with the current query. This feature centers the *conceptual nature* of mathematics, demonstrates the *interrelatedness* of math concepts and shows the *relevance* of mathematics practice. The map would start with a detail-view, showing the current query and a few surrounding nodes \- then, as the user returns and logs more inquiries the map will build, extend, and connect the new areas covered, revealing “neighbor” concepts may become new points of interest and extend engagement, and contribute to identity formation and competence satisfactions: “I am part of  this world.” “I am grasping concepts that relate to very sophisticated domains.” “I am a math person.”

<figure>
    <img src="add image link here"
    <figcaption>Example of inspiration for CONCEPT MAP feature</figcaption>
</figure>

9_mapOfMathematics.png

<br>

### 
---
### ***Solve For WHY*** **| Prototypes \+ Development** 


The original idea, which was based on some naivety as to how to combine modern machine learning methods, was to create training data from which an AI agent would learn. The hope was to create 10 full chat interactions (we ended up with 5\) that we could feed to the agent, but we realized that it would create better outcomes to have guidelines as well as a simple pedagogical flow for an agent to follow. Therefore, the purpose of creating these example chats was twofold:

1) The chats could serve as examples (rather than training data) for the AI agent  
2) By analysing the resulting chats ourselves, we could establish rules and a pedagogical flow for an AI agent

These example chats were created through focus group sessions where expert math teachers interacted with adult, novice math learners through a document that mimicked the chat interface. These sessions were conducted in-person and transparently; all parties had full knowledge of the purpose and structure of the interaction. Most of the initial inquiries were generated by the learners. Then, both parties, teachers and learners, took their time responding to each subsequent line, attempting to create **exemplar** chats. Then, after we created four total chats, teachers and learners attempted to discern rules and pedagogical flow through a group discussion, using a physical whiteboard as a notetaking aid. We hypothesize that valuing both learner and teacher knowledge resulted in more robust discussion and thereby better rules and flow. We then took the whiteboard notes, reorganized and formalized our ideas into rules and flow for the AI agent. 

| Rules | Flow |
| :---- | :---- |
| Invite to roleplay In the first 3-5 chats, attempt to get the user to THINK LIKE A MATHEMATICIAN. Do not invite the user to do this explicitly, but when the user demonstrates thinking like a mathematician, state, “Now you are thinking like a mathematician\!” or something akin to that.  Always have a **question back to the user, preferably end with that question**. Best if the question is open-ended and progresses the learner’s line of inquiry.  Never give learners important info related to the learning objective, but always confirm when they are right. Give historical context and maybe give clarification on terms and their definitions once a learner uses those terms themselves.  | Do a background knowledge assessment (ongoing throughout interaction) Establish representational infrastructure (created by the learner and ongoing throughout interaction) Create a sequence of guiding questions towards the learning objective. This objective is hidden to the learner to preserve playfulness. However, the learner and the bot co-create this objective based on the learner’s line of inquiry.  Look for evidence that the learner answered own question. When this happens, ask the learner what else they’d like to know. Let the learner respond before suggesting anything further.  |

Of course, using these exemplar chats as training data or examples for the AI could result in an agent that is unable to handle chats that went awry in some way, either through learner misuse or genuine confusions and misunderstandings between the learner and the chat bot. However, we believe that this issue could be solved in the future through iteration after larger scale user testing. Our goal was to get a functional prototype from which we would iterate, not to have something perfect from the beginning. 

Initially, we intended to produce this prototype from scratch using what we learned from the assignments in class. However, this proved too difficult and time consuming, and we changed our approach. After briefly examining the space of AI assisted app development, we landed on using Replit. In our first prompt, we described our front-end, our overall philosophy, and target pedagogical method: self-directed, exploratory learning of conceptual mathematics, but neglected to include explicit rules and flow. We then used a second prompt that also emphasized the explicit rules and flow. The second prompt we used for Replit can be found as the only entry in the appendix. 

For both initial prompts, Replit outputted a functional, near identical front-end chat bot interface. On the back-end, Replit outputted two different system prompts for the underlying AI agents. As expected, the first Replit prompt produced a system prompt without a pedagogical flow, whereas the second Replit prompt DID include a pedagogical flow. These system prompts can be found in the [ai.ts](http://ai.ts) file and are easily adjusted.  

We then set out to test how different AI agents functioned within our two apps. Initial prompt 1 we named MathSparkPlayRemix1 and the second prompt MathSparkPlayRemix2. We ran both apps through some of the exemplar inquiries in order to compare the AI’s output to the human output. The following table comically summarizes the results: 

|  | GPT-4 | Gemini 2.5 |
| ----- | :---- | :---- |
| MathSparkPlayRemix1 | Bad | Good |
| MathSparkPlayRemix2 (with explicit pedagogical flow) | Bad | Good |

There was way more variance between AI agents than between system prompts. It was extremely clear that GPT-4 did NOT understand the pedagogical philosophy we hoped to automate. Specifically and qualitatively, when doing a background knowledge assessment, GPT-4 seemed to be concerned about what the learner could DO, while Gemini 2.5 seemed to be concerned with what a learner KNOWS, even though the system prompt is clear about the emphasis on teaching conceptual knowledge. In addition, GPT-4 seemed to take a know-it-all tone and was generally unpleasant to interact with. It felt as if GPT-4 was the AI embodiment of the “Um. Actually,” stereotype. Gemini 2.5, by stark contrast, was generally successful both inducing positive emotions during the interaction and following the intended pedagogical flow even when the system prompt did not include an explicit flow. It seemed as if just from our general rules and philosophy that Gemini 2.5 understood its assignment.

Example of GPT-4 valuing procedural knowledge versus Gemini valuing conceptual knowledge:

>**Learner:** I want to learn more about different number bases in different cultures  
>**Gemini 2.5 version:** That's a fascinating area to explore\! Different cultures have indeed developed unique ways to represent numbers. To start, what do you already know about our own number system, the one we use every day?” 
>
>**Learner:** What is a limit?  
>**GPT-4 Version:** A limit can be a somewhat abstract concept in mathematics. First, let’s think about sequences. Can you describe a sequence that appears to approach a certain number, but never actually reaches it?

<br>

We then moved to testing Gemini 2.5 with and without an explicit pedagogical flow with the same learner inquiry, but ran into issues with the server disconnecting when tabbing out of Replit: 

|  MathSparkPlayRemix1 |  MathSparkPlayRemix2 |
| :---- | :---- |
| Learner: I want to learn more about different number bases in different cultures | Learner: I want to learn more about different number bases in different cultures |
| Bot: That's a wonderful area to delve into—mathematics and culture are deeply intertwined\! Before we look at different cultures, could you tell me a little about what you understand by a "number base" in mathematics? What's the system we use most commonly, and what does its "base" refer to? | Bot: That's a fascinating area to explore\! Different cultures have indeed developed unique ways to represent numbers. To start, what do you already know about our own number system, the one we use every day? |
| L: I think we use base 10\. I am not sure what the base refers to, but 10 is the first number with 2 digits instead of one. | L: I know we 0 through 9\. We have digits. We have 10's place and a hundreds place and so on. We have addition, subtraction, multiplication, and division, plus square roots and other things like that. |
| B: You're exactly right that we commonly use base 10\. It's interesting that you connect 10 to being the first number with two digits. What does that suggest about the \*number of unique single digits\* available in our base-10 system \*before\* we need to combine them to make larger numbers? | B: That's a great overview of our number system\! You've touched on several key ideas: the digits we use, the concept of place value, and the operations we perform with numbers. When you mention the "10's place and a hundreds place," what does that tell you about the number our system is built around? |
| CONNECTION TIMED OUT AND DELETED THE CHAT | L: I have no idea. Can we talk about different cultures now? |
|  | B: That's a great question about different cultures, and we'll certainly get there\! Understanding our own system's foundation will actually make it easier to see how other cultures developed theirs, as it provides a common point of comparison. You mentioned the "10's place and a hundreds place." What do you think is special about the number 10 in our number system, given those names? |
|  | L: Fine. Um. 10 is the first number with two digits? |
|  | B: That's an interesting observation about 10 being the first two-digit number. Let's think about it another way: When you're counting individual items, how many do you count before you typically bundle them together to make a new group? |
|  | CONNECTION TIMED OUT AND DELETED THE CHAT |

<br>

We would like to highlight the right side of the table above, which displays responses from Gemini 2.5 with explicit pedagogical flow in the system prompt. We believe this chat shows the great potential of this app. Gemini closely adheres to a socratic method, even when the learner becomes impatient (or, rather when Bair role-plays becoming impatient). Yet, it still honors the learner’s impatience, offering encouragement and assurance that, indeed, together they will get to what the learner wants to know. We sense, although this is not verifiable because of the black box nature of generative AI, that Gemini has created some sort of line of questioning that it wants to follow and gently guides the learner along this line, asking more and more leading questions if the learner is not answering what the AI expects to hear. After a few more test inquiries with MathSparkPlayRemix2 that also performed admirably, we decided that this was the model that would move on to user testing. 

Note that while we are happy with MathSparkPlayRemix2, it has proved difficult to compare different system prompts given Gemini’s generally good performance and the bugginess of Replit. We hope that user research will generate enough novel inquiries such that we can create a bank of inquiries to be able to test subtle differences between system prompts. This could include additions to the system prompt such as, “Ask the user a clarifying question about their statement when they use imprecise language.” Or, removing certain pieces of the system prompt, such as the seemingly unnecessary, “Never use emojis.”

We also intend to continue testing as Google and OpenAI release new agent models, such as Gemini 3\. Future testing may also include Claude if we can obtain an API key. We will use the following rubric to evaluate the bot’s performance internally and in small scale user testing, although this rubric is subject to change in the future: 

| Category | Category description | Score (1-5) |
| :---- | :---- | :---- |
| Pedagogical Quality | Does the AI use the intended teaching strategies, like providing analogies, asking guiding questions, asking open inquiry questions or identifying core misconceptions? |  |
| Feedback & Assessment | Does the AI accurately identify errors in a student's work and provide clear, adaptive, and constructive feedback without employing direct instruction? Does the AI properly identify when the student is thinking like a mathematician and reward that with encouragement, or in some other way reinforce that behavior?  |  |
| Handling Complex Queries | Can the AI manage multi-step inquiry or ambiguous student questions? |  |
| Affective Effects | Does the AI create a warm and inviting environment that is still demanding of the learner?  |  |
| Error Handling | How does the AI respond when it doesn't know an answer or misunderstands the student? |  |
| Domain Knowledge | Is the AI accurate and knowledgeable about the subject it's supposed to be teaching? |  |
| Context-Awareness | Does the AI remember what was said earlier in the conversation and respond appropriately? |  |

<br>

**AI Agents Unrelated to Chat Bot**  
The concept map and resources sections, while both technically there, are nowhere near the required quality needed to progress to user testing on a larger scale. These sections were included in the initial prompt for Replit, but were not given as much attention as the chat bot. These functionalities will probably require setting up additional AI agents and back-end adjustments. We plan on adding the ability to save resources as well as adjust the resource recommendation agent such that it gives less mainstream options. The concept map needs significant adjustments. 

<br>

**Affective Design**   
Currently, the user interface is lacking affective design features. While we are aware of how to apply affective design principles as they relate to educational technology, implementing these principles will take additional time, will not happen this semester, and may require consultation outside of this team. Our initial prompt to Replit did not give much attention to this matter. 

##
---

### **Evaluating *Solve For WHY*** 

Evaluation of our design can be divided into two main study domains: **Immediate** and **Longitudinal.**

First, are interactions with *Solve For WHY* producing the **immediate responses** we expect? Are the Presentation Model elements of our Evidence Centered Design (see below) generating the Task Model and Learner Model outcomes we expect? If not, why, and what is happening instead? This information would potentially inform redesign toward more effective outcomes, or perhaps force us to rethink our underlying hypotheses. 

10_persona1Card.jpg 

11_persona2Card.jpg

<br>

Then, our core hypothesis is that *Solve For WHY* generates **positive math experiences** that, over time, improve **math attitudes** and **learner self-concept**, extend time spent engaged with mathematics, and cultivate willingness to take intellectual risks and persist through disequilibrium. Longitudinal studies would sample math attitudes, learning habits, and learner self-concept \- plus generalized and math-specific anxiety, in the case of Persona 2 \- of study participants prior to first use of *Solve For WHY*, intermittently during a prescribed period of use, and at the end of a prescribed period of use. We would also conduct longitudinal experiments comparing types of math experiences (positive, negative, neutral, and quantity of each), outcomes (changes in attitude and/or learner self-concept), and habits (time spent, willingness to take intellectual risks and persist through disequilibrium) generated during/by longitudinal use of *Solve For WHY* versus longitudinal use of other AI-based math meaning applications.

<br>

###  **Detailed Evaluation Plan | [click to access](https://docs.google.com/document/d/1YquG7pbgmXASSUQpl275z5HJm5drNmvJboA7d1QD3mE/edit?usp=sharing)** 

<br>

###  **Early Evaluation Findings** 

Prior to proceeding to the full evaluation plan, we decided to run a few participants through a very rudimentary, test version of our evaluation process. We gave participants a pre-survey, then had them run through up to three inquiries with *Solve For Why*, and finished the session with a post survey. We also collected chat logs and took notes while the participants interacted with *Solve For Why*. 

In the pre-survey, we attempted to capture participants' general math attitudes by asking if participants were a math person or not a math person. In the post-survey, we attempted to capture how users felt about using the chat bot, as well as if they would use the *Solve For Why* in their own time, or would have used *Solve For Why* while learning math. 

**Pre-Survey**  
Two out of the three participants selected that they were not math people and one selected that they were a math person (no one selected “other”). For two participants, the last formal math education setting they participated in was high school, and one participant stated that the last time was in community college. 

**Observations/Chat Logs**  
There were many UX/UI issues that participants experienced while using *Solve For Why*. While the intention of the observation was to surface impressions of the chat bot element, as we were aware of many of these issues, there were a few key takeaways that we did not expect. For instance, one participant found it very frustrating that there was not a simple way to type math symbols, such as an exponent. The chat crashed for two users, one after clicking on one of the resources in the resource section, and the other crashed randomly. The UI was also generally clunky. For example, the chat does not scroll down by itself, which was confusing for one user. Most of the issues that surfaced are easily addressed in future development. 

Users had unique inquiries for *Solve For Why*, including subjects like trigonometry, financial math, circles, and one novel question, “If everyone in Manhattan left their apartments at the same time and went into the streets would there be enough room in the streets?” Applying our internal evaluation rubric generally to the chat logs and observations:

| Category | Category description | Score (1-5) |
| :---- | :---- | :---- |
| Pedagogical Quality | Does the AI use the intended teaching strategies, like providing analogies, asking guiding questions, asking open inquiry questions or identifying core misconceptions? | 4 |
| Feedback & Assessment | Does the AI accurately identify errors in a student's work and provide clear, adaptive, and constructive feedback without employing direct instruction? Does the AI properly identify when the student is thinking like a mathematician and reward that with encouragement, or in some other way reinforce that behavior? | 4 |
| Handling Complex Queries | Can the AI manage multi-step inquiry or ambiguous student questions? | 5 |
| Affective Effects | Does the AI create a warm and inviting environment that is still demanding of the learner? | 4 |
| Error Handling | How does the AI respond when it doesn't know an answer or misunderstands the student? | 4 |
| Domain Knowledge | Is the AI accurate and knowledgeable about the subject it's supposed to be teaching? | 4 |
| Context-Awareness | Does the AI remember what was said earlier in the conversation and respond appropriately? | 5 |

<br> 

| Category | Qualitative notes |
| :---- | :---- |
| Pedagogical Quality | The bot did almost too good of a job sticking to the intended pedagogy. At times, participants were frustrated when the bot did not give them a direct answer. It was intellectually exhausting to constantly have to respond to open-ended, guided inquiry questions, however, participants also reported learning from that type of dialog specifically. It is potentially the case that the bot is over-tuned for not giving answers, as over the course of the sessions, participants moved from positive-activating emotions, to negative-activating, to negative-deactivating emotions. Participants   |
| Feedback & Assessment | The bot did a surprisingly good job of understanding when a participant understood what they were talking about or not before moving forward. Again, almost too good of a job, where it seemed like sometimes participants DID understand the math at hand, but were unable to communicate that to the bot. The bot followed its prompt well in this regard, not moving forward with the inquiry unless the participant demonstrated the conceptual knowledge it was looking for. The bot did encourage participants when they provided correct answers. The bot also swapped strategies/analogies often when participants expressed confusion.The bot also had a hard time when participants used vocabulary that they were not fully familiar with. For example, in an exchange about compound interest, the participant went down a line of inquiry with the bot in which the participant became lost in a slog of math jargon, even though they had used the terms themselves.  |
| Handling Complex Queries | The bot did an incredible job of handling complex and even ambiguous queries. It was able to keep track of multi-step problem solving, and made sure to bring the participant along for that journey.  |
| Affective Effects | The bot was certainly warm and demanding. The onslaught of questions back to the participant may have been too demanding, at least cognitively. The bot was certainly patient and encouraging.  |
| Error Handling | The bot did a decent job of asking clarifying questions when participant responses contained errors or were nebulous.  |
| Domain Knowledge | The bot was certainly accurate, but sometimes referenced or brought up knowledge that was not fully relevant.  |
| Context-Awareness | The bot appeared to have full knowledge of what had been talked about in the conversation.  |

<br>

**Post-survey and Other Reflections**  
In response to the question, “How did using the app make you feel? Was this experience different than using other chat bots,” participants answered:

* *Yeah it definitely was different, I definitely felt like I was being guided towards answers and thinking. And even when I fully didn't know or remember the chatbot did a great job of reframing questions to guide my learning. Definitely felt like it was scaffolding.*
   
* *It was very different from the usual chat bot experience because it didn't give me the answers outright... it was annoying at points (as someone who isn't a current math student) but I think it would definitely be helpful for a math student.*
  
* *positive start, terrible end* (this participant had the most issues with the fact that the bot wouldn’t use direct instruction)


These answers are generally encouraging. So far, it appears that the bot is doing what it is designed to do: teach conceptual knowledge. However, for teaching factual information, it struggles to provide learners with that knowledge directly. The participant who gave the first answer also stated that, “The chat bot did a really great job of determining what I did and didn't know, which is not very common.” Prior knowledge assessment is an explicit part of the bot’s pedagogical flow, and it was encouraging to see participants notice this aspect. 

When asked if they learned anything, participants stated that most of what they learned was review or recall. This is expected given the nature of their inquiries. One participant did state that they learned about financial math, but clarified that the bot would, “...not be useful for financial planning, but good for financial literacy.” Again, this confirms that the bot is teaching conceptual knowledge, rather than procedural knowledge. It was interesting to see this was evident to some of the participants. 

In response to the question, “Would you use this app on your own time,” two of the three participants responded, “No.” When asked to clarify, these participants stated that learning math was not currently relevant to their lives. The participant that said yes stated, “I'd use it to probably support math related questions in my own experimentation and exploration or if I have specific math needs in relation to my life like the finance example.” In response to the question, “Would you have used this app while you were learning mathematics in an educational setting (e.g. high school, home school, math camp, etc),” all of the participants said, “Yes.” When asked to clarify, one participant stated, “I think it would have been super helpful. Especially when it's one of those subjects where I understood it in class, but I never understood it at home. Math didn't feel as plug and play as it was advertised.” This participant was imagining *Solve For Why* as sort of a math version of Microsoft’s Clippy, which is not exactly the intended use-case, but a welcome one. 

<br>

**Summary | Initial Implications**  
Overall early testing has unearthed what we had expected, with tensions occurring when participants wanted direct instruction and positive feedback for the general pedagogical approach. We found it especially encouraging to hear that this chat bot experience differed from others, solidifying the need for an app like *Solve For Why*. This testing has brought up a user agency question; the current design puts the onus on bot to decide when the learner has reached a stopping point. None of the participants reached the end of a line of inquiry with *Solve For Why*, always exercising their agency to change the line of inquiry or stopping altogether. This is a question/tension to consider in future designs. 

##
---

### **Ethical Implications** 

We have worked to ensure our pedagogical design is research-based and have, via our guiding values, actually hoped to restore a measure of learner freedom and the rights of youth to direct their own learning, engage with mathematics on a recreational basis, and pursue mastery according to their own interest and desires. But we must remain vigilant for unexpected experiences and outcomes, we must assume they will occur, and we must do what is necessary to prepare for them. Here are some initial concerns we have surfaced, but we are eager to gather feedback from others to learn what we may be overlooking:

* Overall, we must…  
  * consider what guardrails should be in place for both our chatbot & user  
  * design an alert system for users to share concerns  
  * define response- and responsibility-protocols in case of a negative outcomes


* In order to interact effectively, our chatbot needs information about what our user already knows about specific math concepts being discussed or queried, and may benefit from knowing the general age range of our user. We have considered that any demographic information should be gathered *outside* the chat interface \- not so our chatbot won’t know (it will), but to avoid giving our user the impression that it’s normal and appropriate to share demographic information with the chatbot. We don’t otherwise plan to collect identifying information from users, but MIT’s *Guide to AI in Schools* asserts that chatbots can infer user identities from just a few identity markers shared through interactions, then share it without users’ knowledge or consent. So we must proceed under the assumption that our chatbot may infer the identity of our users. As our target users are minors, this is of significant concern. We need to conduct significant research into how to both prevent this from occurring and address it if it does.  
    
* Our chatbot interfaces with LLMs via API, so we must assume that it will eventually surface bias and other harmful material, assertions and assumptions.  
    
* We must take steps to ensure that users can’t use *Solve For WHY* other than as intended, as other activities accomplished with the application may harm individuals, communities, environments, etc.  
    
* Participants in our evaluation studies will be aware that we will review their entire interactions with *Solve For WHY* or feed this data into AI models for analysis. This may cause them to use the application differently than users “in the wild”. So we must be alert to novel instances occurring “in the wild” that we will not have anticipated based on our evaluation studies.

##
---

### **Future Work | Penny Hays** 

Evidence shows that self-identifying as “a math person” has strong positive impacts throughout the lifespan  (Schwartz et al, 2025). Yet \~30% of middle and high school students have never considered themselves a “math person” (Schwartz et al, 2025). Those who do developed this notion during elementary school (Schwartz et al, 2025), suggesting experiences that occur during those years \- whether positive or negative \- massively affect lifelong self-concept, math learning, and educational, career, and retaining pathways. The period from roughly age 5 to 11, then, seems to form a kind of crossroads \- some students develop self-identity as a “math person”, some develop math aversion or even anxiety.

Building an application for this age group would be a “heavier lift” than *Solve For WHY* because:

* Concerns re: interactions between a more juvenile age group and AI would be more numerous, more complex and potentially more consequential.    
* Users would have far less prior knowledge.  
* Scope would be more limited, but require more considered design. We couldn’t rely on the fascinating-ness of math itself to comprise the curriculum. At a minimum, we would need to design effective ways to support self-directed discovery learning of a smaller palette of foundational concepts, provide scaffolding, and offer more direct instruction. 

But it’s clear that application to support positive math experiences for this age group and encourage self-identification as a “math person” would be a valuable contribution, and is something I intend to pursue. 

##
---

### **Future Work | Bair**

See: [https://docs.google.com/document/d/1-\_hDjpwt1JsmCbq9HRlojZAytkda5wcn0fCmpE50LJY/edit?usp=sharing](https://docs.google.com/document/d/1-_hDjpwt1JsmCbq9HRlojZAytkda5wcn0fCmpE50LJY/edit?usp=sharing)

<br>

---

### **Appendix 1 | Second Prompt For Replit | [click to access](https://docs.google.com/document/d/1kyX-fDbY0PhODMbs2C2ac5NNxwxz9diF-KNcQnpTCH8/edit?usp=drive_link)** 

<br>

---

### **References** 

Boaler, J. (2015). Mathematical mindsets \[EPUB\]. Jossey Bass Wiley.

Boaler, J. (2024). Transforming Mathematics Education Through Mindset-Based Teaching. Stanford Graduate School of Education. [doi.org/10.33548/SCIENTIA1000](http://doi.org/10.33548/SCIENTIA1000)  
[https://www.youcubed.org/wp-content/uploads/2024/09/Scientia-article.pdf](https://www.youcubed.org/wp-content/uploads/2024/09/Scientia-article.pdf)

Deutsch, M. (2017, Jan 9). *M2M Day 69: Decoding Rubik’s Cube Algorithms*. Medium. [https://medium.com/@maxdeutsch/m2m-day-69-decoding-rubiks-cube-algorithms-6ea7e7704ec9](https://medium.com/@maxdeutsch/m2m-day-69-decoding-rubiks-cube-algorithms-6ea7e7704ec9)

Garner, L. E., Steinberg, E. J., & McKay, D. (2021). Exposure therapy. In A. Wenzel (Ed.), Handbook of cognitive behavioral therapy: Overview and approaches (pp. 275–312). American Psychological Association. [https://doi.org/10.1037/0000218-010](https://psycnet.apa.org/doi/10.1037/0000218-010)

Gray, K. (2013, April 18). Embracing Disequilibrium. Math Minds. \[blog\]. [https://kgmathminds.com/2013/04/18/embracing-disequilibrium/\#:\~:text=Disequilibrium%20in%20the%20way%20students,to%20see%20teachers%20teaching%20students](https://kgmathminds.com/2013/04/18/embracing-disequilibrium/#:~:text=Disequilibrium%20in%20the%20way%20students,to%20see%20teachers%20teaching%20students).

Jimenez, L. & Modaffari, J. (2021, Sep 16). Future of Testing in Education: Effective and Equitable Assessment Systems. Center for American Progress. [https://www.americanprogress.org/article/future-testing-education-effective-equitable-assessment-systems/](https://www.americanprogress.org/article/future-testing-education-effective-equitable-assessment-systems/)

LeBlanc, G. (2025, June 11). 551\. The Math Mindset and How to be Math-ish feat. Jo Boaler. \[YouTube Video\]. unSILOed Podcast. [https://www.youtube.com/watch?v=kq4YXpWUTRo](https://www.youtube.com/watch?v=kq4YXpWUTRo)

Leyva, E., Walkington, C., Perera, H., Bernacki, M. (2022). Making Mathematics Relevant: An Examination of Student Interest in Mathematics, Interest in STEM Careers, and Perceived Relevance. Int. J. Res. Undergrad. Math. Ed. 2022;8(3):612–41. doi: 10.1007/s40753-021-00159-4. Epub 2022 Feb 2\. PMCID: PMC8807670.

Maltese A.V. & Tai, R.H. (2017.) Pipeline persistence: Examining the association of educational experiences with earned degrees in STEM among US students. Science Education. 2011;95(5):877–907. doi: 10.1002/sce.20441. 

McMurrer, J. (2007). Choices, Changes, and Challenges: Curriculum and Instruction in the NCLB Era. Washington: Center on Education Policy. [https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=593580376CAA72933F4BB739B7C12DBD?doi=10.1.1.643.5250\&rep=rep1\&type=pdf](https://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=593580376CAA72933F4BB739B7C12DBD?doi=10.1.1.643.5250&rep=rep1&type=pdf)

NAEP. (2024). NAEP Mathematics Assessment, aka “Nation’s Report Card”, a Congressionally Mandated National Assessment Program. Institute of Education Sciences. [https://www.nationsreportcard.gov/reports/mathematics/2024/g4\_8/?grade=8](https://www.nationsreportcard.gov/reports/mathematics/2024/g4_8/?grade=8)

Phelps, R. P. (2016). Teaching to the Test: A Very Large Red Herring. *Nonpartisan Education Review* 12 (1). [https://www.nonpartisaneducation.org/Review/Essays/v12n1.htm.](https://www.nonpartisaneducation.org/Review/Essays/v12n1.htm)

**Recreational mathematics. (last edited 2025, August 18). In *Wikipedia.* [https://en.wikipedia.org/wiki/Recreational\_mathematics](https://en.wikipedia.org/wiki/Recreational_mathematics)** 

**Internal citation within Wikipedia:** Kulkarni, D. [Enjoying Math: Learning Problem Solving With KenKen Puzzles](http://www.matholympiad.info/Documents/TeachingWithKenKen.pdf) [Archived](https://web.archive.org/web/20130801080339/http://www.matholympiad.info/Documents/TeachingWithKenKen.pdf) 2013-08-01 at the [Wayback Machine](https://en.wikipedia.org/wiki/Wayback_Machine), a textbook for teaching with KenKen Puzzles.

**Internal citation within Wikipedia:** 

[Special Interest Groups of the MAA](https://www.maa.org/community/sigmaas) [Archived](https://web.archive.org/web/20130718123507/https://www.maa.org/community/sigmaas) 2013-07-18 at the [Wayback Machine](https://en.wikipedia.org/wiki/Wayback_Machine) Mathematical Association of America (MAA)

Ryan, R. M., & Deci, E. L. (2017). [Self-Determination Theory: Basic Psychological Needs in Motivation, Development, and Wellness](https://www.google.com/search?sca_esv=bffb88f62265f716&rlz=1C5CHFA_enUS534US534&cs=0&q=Self-Determination+Theory%3A+Basic+Psychological+Needs+in+Motivation%2C+Development%2C+and+Wellness&sa=X&ved=2ahUKEwjvkNb48IuQAxW_K1kFHScUMlMQxccNegQIGxAB&mstk=AUtExfD7MahJTtxx3rxkyS7Bcp55dOUKtiMXfItkXFU_dwXOVizQPEy8X1x3mLFZyb2cQGJD6up6JnrcpEmuXHn-JCMZJbwfPYJykbf1bpjOSe_Vr4jDPnp5gQ9XMhI-N5jS2e702FHzV5dFun5ON9C3ev2pvmsoZCy08L1W_kUZ04VFfTMVggrN1P_NUlKOFz5AaJ1w&csui=3). New York: Guilford Press. [SCIRP Open Access](https://www.scirp.org/reference/referencespapers?referenceid=2531959) 

Samuelsson, J. (2021). Developing students’ relationships with mathematics. *Educational Action Research*, *31*(2), 180–194. [https://doi.org/10.1080/09650792.2021.1899012](https://doi.org/10.1080/09650792.2021.1899012)

Schwartz, H., Bozick, R., Diliberti, M. K., Ohls, S. (2025, June 17). Students Lose Interest in Math: Findings from the American Youth Panel. Rand Corporation. Funded by the Gates Foundation. [https://www.rand.org/pubs/research\_reports/RRA3988-1.html](https://www.rand.org/pubs/research_reports/RRA3988-1.html)

Schwartz, S., (2024, November 25). *Which Nation’s Students Are Defying the Math Anxiety Trend?*. Education Week. [https://www.edweek.org/teaching-learning/which-nations-students-are-defying-the-math-anxiety-trend/2024/11\#:\~:text=By%20Sarah%20Schwartz%20%E2%80%94%20November%2025,Canada%20who%20studies%20mathematical%20thinking.](https://www.edweek.org/teaching-learning/which-nations-students-are-defying-the-math-anxiety-trend/2024/11#:~:text=By%20Sarah%20Schwartz%20%E2%80%94%20November%2025,Canada%20who%20studies%20mathematical%20thinking)

Schwartz, S., (2024, December 4). *‘Sharp, Steep Declines': U.S. Students Are Falling Behind in Math and Science*. Education Week. [https://www.edweek.org/leadership/sharp-steep-declines-u-s-students-are-falling-behind-in-math-and-science/2024/12](https://www.edweek.org/leadership/sharp-steep-declines-u-s-students-are-falling-behind-in-math-and-science/2024/12)

Singh, S. (2025, November 6). The Joy Of Teaching Mathematics Without A Curriculum. Medium. [https://sunilsingh-42118.medium.com/the-joy-of-teaching-mathematics-without-a-curriculum-69c7ea589028](https://sunilsingh-42118.medium.com/the-joy-of-teaching-mathematics-without-a-curriculum-69c7ea589028)

Smith, J., Fotou, N., & Sharpe, R. (2025). Changes in mathematics anxiety and mathematics confidence. *International Journal of Mathematical Education in Science and Technology*, 1–19. [https://doi.org/10.1080/0020739X.2025.2475928](https://doi.org/10.1080/0020739X.2025.2475928)  
[https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928\#d1e127](https://www.tandfonline.com/doi/full/10.1080/0020739X.2025.2475928#d1e127)

Smith, J. M., Dukes, J., Sheldon, J., Nnamani, M. N., Esteves, N., & Reich, J. (2025). A Guide to AI in Schools: Perspectives for the Perplexed. MIT Teaching Systems Lab. [https://tsl.mit.edu/wp-content/uploads/2025/08/GuideToAIInSchools.pdf](https://tsl.mit.edu/wp-content/uploads/2025/08/GuideToAIInSchools.pdf)

Tam, F. & Pawar, S. (2020). Emerging Design Factors in Game-Based Learning: Incentives, Social Presence, and  
Identity Design. In J.L. Plass, R.E. Mayer, and B.D. Homer, (Eds.), [Handbook of Game-based Learning](https://mitpress.mit.edu/9780262043380/handbook-of-game-based-learning/), pp. 153 \- 176\.  
Cambridge: MIT Press.

Weir, K. (2023, October 1). How to solve for math anxiety? Studying the causes, consequences, and prevention methods needed. Monitor on Psychology, Vol. 54, No. 7\. American Psychological Association. [https://www.apa.org/monitor/2023/10/preventing-math-anxiety](https://www.apa.org/monitor/2023/10/preventing-math-anxiety)

Winne, P. H. & Azevedo, R. (2014). Metacognition. In R. K. Sawyer (Ed.) The Cambridge handbook of the learning sciences (2nd ed., pp. 63–87). Cambridge University Press. [https://doi.org/10.1017/CBO9781139519526.006](https://doi.org/10.1017/CBO9781139519526.006)

Wise, A., Reza, S., & Han, R. (2020). Becoming a Dentist: Tracing Professional Identity Development Through Mixed Methods Data Mining of Student Reflections. In M. Gresalfi (Ed.), Proceedings of the Fourteenth International Conference of the Learning Sciences (pp. 1031-1032). International Society of the Learning Sciences. [https://repository.isls.org/bitstream/1/6650/1/294-301.pdf](https://repository.isls.org/bitstream/1/6650/1/294-301.pdf)
