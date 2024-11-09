# LLM 4 Data Science

- [Project summary](#project-summary)
  - [The issue we are hoping to solve](#the-issue-we-are-hoping-to-solve)
  - [How our technology solution can help](#how-our-technology-solution-can-help)
  - [Our idea](#our-idea)
- [Presentation materials](#presentation-materials)
  - [Solution demo video](#solution-demo-video)
  - [Project development roadmap](#project-development-roadmap)
- [Additional details](#additional-details)
  - [How to run the project](#how-to-run-the-project)
  - [Live demo](#live-demo)

_INSTRUCTIONS: Below are the suggested sections to include in your README file to make sure your project is well documented. You can remove this instruction text._

## Project summary

### The issue we are hoping to solve

REPLACE THIS SENTENCE with a short description, 2-3 sentences in length, of the specific sustainability problem your solution is meant to address.

### How our technology solution can help

REPLACE THIS SENTENCE with a short description of your team's solution, in about 10 words.

### Our idea

INSTRUCTIONS: Replace this paragraph with a longer description of your solution. In about 500 words, describe your solution in more detail. Include the real-world problem you identified, describe the technological solution you have created, and explain how it’s an improvement over existing solutions. You can supply additional documentation in this source code repository that you link to as well.

More detail is available in our [description document](./docs/DESCRIPTION.md).


### Project development roadmap

```mermaid
flowchart TB
    start([Start]) --> step1

    subgraph Preparation[Preparation Phase]
        step1[1- Select Stratascratch as Problem Source]
        step2[2- Select 1 Problem per Task Category]
        
        subgraph PromptEngineering[Prompt Eng. Iteration]
            direction TB
            step3[3- Prompt Engineering]
            evaluate[Evaluate AI Assistants]
            feedback[Adjust Prompts Based on Performance]
            
            step3 --> evaluate
            evaluate --> feedback
            feedback -->|Iterate until satisfactory| step3
        end

        subgraph Outcomes[Iteration Outcomes]
            direction TB
            step4[4- Final Selection of 4 AI Assistants and LLMs]
            step5[5- Final Prompt Templates]
        end

        step6[6- Select 100 Data Science Problems]
        step7[7- Create 100 Prompts Using Templates]

        step1 --> step2
        step2 --> PromptEngineering
        
        %% Show outcomes flowing from the iteration process
        PromptEngineering --> |Results in| Outcomes
        Outcomes --> step6
        step6 --> step7
    end

    subgraph Execution[Execution Phase]
        step8[8- Execute Each Prompt with AI Assistants]
        copilot[Assistant 1: Microsoft Copilot]
        chatgpt[Assistant 2: ChatGPT]
        claude[Assistant 3: Claude]
        perplexity[Assistant 4: Perplexity Labs]
        
        step8 --> copilot
        step8 --> chatgpt
        step8 --> claude
        step8 --> perplexity
        
        step9[9- Submit Code to Stratascratch Platform]
        copilot --> step9
        chatgpt --> step9
        claude --> step9
        perplexity --> step9
        
        step10[10- Execute Code and Save Results]
        step9 --> step10
    end

    subgraph Analysis[Analysis Phase]
        step11[11- Data Analysis: Compare Performance Results]
    end

    step7 --> step8
    step10 --> step11
    step11 --> endNode([End])

    classDef preparation fill:#e1f3d8,stroke:#82c366
    classDef execution fill:#dae8fc,stroke:#6c8ebf
    classDef analysis fill:#ffe6cc,stroke:#d79b00
    classDef iteration fill:#fff2cc,stroke:#d6b656,stroke-width:3px
    classDef outcomes fill:#ffe6cc,stroke:#d6b656,stroke-width:2px
    
    class step1,step2,step6,step7 preparation
    class step8,step9,step10,copilot,chatgpt,claude,perplexity execution
    class step11 analysis
    class step3,evaluate,feedback iteration
    class step4,step5 outcomes
```


## Additional details

_INSTRUCTIONS: The following deliverables are suggested, but **optional**. Additional details like this can help the judges better review your solution. Remove any sections you are not using._

### How to run the project

INSTRUCTIONS: In this section you add the instructions to run your project on your local machine for development and testing purposes. You can also add instructions on how to deploy the project in production.

### Live demo

You can find a running system to test at...


---
