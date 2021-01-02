# Security

General software and systems security resources

## Threat Modelling

The threat modeling process can encompass about three steps, each of which will produce an answer the following question.

1. Decompose the application or system infrastructure and diagram it
2. Determine and rank the threats
3. Determine countermeasures and mitigations

### Diagramming System/Application Architecture

The first step is to model the system either with data or process flow diagrams (DFDs/PFDs) or other relevant diagrams such as Threat Trees (TTDs). From these diagrams, you can identify assets of interest for bad actors such as data stores, application programming interfaces (APIs) that expose data or functionality, and user interfaces that expose data or functionality.

-   https://drawio-app.com/analysing-vulnerabilities-with-threat-modelling-in-draw-io/
-   https://michenriksen.com/blog/drawio-for-threat-modeling/
-   https://github.com/michenriksen/drawio-threatmodeling
-   https://www.csoonline.com/article/3537370/threat-modeling-explained-a-process-for-anticipating-cyber-attacks.html

#### Diagram Types

-   Data Flow Diagrams (DFDs)
-   Process Flow Diagrams (PFDs)
-   Threat (or Attack) Tree (TTDs)

### Assessing and Ranking Threats

The second step is to understand the potential threats and imagine what a bad actor might do to attack your system. Ask questions such as "What mechanisms could the actor use gain access to an asset and retrieve restricted information, manipulate information within the system, or cause the system to fail or be unusable".

Additionally you should try to rank the severity of the action and determine how much damage the actor could do given access to the asset.

### Countermeasures and Mitigations

The third step is to determine how to mitigate or counter a threat. This can be aided by a diagram called a threat tree. At the root of the tree is the threat itself, and its leaves are the conditions that must be true for the actor to realize their goal.

For example, under the condition that an adversary makes an illicit payment. The fact that the person uses a stolen credit/debit card is a subcondition. For each of the leaf conditions you must identify potential mitigation strategies. For the payment threat the mitigation is to verify the card using the a reliable verification package. Every path through the threat tree that does not end in a mitigation strategy is a system vulnerability.
