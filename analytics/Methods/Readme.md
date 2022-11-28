
## Method
A procedure or process for attaining an object

## Research methodology
Is the justification (or explanation) for using a particular research method.

## Research method
Is the strategy employed in the collection of data or evidence for analysis to uncover new information or arrive at a better understanding of a particular topic.

## Type of methods:
### 1. Qualitative data analysis (aims to understand the problems being investigated in greater detail, and is often quite subjective). 
Is often referred to as "storytelling" because it includes `extensive aditional information` beyond a simple response to the hypothesis question. <br/>
Collecting Qualitative data can help you understand more facts and circunstances and `how they impact` the problem you are trying to solve.
### 2. Quantitative data analysis (relies on numbers, objective and repeatable data, and avoids subjectivity) <br/>

Process model that serves as the base for a data science process.  Shouldn't be considered  BETTER or WORSE than QUALITATIVE data. <br/>
It has six sequential phases: <br/>

2.1. Business understanding – What does the business need? <br/>
- Determine business objectives: You should first “thoroughly understand, from a business perspective, what the customer really wants to accomplish.” (CRISP-DM Guide) and then define business success criteria.
- Assess situation: Determine resources availability, project requirements, assess risks and contingencies, and conduct a cost-benefit analysis.
- Determine data mining goals: In addition to defining the business objectives, you should also define what success looks like from a technical data mining perspective.
- Produce project plan: Select technologies and tools and define detailed plans for each project phase. <br/>

2.2. Data understanding – What data do we have / need? Is it clean? <br/>
- Collect initial data: Acquire the necessary data and (if necessary) load it into your analysis tool.
- Describe data: Examine the data and document its surface properties like data format, number of records, or field identities.
- Explore data: Dig deeper into the data. Query it, visualize it, and identify relationships among the data.
- Verify data quality: How clean/dirty is the data? Document any quality issues. <br/>

2.3. Data preparation – How do we organize the data for modeling? <br/>
- Select data: Determine which data sets will be used and document reasons for inclusion/exclusion.
- Clean data: Often this is the lengthiest task. Without it, you’ll likely fall victim to garbage-in, garbage-out. A common practice during this task is to correct, impute, or remove erroneous values.
- Construct data: Derive new attributes that will be helpful. For example, derive someone’s body mass index from height and weight fields.
- Integrate data: Create new data sets by combining data from multiple sources.
- Format data: Re-format data as necessary. For example, you might convert string values that store numbers to numeric values so that you can perform mathematical operations. <br/>

2.4. Modeling – What modeling techniques should we apply? <br/>
- Select modeling techniques: Determine which algorithms to try (e.g. regression, neural net).
- Generate test design: Pending your modeling approach, you might need to split the data into training, test, and validation sets.
- Build model: As glamorous as this might sound, this might just be executing a few lines of code like “reg = LinearRegression().fit(X, y)”.
- Assess model: Generally, multiple models are competing against each other, and the data scientist needs to interpret the model results based on domain knowledge, the pre-defined success criteria, and the test design. <br/>

2.5. Evaluation – Which model best meets the business objectives? <br/>
- Evaluate results: Do the models meet the business success criteria? Which one(s) should we approve for the business?
- Review process: Review the work accomplished. Was anything overlooked? Were all steps properly executed? Summarize findings and correct anything if needed.
- Determine next steps: Based on the previous three tasks, determine whether to proceed to deployment, iterate further, or initiate new projects. <br/>

2.6. Deployment – How do stakeholders access the results? <br/>
- Plan deployment: Develop and document a plan for deploying the model.
- Plan monitoring and maintenance: Develop a thorough monitoring and maintenance plan to avoid issues during the operational phase (or post-project phase) of a model.
- Produce final report: The project team documents a summary of the project which might include a final presentation of data mining results.
- Review project: Conduct a project retrospective about what went well, what could have been better, and how to improve in the future.


