#The Art of Machine Learning Experimentation
(5 simple strategies to help you get the most out of your ML experiments)

- I’m talking about what happens before and after the experiment is done. 
- How can you get the most out of your ML experiments? Here are 5 simple strategies that you can adopt.

## 1. Know when to experiment
- The possibilities for spending your time are endless.
- How should you decide what to experiment on, given your limited time budget? 

### 1.1. Prioritize experiments with the highest expected gain. 
- Take your time to fully understand the existing model and find out where the largest gaps are: that’s where you want to focus your efforts. 
- For example, if a model uses just a handful of features, the best experiments are probably around feature discovery. 
- If a model is a simple logistic regression model, work on model architecture may be more promising.

### 1.2. Don’t experiment to learn things that are already known. 
- Before even thinking about launching any experiments, do your research. 
- If there’s a broad consensus in the literature about a question you’re trying to answer, then you probably don’t need to design an experiment around it. 
- Trust the consensus, unless you have strong reasons not to.

### 1.3. Define clear success criteria prior to the experiment. 
- `If you don’t have clear success criteria, you’ll never know when you’re done`.  It’s as simple as that. 
- I’ve seen too many `models that were never deployed` because `the launch criteria changed after the experiments were run.` 
- Avoid this pitfall by `defining and communicating clear criteria prior to running any experiments`.

## 2. Always start with a hypothesis
- `We hypothesize first, and then run an experiment that will either confirm it or rule it out`. 
- Either way, we have gained knowledge. That’s how science works.
- A scientific hypothesis has to be a statement, usually with the word “because” in it. `It can’t be a question. “Which model is better?” Is not an hypothesis`.
- The scientific method — formulating a hypothesis prior to the experiment — is the best guard against fluke discoveries.

## 3. Create tight feedback loops
- Changing one thing in your ML pipeline should be as simple as changing one line of code and executing a submit script in a terminal. 
- If it’s much more complicated than that, it’s a good idea to first tighten your feedback loop. 
- `A tight feedback loop simply means that you can test ideas quickly, without any complicated stunts`.
- Here are some ideas on how to do that:

### 3.1. Automate naming. 
- Time spent thinking about how to name something (a model, a trial, a dataset, an experiment, etc) is time that’s not spent actually experimenting. 
- Instead of trying to come up with clever and insightful names such as “BERT_lr0p05_batchsize64_morefeatures_bugfix_v2”, automate naming with libraries such as coolname, and instead simply dump the parameters into logfiles.

### 3.2. Log generously. 
- When logging experimental parameters, err on the side of logging more than you need. 
- Logging is cheap, but re-running experiments because you don’t remember which knobs you’ve changed is expensive.

### 3.3. Avoid notebooks. 
- `Notebooks are hard to version, hard to share, and mix code with logs, making you scroll up and down each time you want to change something`. 
- They do have their use-cases, for example in exploratory data analysis and visualization, but in ML experimentation, scripts are usually better: they can be versioned, shared, and create a clear boundary between code and logs, i.e. inputs and outputs.

### 3.4. Start small and fail fast. 
- `It’s a good idea run an experiment first on a small, sub-sampled, dataset`. 
- `This allows you to get quick feedback without losing too much time, and “fail fast”: if the idea isn’t working, you’ll want to know as soon as possible`.

### 3.5. Change one thing at a time. 
- If you change multiple things at the same time, you simply can’t know which of these things caused the change in model performance that you’re seeing. 
- Make your life easier by changing just one thing at a time.

## 4. Avoid “shiny new thing” bias.
- All too often I’ve seen people getting overly excited about the latest ML research paper and trying to force it into their particular use-case. 
- `The reality is that the problems we tackle in ML production are oftentimes much different from the problems studied in ML research`.
- `The antidote to “shiny new thing” bias is, once again, to rigorously follow the scientific method and formulate clear hypotheses prior to running any experiments`.









