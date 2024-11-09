[![License](https://img.shields.io/badge/License-Apache2-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0) [![Community](https://img.shields.io/badge/Join-Community-blue)](https://developer.ibm.com/callforcode/solutions/projects/get-started/)

_INSTRUCTIONS: This GitHub repository serves as a template and example you can use to create a well documented README for your project for the [2024 Call for Code Global Challenge](https://developer.ibm.com/callforcode/global-challenge/)._


# Replace this heading with your team/submission name

- [Project summary](#project-summary)
  - [The issue we are hoping to solve](#the-issue-we-are-hoping-to-solve)
  - [How our technology solution can help](#how-our-technology-solution-can-help)
  - [Our idea](#our-idea)
- [Technology implementation](#technology-implementation)
  - [IBM watsonx product(s) used](#ibm-ai-services-used)
  - [Other IBM technology used](#other-ibm-technology-used)
  - [Solution architecture](#solution-architecture)
- [Presentation materials](#presentation-materials)
  - [Solution demo video](#solution-demo-video)
  - [Project development roadmap](#project-development-roadmap)
- [Additional details](#additional-details)
  - [How to run the project](#how-to-run-the-project)
  - [Live demo](#live-demo)
- [About this template](#about-this-template)
  - [Contributing](#contributing)
  - [Versioning](#versioning)
  - [Authors](#authors)
  - [License](#license)
  - [Acknowledgments](#acknowledgments)

_INSTRUCTIONS: Below are the suggested sections to include in your README file to make sure your project is well documented. You can remove this instruction text._

## Project summary

### The issue we are hoping to solve

REPLACE THIS SENTENCE with a short description, 2-3 sentences in length, of the specific sustainability problem your solution is meant to address.

### How our technology solution can help

REPLACE THIS SENTENCE with a short description of your team's solution, in about 10 words.

### Our idea

INSTRUCTIONS: Replace this paragraph with a longer description of your solution. In about 500 words, describe your solution in more detail. Include the real-world problem you identified, describe the technological solution you have created, and explain how it’s an improvement over existing solutions. You can supply additional documentation in this source code repository that you link to as well.

More detail is available in our [description document](./docs/DESCRIPTION.md).

## Technology implementation

### IBM watsonx product(s) used

_INSTRUCTIONS: Included here is a list of IBM watsonx products. Remove any products you did not use. Leave only those included in your solution code. In your official submission on the Call for Code Global Challenge web site, you are required to provide details on where and how you used each IBM watsonx product so judges can review your implementation. Remove these instructions._

**Featured watsonx products**

- [watsonx.ai](https://www.ibm.com/products/watsonx-ai) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [watsonx.governance](https://www.ibm.com/products/watsonx-governance) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [watsonx Assistant](https://cloud.ibm.com/catalog/services/watsonx-assistant) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

### Other IBM technology used

INSTRUCTIONS: List any other IBM technology or IBM AI services used in your solution and describe how each component was used. If you can provide details on where these were used in your code, that would help the judges review your submission.

**Additional IBM AI services (Remove any that you did not use)**

- [Watson Machine Learning](https://cloud.ibm.com/catalog/services/watson-machine-learning) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [Watson Studio](https://cloud.ibm.com/catalog/services/watson-studio) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [Natural Language Understanding](https://cloud.ibm.com/catalog/services/natural-language-understanding) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [Speech to Text](https://cloud.ibm.com/catalog/services/speech-to-text) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [Text to Speech](https://cloud.ibm.com/catalog/services/text-to-speech) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

- [Language Translator](https://cloud.ibm.com/catalog/services/language-translator) - WHERE AND HOW THIS IS USED IN OUR SOLUTION

### Solution architecture

REPLACE THIS EXAMPLE WITH YOUR OWN, OR REMOVE THIS EXAMPLE

Diagram and step-by-step description of the flow of our solution:

![Video transcription/translaftion app](https://developer.ibm.com/developer/tutorials/cfc-starter-kit-speech-to-text-app-example/images/cfc-covid19-remote-education-diagram-2.png)

1. The user navigates to the site and uploads a video file.
2. Watson Speech to Text processes the audio and extracts the text.
3. Watson Translation (optionally) can translate the text to the desired language.
4. The app stores the translated text as a document within Object Storage.

## Presentation materials

_INSTRUCTIONS: The following deliverables should be officially posted to your My Team > Submissions section of the [Call for Code Global Challenge resources site](https://cfc-prod.skillsnetwork.site/), but you can also include them here for completeness. Replace the examples seen here with your own deliverable links._

### Solution demo video

[![Watch the video](https://raw.githubusercontent.com/Liquid-Prep/Liquid-Prep/main/images/readme/IBM-interview-video-image.png)](https://youtu.be/vOgCOoy_Bx0)

### Project development roadmap

```mermaid
<flowchart TB
    start([Start]) --> step1

    subgraph Preparation[Preparation Phase]
        step1[1. Select Stratascratch as Problem Source]
        step2[2. Select 1 Problem per Task Category]
        
        subgraph PromptEngineering[Prompt Engineering Iteration]
            direction TB
            step3[3. Prompt Engineering]
            evaluate[Evaluate AI Assistants]
            feedback[Adjust Prompts Based on Performance]
            
            step3 --> evaluate
            evaluate --> feedback
            feedback -->|Iterate until satisfactory| step3
        end

        subgraph Outcomes[Iteration Outcomes]
            direction TB
            step4[4. Final Selection of 4 AI Assistants and LLMs]
            step5[5. Final Prompt Templates]
        end

        step6[6. Select 100 Data Science Problems]
        step7[7. Create 100 Prompts Using Templates]

        step1 --> step2
        step2 --> PromptEngineering
        
        %% Show outcomes flowing from the iteration process
        PromptEngineering --> |Results in| Outcomes
        Outcomes --> step6
        step6 --> step7
    end

    subgraph Execution[Execution Phase]
        step8[8. Execute Each Prompt with AI Assistants]
        copilot[Assistant 1: Microsoft Copilot]
        chatgpt[Assistant 2: ChatGPT]
        claude[Assistant 3: Claude]
        perplexity[Assistant 4: Perplexity Labs]
        
        step8 --> copilot
        step8 --> chatgpt
        step8 --> claude
        step8 --> perplexity
        
        step9[9. Submit Code to Stratascratch Platform]
        copilot --> step9
        chatgpt --> step9
        claude --> step9
        perplexity --> step9
        
        step10[10. Execute Code and Save Results]
        step9 --> step10
    end

    subgraph Analysis[Analysis Phase]
        step11[11. Data Analysis: Compare Performance Results]
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
    class step4,step5 outcomes>



See below for our proposed schedule on next steps after Call for Code 2024 submission.

![Roadmap](./images/roadmap.jpg)

## Additional details

_INSTRUCTIONS: The following deliverables are suggested, but **optional**. Additional details like this can help the judges better review your solution. Remove any sections you are not using._

### How to run the project

INSTRUCTIONS: In this section you add the instructions to run your project on your local machine for development and testing purposes. You can also add instructions on how to deploy the project in production.

### Live demo

You can find a running system to test at...

See our [description document](./docs/DESCRIPTION.md) for log in credentials.

---

_INSTRUCTIONS: You can remove the below section from your specific project README._

## About this template

### Contributing

Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

### Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/your/project/tags).

### Authors

<a href="https://github.com/Call-for-Code/Project-Sample/graphs/contributors">
  <img src="https://contributors-img.web.app/image?repo=Call-for-Code/Project-Sample" />
</a>

- **Billie Thompson** - _Initial work_ - [PurpleBooth](https://github.com/PurpleBooth)

### License

This project is licensed under the Apache 2 License - see the [LICENSE](LICENSE) file for details.

### Acknowledgments

- Based on [Billie Thompson's README template](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2).
