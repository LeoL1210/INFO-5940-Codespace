Building the multi-agent workflow taught me how to create better results by using interaction between two agents. The Planner Agent focuses on turning a short travel prompt into a detailed day-by-day schedule. The Reviewer Agent then checks that plan to make sure it’s realistic. For example, all the landmarks the agent mentioned is not made up. This interaction showed me that splitting tasks by role makes the system more organized and easier to control. It shows me two agents are better than one by dividing tasks and make the system more efficient.

One of the main challenges was putting the API key in the right place. I encountered several problems about the API key failed the authentication. Eventually, I put the API key at the env and also the devcontainer to solve that problem. I also looked at the Tavily API documentation to understand how the search tool works. 

 At first, the Planner created plans that were too unrealistic. The Reviewer will remove wrong information. I solved this by adjusting the Reviewer’s instructions to only point out specific changes instead of rewriting everything. 

For design, I made each agent have its own personality: the Planner sounded friendly and flexible, while the Reviewer was more serious and careful. I also asked the Planner to organize the output not strictly by time. It only provides recommendation of places or restaurant but not like “you should go to this place from 5pm to 6pm” so the plan provides more flexibility. I also add the recommendation tab for prompt for people who do not have any idea about what places they want to go.

External tools and GenAI assistance: I used ChatGPT to help me write and edit the system prompts, fix setup errors, and explain how to structure the agents. 

