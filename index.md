# **DSC 180A MA 4**
Author: Susana Haing 
Contact: shaing@ucsd.edu

## Capstone 
Domain: D01, AI4Good
Mentor: Dr. Ali Arsanjani

## Project Proposal Questions 
**1. What is the most interesting topic covered in your domain this quarter?** 

The most interesting topic covered so far is knowledge graphs, decision graphs, and causal graphs, how they differ and how they can help LLMs/Agents organize information more clearly, which in turn allows them to produce more accurate and grounded information based on data (like news articles) passed in for information gathering, rebuttal, and synthesis. This is as although they organize the same information, they showcase different things in varying formats (although all graphical in nature). Knowledge graphs show entity relationship triples, meaning 2 nodes representing entities or claims, and their relationship between them (i.e claims, causes, "X said 'abc'"). Decision graphs map the logical argument and reasoning paths that the information and the author of the text has taken to present the information, which can help unearth inconsistencies, or hidden manipulations not initially clear through an initial linear pass. Causal graphs track cause-and-effect claims and chains across events within the text. The 3 graphs in combination are easy places for the LLM/Agent to pull its findings from, allowing us to pass it back into the scoring and interpretation, which can help produce a more robust output and overall analysis.

**2. Describe a potential investigation you would like to pursue for your Quarter 2 Project.** 

I would like to investigate how we can further ground an LLM's/Agent's scoring of how veracious a news article is using the knowledge graphs, decision graphs, and causal graphs. I'm curious to see if these work well, or if there is some other graphical organization of information that works better than a combination of these. I also want to determine if there is a difference in token and compute costs between grounding generative AI's outputs using the graphs, as compared to using strictly Fractal Chain of Thought, and if there is any contextual differences. 

**3. What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

My team and I's Quarter 1 Project is building a Veracity Engine, a tool where users can upload any form of textual media, mostly news articles, to understand what aspects within it are factual or false. Additionally, it allow builds various visualizations to interact with the claims and information in the text, such as a knowledge graph. With this, one change I would make in our current approach is to add in a layer of textual synthesis that overlaps the 3 perspectives (economic, sentiment, and political) that we interpret the Veracity Vector and Factuality Factor scores from. This is because for many topics, especially for more controversial news articles and topics, the economic and political perspectives overlap heavily, and oftentimes, the political and economic views have great impacts on the sentiment of the given topic. Keeping that in mind, I'm curious to see how the interpretation of the text changes with the different views, but also, if there is another perspective we can include that potentially provides more nuance and context. 

**4. What other techniques would you be interested in using in your project?**

I am interested in implementing Constrained Chain of Thought onto Fractal Chain of Thought. This is as FCoT uses up an extremely large amount of tokens due to the recursive and iterative structure of the prompt, especially with the scale down and hill-climb. From what I understand, Constrained Chain of Thought, when compared to regular Chain of Thought, was able to maintain similar accuracy and performance rates while using less tokens and processing power. With that in mind, considering how FCoT uses up even more compute and processing power than standard CoT does, I'm curious if we are able to constrain it using methods proposed in CCoT, whilst still getting the same level of detail and security in responses. I'm curious to see if constraining it will have an effect on the reduced hallucinations, self-consistency, and corrections that standard FCoT produces, but using less tokens and lower costs overall.


