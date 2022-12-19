# How to Write Good Code Documentation for Data Scientists
(A crash course on the best practices you need to ensure that everyone understands the code you write)

#### Write step-by-step notes that describe how your code works and the steps you need to make the code work
- The key here is to write down absolutely everything that comes to mind when writing your code, especially things that you may deem inconsequential to mention though could end up being game-changers in its later usages. 
- This includes items such as describing what each variable represents, what each function does, and the results the code should yield. 
- You will also want to include notes on why the code has to be written a certain way and in what order the functions are used and called.

#### Assume that the person reading your code knows nothing
- One of the best things you can do when writing your code documentation is to write it as if the next person has no clue about anything to do with your code.
- This information could reside within the code (again, most helpful if coherent) or could reside in an external document.
- Short-form notes should be included within the code, whereas long-form explanations or descriptions are better left in an external document.

#### Use coding conventions and best practices
- This not only helps those after you to understand the code, but it also makes the code as production-ready as possible if and when that time comes.
- The key ideas to focus on when it comes to coding conventions and best practices are to:
1.	Use descriptive variable names.
2.	Use functions.
3.	Use comments (as discussed above).
4.	Use a consistent coding style.
5.	Use the syntax conventions of the language you use.
6.	Use libraries.
7.	Keep your code DRY.

#### Provide your contact information
- Providing your contact information at the end of your code or documentation is a simple, yet effective way of ensuring that any questions or issues are directed to you, which can help save time, money, and frustration.

#### Use flow-charts
- Viewing a process graphically can be an extremely effective way of understanding how it works
- These flow charts can be included in the external documentation for your code and should provide step-by-step instructions on how a function works, what it should return, and what should occur if something goes wrong or if a condition isn’t satisfied.

#### Practice describing how your code works so that a 5-year-old could understand it
- By reviewing your code documentation a few times before making it available, you ensure that you can explain your code as simply as possible through your literature and that you can explain it in more detail if questions ever arise.

------------------
# Good Data Scientists Write Good Code
(Tips on how to be nice to yourself and your colleagues when developing code for data products)

#### What makes a “good code” exactly?
<p align="center">
  <img src="https://github.com/akimwong/akimwong/blob/main/articles/summaries/coding/coding1.jpg" width="450" height="450">
</p>

Best practices and principles to be particularly relevant and useful:
-	it takes minimal time and cost for new team members to join the project;
-	the code is written in a modular way and is version-controlled and unit-tested;
-	the application is fully configurable and contains no hard-coded values that control its execution;
-	the application is portable between execution environments;
-	the application is scalable without changing the tooling, architecture or development practices;
-	no code gets deployed in production without a peer review;
-	there is a monitoring infrastructure that allows one to track and understand how the application behaves in production.

#### Writing a perfect piece of code in one go is almost impossible, and that’s OK
- Having clearly formulated requirements in Data Science projects is uncommon.
- Given the highly risky nature of Data Science projects, especially in their early stages, it doesn’t make much sense to write production-grade code from Day 1.
- Instead, it’s useful to approach code development more pragmatically, similar to how it’s done in software development projects.
- One approach to software development that I find particularly relevant suggests thinking about the evolution of the application codebase in terms of the following stages: “make it work, make it right, make it fast”. 

## 1. Make it work
('prototype': early sample, model, or release of a product built to `test a concept` or process)
- At the beginning of a project it is important to start small and build a prototype first. 
- Develop a prototype solution for the business problem at hand in order to analyse that solution, learn from it, and decide if further development and deployment are justified. 
- For instance, this could involve quickly building a predictive model on a limited sample of data using default hyperparameters. 
- The code at this stage doesn’t have to be “pretty”.
- We build prototypes to analyse and learn from them as cheap as possible so that we can quickly decide whether further development and deployment are justified ROI-wise. 

#### A prototype code is a throw-away code
- The code of a prototype solution needs to be treated as disposable code. 
- As a Data Scientist leading the project or as a Project Manager, you must make this very clear to your stakeholders.

#### What’s OK to do when building a prototype as code
Since the prototype code is disposable, it:
- doesn’t have to be “pretty” or optimised for computational speed as the speed of development is way more important at this stage;
- doesn’t have to be documented to the same level as a production-grade code (however, there should be enough comments and/or Markdown-based notes to understand what the code does and to ensure its reproducibility);
-	doesn’t have to be version-controlled (although setting up version control at the beginning of any project is always a good idea);
-	it’s OK to have hard-coded values (but not the sensitive ones, such as passwords, API keys, etc.);
-	can be written and stored in a Jupyter Notebook or similar media (e.g., R Markdown Notebook) instead of being organised into a library of functions and/or a collection of production-ready scripts.

#### What’s not OK to do when building a prototype as code
- using cryptic or abbreviated names for variables and functions;
- mixing code styles (e.g., randomly using camelCase and snake_case to name variables and functions in languages like Python or R, or using uppercased and lowercased command names in SQL);
-	not using comments in the code at all;
-	having sensitive values (passwords, API keys, etc.) exposed in-code;
-	not storing notebooks or scripts with the prototype code for future reference.

## 2. Making it right



