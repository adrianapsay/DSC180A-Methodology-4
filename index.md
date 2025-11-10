# Student & Section Information
Name: Adrian Apsay<br>
UCSD Email Address: adapsay@ucsd.edu<br><br>
Section: A07<br>
Mentor: Ryan Lingo<br>

# Quarter 2 Project Proposal: Brainstorm
1. **What is the most interesting topic covered in your domain this quarter?**<br>
The most interesting topic covered in our domain this quarter was pursuing the evaluation of context policy (not the model) in an AI/LLM system under deterministic and non-deterministic feedback. The agent adapts to prompts/tool policy/memory while the model itself stays fixed, and we measure outcome/efficiency/stability during evaluation. Our capstone currently aims to reframe agent evaluations from leaderboard scores to process-aware improvement loops, which iteratively fix itself overtime by learning from its previous iterations.
2. **Describe a potential investigation you would like to pursue for your Quarter 2 Project.**<br>
A potential investigation we would like to pursue for Quarter 2 is temporal robustness of the system. We want to assess/evaluate the quality of the system's output as the context/data changes over time, and the way we plan on testing this is by creating some sort of shift in our data setup (CIFAR-10 (vision) / IMDB (text) / Titanic (tabular)), and evaluate whether different context controllers such as prompt scaffolds, tool policies, and memory strategies recover performance after this shift.
3. **What is a potential change you’d make to the approach taken in your current Quarter 1 Project?**<br>
A potential change I'd make to our approach in our current Quarter 1 Project is being able to test different context ablations, more specifically different combinations of context settings. An example of this would be "Prompt A + tool X + memory off" vs "Prompt B + tool X, memory on" and so forth. I would also utilize some sort of budgeting/limiting for each run (whether that might be the number of iterations, tokens, time, etc.) so results can be compared more fairly. Results being the amount of tries it takes to reach success, how computationally expensive it is (i.e. tokens/runtime), and how consistent it is across runs.
4. **What other techniques would you be interested in using in your project?**<br>
One technique I would be interested in using for our project is using reinforcement-style controllers that decide which context change to apply next, instead of just manually cycling through them. I would also probably research strategies regarding memory management such as comparing short-term episodic memory vs. long-term distilled summaries to see how different methods of memory retention impact stability and recovery. Optionally (and hopefully), we get to create visual analytics dashboards to display performance across iterations as well.
