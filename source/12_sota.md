## Environment 

In the AMALEA project, the Institut für Technik der Informations­verarbeitung (ITIV) is working on an online course based on a practical course. Project partners are the *Zentrum für Mediales Lernen* (ZML), which is responsible for the video recordings, graphics, and didactical basics and the AI Campus of the Hasso Plattner Institute Potsdam (HPI), providing the setting and platform of the Massive Open Online Course. 

### LAMA

The practical course at KIT called *Labor für angewandte Machine Learning Algorithmen* (Laboratory for Applied Machine Learning Algorithms, LAMA) was established in 2019 and targets Undergrad Students.
The learning objectives of this 6 ECTS course are:\footnote{Based on the module objectives of the institute} 

* The students are able to analyze current and complex problems of a modern electrical and information technology engineer and assess the necessity for machine learning methods.
* Students can name various modern machine learning methods and explain how they work.
* The students are able to select these concerning their requirements (including training time, data availability,
efficiency, and performance). They can implement them successfully with current programming languages and typical software frameworks.
* The students are able to select and implement suitable implementation alternatives (HW/SW codesign) in the entire process.
* The students are able to systematically develop a suitable practical concept for a given problem based on machine learning methods. Alternatively, students are able to evaluate, compare and assess given concepts.
* The students master the analysis and solution of these problems in a team. 

Assessment of the protocols, continuous assessment of the teamwork, and the query on the contents of the laboratory form the final grade of this course.
\todowrite{Einordnung LAMA in MOOC Kurs}

### E-Assessment
E-Assessment is the umbrella term for all systems that check digital students submissions in a somewhat automatic fashion. 
These systems are used to reduce the possibilty of errors by lecturers, provided almost instant feedback to students and reduce workload of lecturers. 

The tools can be used both for formative assessment to check the learning progress of a student during the course time and for summative assessment to determine the learning outcomes. \todowrite{Quelle: Harlen and James 1997)}

Especially MOOC-Courses, where hundreds of student submit each assignment require tools to automatically assess assignments. These courses are often designed around these tools, as requirements for the certification of students are directly determined by these tools. 

# State of the Art of Code Evaluation

Felizardo et. al. group different publications on code assesment by categories. \todo{Quelle}


## Static Code Assessment
Tools use Static Code Assessment to assess code styling, determine design requirements or calculate metrics like complexity and readability. 

## Dynamic Code Assessment
Dynamic Code Assessments is characterized by checking code at runtime, meaning the assessment tool checks the functionality and efficiency by running a code example. Dynamic code assessment can be risky, as Bugs or malicious code can cause damage to the system. \cite{ala2005survey} Therefore, code is often run in virtualized containers like Docker to reduce the risk surface.
\todowrite{More on Docker and Co?, Based on the actual implementation.}

@galassi2020improved first proposed a hybrid system that uses both static source code analysis to check the correctness and a supervised classifier to provide feedback to open-ended questions. This approach is based on the distance between a sample solution and the learners' solution and can therefore not work in the open-ended task environment this work aims to assess. 
Dynamic Code Assessment is defined as the automatic assessment of code based on 



# Natural Language Understanding

@elnaggar2021codetrans introduced the T5 Transformer structure to Programming Code. 



