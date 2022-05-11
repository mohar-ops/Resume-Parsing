# Resume-Parsing
Latex file, PDF file of the resumes uploaded as resume4.tex and resume4.pdf, respectively
JD.docx is a sample JD taken from the reference https://www.internships.com/employer/resources/internships/computer 

This project takes a resume (in tex and pdf formats).

Below are the code files that we wil be using for described functionalities:
1. SanityChecks(.ipynb): To check the number of pages in the resume [resume4.pdf file used]
                 To extract the section names of the resume [resume4.tex file used] 
 The purpose of this is to give feedback to the students, based on two situations; first one is: if the resume is longer than 2 pages, feedback can be given to make it shorter; second one is: if among the resume sections an important section is missed (Eg. Education or Skills section), the students can be notified in the feedback

2. Structure Measurement(.ipynb): To check whether the sections are bulleted since from research, a bulleted resume is preferred compared to a one with lots of paragraphs. 
                          To classify the links as professional or unprofessional, valid or invalid and checking the validility of email addresses and email ids. 
                          In case of unprofessional or invalid link and email ids, students can get a feedback to include necessary changes.
              
3. Content Measurement(.ipynb): To arrange the sections and its contents as a dictionary key-value pair. A sample JD.docx is used for cosine similarity comparison of each skill section with the given JD and the match % is shown to the student. 
Grammatical mistake as well as formatting error detection and correction along with corrected text will be displayed, section-wise. Extra spaces are also corrected. For a section needing no corrections a null list is returned. 
Finally, Job roles suited for the candidate are displayed according to the skillset (based on static nlp based rules for 4 broad job roles). 
