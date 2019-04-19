---
title: "Content"
date: 2018-08-12T14:37:23-04:00
draft: false

type: kira_talent

company_name: Kira Talent
# url: "https://www.kiratalent.com/"
logo: kira-logo.jpg
introduction: My name is Jordan Chalupka, and at the time of writing this, I am completing my Undergraduate degree in  Software Engineering at the University
                      of Guelph. For the past 4 months, I have been working at a Toronto based ed-tech company named Kira Talent. The purpose of this blog
                      is to document my time at Kira Talent; covering topics such as my goals, projects I was involved with,
                      and skills that I gained through this work experience.
about: For my third work term, I had the pleasure to work for [Kira Talent](https://www.kiratalent.com/).  Kira Talent operates a cloud-based holistic admissions assessment platform designed for use by academic admissions departments, to assess and enroll students using timed video and written questions.

job_description: My job as a Software Developer involved creating small enhancements, writing tests, and fixing bugs on our main product, Kira Assess.  During my work-term, I was part of two teams, the Tactical team, and the Platform team.  The Tactical team was responsible for triaging bugs and developing small enhancements for the product.  The Platform team was responsible for everything infrastructure related and my involvement with this team was mainly focused on a proof of concept infrastructure change that I developed (more on that later).
# talk at some point about the meetings that I had and how that was different than my previous work term. -->

projects:
  description: An overview of some of the different projects that I worked on at Kira Talent.
  project_list:
    - name: Video Conversion Worker Proof of Concept.
      description: 
        - <div><img class="center-block img-responsive" src="/img/elastic_transcoder_infrastructure.png" style="width:50%"/></div>

        - One of the projects that I worked on at Kira Talent was a proof of concept for a video conversion service which utilized managed services.  In this project, I designed, planned and implemented a proof of concept service which makes use of AWS Elastic Transcoder to replace the existing video conversion workers (VCWs).  By using AWS Elastic Transcoder I was able to create a service which is scalable, and easier to maintain.
        - <div><img class="center-block img-responsive" src="/img/elastic_transcoder_presentation.png" style="width:50%"/></div>

        - While creating this service, I also created docs and an infrastructure diagram for it.  to educate everyone on how the service works, as well as pass on all of the knowledge that I gained while working on the proof of concept, I made a presentation to all of the senior developers on the engineering team.
          # include some photos from my presentation (atleast mention that I made a presentation)
    - name: Spelling and Grammar Checker Microservice
      description:
        - In addition to video responses, Kira Talent also offers the option to use written responses as part of an applicant's assessment.  To help assess written responses, there is a spelling and grammar checker which assesses written responses based on their spelling and grammar correctness.  However, the previous implementation of the spelling and grammar checker was not very accurate, and often missed errors and provided false positives when checking for spelling and grammar.  In the improved spelling and grammar checker which I built, I was able to make use of the open source project LanguageTool to improve the accuracy of the spelling and grammar checker while keeping costs associated with the spelling and grammar checker low.  Alongside creating this service, I also wrote the documentation and created an infrastructure diagram for this service. 
        - <div><img class="center-block img-responsive" src="/img/spelling_and_grammar_highlighting.png" style="width:50%"/></div>
        - The spelling and grammar checker also provides reasons for why it highlighted text.        
        - <div><img class="center-block img-responsive" src="/img/spelling_and_grammar_analysis.png" style="width:50%"/></div>
    - name: Kira Assess
      description: 
        - The largest project which I worked on this semester was Kira Assess.  This is Kira Talent's main product, and as such, I spent the majority of my time working on it.  The work that I did on Kira Assess ranged across our tech stack, from front-end cosmetic changes to backend data manipulation to ops work such as managing resources used when deploying the application to different environments.  While working on this project gained skills in python development using the Django framework, front-end development skills using Flight.js, Sass, and a bit of Vue.js.
        - <div><img class="center-block img-responsive" src="/img/kira_assess_ratings.png" style="width:50%"/></div>
# This should be broken down into paragraphs ...
learning_goals_and_reflections:
  - My first goal was to create a proof of concept for a Video Conversion Worker replacement using Amazon Web Services.  This larger goal encompassed a lot of smaller goals, such as designing my own project and learning more about how to utilize managed services on AWS.  Upon completion of this goal, I am very happy with the proof of concept that I created, and I feel that it will provide a very solid foundation for a future re-implementation of our Video Conversion Workers.
  - My second goal was to create or substantially improve a piece of documentation.  Throughout my work term I ended up writing several different pieces of documentation, such as a document on Testing in Python, documentation for the Spelling and Grammar microservice that I wrote, documentation for the Video Conversion Worker service that I wrote, as well as instructions for how to migrate client's data to a different AWS region.
  - Another goal that I set for myself this term was to write 10 unit tests and deploy them to production.  Throughout my time at Kira, I learned a lot about how to write good unit tests through mocking (I even wrote a document about it for future hires to reference).
  - My final goal this semester was to create a spelling and grammar checker microservice and deploy it to production.  While completing this goal I gained several new technical skills, such as modern Java best practices, and how to design serverless architecture.  The end product for this goal also ended up being a big success and is currently being used in production. 
lessons_learned:
  description: During my time at Kira Talent, I learned a lot of skills both technical and non-technical.
  lessons_list:
    - During this work term, I discovered Terraform, which has now become one of my favourite technologies.  Terraform allows users to write infrastructure as code, which apart from just being really cool adds a lot of benefits.  One of the benefits I found through using Terraform is being able to check infrastructure changes into version control software (Git) and perform pull requests on changes, allowing infrastructure changes to be reviewed the same way as code changes are.  Another benefit terraform provides is being able to "plan" changes before execution, to see what changes will occur when you execute.  I found that this gave everyone on the team a lot more confidence when deploying changes since we could see exactly what terraform was going to do before executing the changes.
    - Another lesson that I learned this semester is how to use feature flags to deploy new features with confidence.  Before working at Kira Talent I had never used feature flags in my code.  Now, after seeing the benefits that they bring, such as being able to roll back changes without deploying code, or being able to restrict new features to certain clients, I am confident that I will continue to use feature flags when releasing new features in my code going forward.
    - Although there are many more, for the purposes of this work term report the final lesson that I learned this semester was to validate approaches early.  As one of my co-workers said, "One of the best ways to learn is to say stupid things and have them contradicted or corrected".  Despite how much everyone wants to believe that their idea is the best, often the best ideas come through collaboration, and by validating ideas with someone else before beginning to work on a problem it can save a lot of time.
  
conclusion:
  - I would consider my work term at Kira Talent a huge success. I learned a lot, gained valuable experiences, got to work with
                      a great team, and had some fun while doing it. I would like to thank Robyn for the great management and support throughout the term, as well as the rest of the engineering team for their help and encouragement throughout the term.  And of course, a big thank you to everyone at Kira Talent for making such a great work environment.  Best of luck to Kira Talent with your awesome new office space and future employees! 
---
