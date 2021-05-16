# Concept for Learner focused Code Evaluation
To identify the most significant factors influencing a learner's success, this chapter presents the results of a user study. Based on these insights and a literature review, a didactic and pedagogical concept for the E-Assessment Use Case - as described in chapter \*@sec:environment - is developed.

## User Study
Exploratory qualitative interviews are the standard in the development of new software solutions. As this master thesis aims to introduce a novel user-centric approach, the user's needs have to be investigated. The qualitative interviews follow the best practices, as described by @kuniavsky2003observing.
A total of eleven interviews with a duration of 15-45 minutes were conducted virtually, asking participants of the LAMA course about their impressions on MOOCs, E-Assessment, Learning Programming, and the LAMA course in general. The interview questions and guide can be found in \*@sec:interview-guide.

\todo{Do I need to transcribe the interviews?}

### Overall
The overall reception of the course was exceptional. Students liked the mix of theoretical inputs, independent work, and the final project that reproduces real-world use cases. 

Most still apply the topics introduced in this course today and believe that their theoretical knowledge and practical action ability have been improved. All participants agreed that they feel confident or somewhat confident to work on a new problem with machine learning
About two-thirds applied or are applying machine learning in a new context like an internship, thesis, university, or private project.  

### Feedback
The main pain point of the LAMA was the missing feedback for submissions. All participants wished for more transparency in the grading. Interviewees agreed that getting prompt results for the weekly assignments would have been beneficial for their learning outcomes. Students were ambiguous about the type of feedback that would increase their learning effect most. About two-thirds said they liked a form of grading, while the rest preferred to check their solutions on their own with a sample solution. 
In the grading peer group, there were multiple references to the type of grading. Some whished to in-depth written feedback by experts. Others favored highlighting the differences between their solution and the sample solution. 

### Experience with E-Assessment
About half of the participants had previously learned a programming language or participating in a MOOC course. The reception of this was mixed: Some described their problems with finishing a course, or to find a course that fits their level and speed. The E-Assessment component of most courses was described to be mostly simple static checking of required functionality, working only on code snippets. Students agreed that this iterative approach to problem-solving helped their understanding. 
One participant highlighted how inline feedback to common errors and tips helped him to improve his solution. 

## Components
The components of E-Assessment Systems are systematically reviewed by @striewe2019components.

| Component (@striewe2019components)      | Description                                                               | Corresponding Component |
| --------------------------------------- | ------------------------------------------------------------------------- | ----------------------- |
| Student, Teacher Frontend               | User-facing Interface                                                     | ANNIE                   |
| Pedagogical module, evaluator component | Analyzes submissions and returns feedback                                 | CURT, STEVE             |
| Peer Review System                      | Users can add peer review and get matched to users with similar interests | PETER                   |
Table: Overview of E-Assessment Components. {#tbl:components}


The design of this E-Assessment tool follows an asynchronous pull principle. @striewe2019components
A Queue based on the Python Package *Celery*\footnote{Celery is an open-source python package widely used.} is used to keep user inputs, the evaluator component pulls the next task on demand 
\todowrite{Description of the Components - might move to implementation later}

### Code Understanding for Process Classification (CURT)
Code Understanding for Review and Taxonomy (CURT) is an NLP-based component for programming code analysis. The goal is to provide human-readable feedback and classify parts of a program to match it to the steps of a given ML-Process description (for example CRISP-DM or QUA\textsuperscript{3}RK).
An in-depth description of this approach, including data-set generation, implementation, and evaluation can be found in \*@sec:Training-Neuronal-Networks-for-Code-Assessment. 
