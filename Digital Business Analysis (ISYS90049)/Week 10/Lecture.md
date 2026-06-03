# Lecture

Course: [[Digital Business Analysis (ISYS90049)/Course Overview|Digital Business Analysis (ISYS90049)]]
Week: 10
Topic: Requirements Analysis and Design Definition

## Topic

Requirements Analysis and Design Definition

## Key Concepts

### Purpose

Requirements analysis and design definition structures, analyses, models, verifies, and validates requirements and designs so that a suitable solution can be defined.

This knowledge area helps the analyst:

- Structure and organise requirements discovered during elicitation.
- Specify and model requirements and designs.
- Verify that requirements are usable and high quality.
- Validate that requirements align with business needs and solution scope.
- Identify design options that could meet the business need.
- Estimate the potential value of each option and recommend a solution.

### Requirements Classification

| Requirement type | Meaning |
| --- | --- |
| Business need | A problem or opportunity of strategic or tactical importance. |
| Business requirements | Goals, objectives, and outcomes that describe why a change has been initiated. |
| Stakeholder requirements | Needs of stakeholders that must be met to achieve the business requirements. |
| Solution requirements | Capabilities and qualities of a solution that meet stakeholder requirements. |
| Functional requirements | Capabilities that a solution must have. |
| Non-functional requirements | Conditions or qualities under which the solution must remain effective. |
| Transition requirements | Capabilities or conditions needed to move from the current state to the future state, but not needed once the change is complete. |

The lecture distinguishes between the problem domain and the solution domain. Business needs, business requirements, and stakeholder requirements sit closer to the problem domain. Solution, functional, non-functional, and transition requirements sit closer to the solution domain.

The transcript emphasises that Week 10 focuses mainly on solution or system requirements because these are the requirements that bridge analysis work to solution design. Functional and non-functional requirements are especially important at this point because they can be translated into prototypes, use cases, user stories, and system design discussions.

Functional requirements describe capabilities the system should provide, such as allowing users to upload content, log in, create a study group, or track study sessions with a timer. Non-functional requirements describe qualities or constraints such as usability, reliability, scalability, security, compliance, availability, and performance. A useful test is whether the statement describes something the system does for the user, or a quality of how the system must operate.

System requirements should not be confused with SMART objectives. A SMART objective might say that customer satisfaction should increase by 25% within one year. A system requirement should describe an implementable capability or quality, such as allowing users to track a study session with a 25-minute timer. The objective describes the desired business outcome; the requirement describes what the system must do or how it must perform.

### Requirements and Design Cycle

Requirements and designs influence each other. Requirements express what needs to be satisfied; designs describe possible ways to satisfy those requirements.

As analysis progresses:

- Needs are refined into requirements.
- Requirements reveal design options.
- Design options may expose missing, unclear, or conflicting requirements.
- Requirements and designs are iterated until they are sufficiently clear for decision making and delivery.

### Main Tasks

| Task | Purpose |
| --- | --- |
| Specify and model requirements | Analyse, synthesise, refine, document, and represent elicitation results as requirements and designs. |
| Verify requirements | Ensure requirements and designs are defined correctly, consistently, and at enough quality to be usable. |
| Validate requirements | Ensure requirements and designs align with business requirements, solution scope, goals, and objectives. |
| Define requirements architecture | Ensure requirements collectively support one another and achieve the objectives. |
| Define design options | Identify and describe possible ways to meet the need and reach the future state. |
| Analyse potential value and recommend solution | Estimate benefits and costs, compare options, and recommend the most appropriate solution. |

### Specify and Model Requirements

Specifying and modelling requirements means converting elicitation results into clear representations that stakeholders can review and use.

This includes:

- Modelling requirements using textual or visual representations.
- Analysing whether anything is missing, unnecessary, inconsistent, or should be changed.
- Representing requirements and attributes.
- Choosing appropriate levels of abstraction.
- Presenting requirements in formats that different stakeholder groups can understand.

Common formats include:

- Matrices.
- Diagrams.
- Textual descriptions.
- Process models such as BPMN.
- Prototypes and wireframes.
- Use case diagrams and narratives.
- Requirements specification documents.
- User stories.
- Functional decomposition.

The transcript highlights why multiple representations matter. A developer may benefit from process models, use cases, or structured matrices because they show activity flow, actors, or system behaviour more precisely. A senior manager may need a more natural-language or high-level representation because detailed modelling notation can obscure the decision they need to make. The analyst's job is to maintain enough representations to communicate requirements to different audiences without changing the underlying meaning.

### Model Categories

| Model category | Focus | Examples |
| --- | --- | --- |
| People and roles | Organisations, groups, roles, and relationships. | Personas, organisational models. |
| Rationale | Why a change is needed. | Decision modelling, root cause analysis. |
| Activity flow | Sequences of actions, events, or choices. | Process modelling, BPMN. |
| Capability | Features or functions of an enterprise or solution. | Prototyping, capability views. |
| Data and information | Characteristics, structures, or flows of information. | State modelling, data models, interface models. |

Different models provide different viewpoints. A single model is rarely enough for complex requirements work.

### Verify Requirements

Verification checks whether requirements and designs are defined correctly and are ready for validation.

Good requirements should be:

| Attribute | Meaning |
| --- | --- |
| Atomic | Understandable independently and self-contained. |
| Complete | Detailed enough for work to continue at the required level. |
| Consistent | Aligned with stakeholder needs and not contradictory. |
| Concise | Contains enough information without unnecessary explanation. |
| Feasible | Reasonable within project risk, schedule, budget, or exploration value. |
| Unambiguous | Clear enough to determine whether a solution meets the need. |
| Testable | Possible to determine whether the requirement has been fulfilled. |
| Prioritised | Shows relative importance or value compared with related requirements. |
| Understandable | Uses terminology appropriate for the intended audience. |

Verification focuses on requirement quality, notation, internal consistency, and understandability.

### Validate Requirements

Validation checks whether requirements and designs support the business requirements, solution scope, goals, and objectives.

Validation includes:

- Identifying assumptions where information is incomplete.
- Defining measurable evaluation criteria.
- Checking alignment with solution scope.
- Ensuring the requirements support the organisation's goals and objectives.

Verification asks whether requirements are written and modelled well. Validation asks whether they are the right requirements.

### Requirements Architecture

Requirements architecture ensures that requirements collectively support the objectives.

It includes:

- Defining viewpoints, views, model types, notations, and attributes.
- Using template architectures or organisational standards where useful.
- Checking completeness.
- Relating and verifying requirement relationships.
- Defining how requirements, designs, models, and elicitation results connect.

Requirements architecture helps reveal conflicts, dependencies, gaps, and trade-offs.

The transcript distinguishes this from checking individual requirements. Verification and validation can assess whether one requirement is well written, feasible, and aligned with objectives. Requirements architecture checks how requirements relate to one another: dependencies, priorities, conflicts, integration with existing infrastructure, and whether the set of requirements collectively supports the objectives.

Template architectures or existing patterns can be useful where similar problems have already been solved. Analysts do not always need to define every requirement relationship from scratch; they can adapt proven templates where they fit the context.

### Design Options

Design options describe different possible ways to meet the need and reach the future state.

Defining design options includes:

- Deciding whether solution components will be purchased, created, or combined.
- Identifying opportunities to improve business operations.
- Allocating requirements to solution components or planned releases.
- Describing design options while considering the desired future state.

Design options may include changes to business policies, processes, organisational structures, interfaces, data, software, or other solution components.

The transcript explains this as a more detailed step than the future-state solution space. Future state analysis may identify broad options such as a CRM platform, vendor solution, or self-developed system. Requirements analysis and design definition then zooms in: mapping requirements to features, comparing vendors or build options, considering what must be customised, and estimating the cost and fit of specific options.

When using existing platforms, requirements should be allocated at a granular level. A large system may contain more functions than the organisation needs, so the analyst should map requirements to specific components, features, releases, or configuration decisions rather than treating the whole vendor product as a single answer.

### Potential Value and Recommendation

Design options should be compared by estimating their potential value.

Consider:

- Expected benefits.
- Expected costs such as time, effort, operating costs, maintenance costs, and human resources.
- Whether benefits outweigh costs.
- Whether the option satisfies requirements and supports the future state.
- Which option best meets business needs in context.

The analyst recommends the option that best balances value, feasibility, cost, risk, and alignment with requirements.

The transcript stresses that the analyst recommends; authorised stakeholders decide. The analyst should communicate a small number of viable options rather than overwhelming decision makers with every possible alternative.

Expected benefits should relate back to the problem or opportunity being addressed. They do not need to be only financial, and they should not be exaggerated into unsupported revenue claims. Benefits may include solving the specific problem, reducing friction, improving access to information, creating new capabilities, improving user experience, or creating intermediate value that later supports revenue.

### Wireframes

A wireframe is a simplified representation of a system interface.

Wireframes:

- Can be hand-drawn or electronically generated.
- Focus on structure rather than visual design, colour, or branding.
- Are low-fidelity prototypes.
- Support idea generation, brainstorming, and requirements analysis.
- Help stakeholders discuss layout, content, flow, and interaction before expensive design or implementation work begins.

All wireframes are prototypes, but not all prototypes are wireframes.

The transcript distinguishes prototype fidelity:

| Prototype type | Meaning |
| --- | --- |
| Low-fidelity prototype | A rough representation focused on structure. Wireframes sit here. They may be hand drawn and are cheap to change. |
| Medium-fidelity prototype | Shows more realistic interface components, labels, pages, and navigation, but may not be fully functional. |
| High-fidelity prototype | Looks and feels close to the final solution and may allow realistic interaction, but may not be connected to live data or production systems. |

Low-fidelity wireframes are useful early because they create a basis for discussion without the cost and commitment of detailed design. AI tools can generate wireframes quickly, but the analyst still needs to judge whether the output is truly low fidelity or has drifted into a more detailed prototype than needed.

### Use Cases

Use cases illustrate how users interact with a system.

They are useful because they:

- Are technology independent.
- Can be understood without deep IT knowledge.
- Show system behaviour from an actor's perspective.
- Can be represented through use case diagrams and narratives.

Important concepts:

| Concept | Meaning |
| --- | --- |
| Actor | Anyone or anything that interacts with the system. |
| Stakeholder | Anyone interested in the system, even if they do not directly use it. |
| Use case | A piece of functionality or interaction scenario. |
| Trigger | Event that starts the use case. |
| Pre-condition | What must be true before the use case begins. |
| Post-condition | What must be true after the use case completes. |
| Normal flow | The standard sequence of steps. |
| Alternative flow | A variation from the normal path. |

Use case relationships can include include, extend, and generalisation relationships.

Use cases can be written as narratives and then represented as diagrams. The narrative explains the step-by-step user-system interaction, while the diagram visualises actors, system boundaries, use cases, and relationships.

The transcript highlights two common relationships:

| Relationship | Meaning |
| --- | --- |
| Include | A required interaction that must occur for the use case to complete. |
| Extend | An optional or conditional interaction that may occur but is not required for the main use case. |

Use cases complement wireframes. Wireframes show the structural layout of an interface; use cases show the flow of interaction through the system.

#### Extra Materials

- [UML Use Case Diagram Tutorial](https://www.youtube.com/watch?v=1WHjaG_LHsQ) - Imerging Careers. Supports use cases, actors, system boundaries, relationships, and modelling user-system interaction.
- [Use-Case Foundation](https://www.ivarjacobson.com/publications/use-case-foundation) - Ivar Jacobson International. Adds history and purpose: use cases were developed to describe all the ways a user can use a system to achieve a goal, making them a bridge between stakeholder needs and system behaviour.
- [Use Cases: The Ideal Bridge Between Requirements and Design?](https://www.interaction-design.org/literature/article/uses-cases-diagrams-narratives) - Interaction Design Foundation. Useful for understanding why use cases are still taught: they make requirements concrete through scenarios before the solution is fully designed.

## Textbook Connections

Milani Chapter 15 connects directly to the lecture's requirements and design content.

### Requirements and Design

Milani explains that once the general solution path has been chosen, the solution is still not detailed enough for coding or delivery. Requirements must be analysed, refined, modelled, prioritised, approved, and maintained.

Milani also highlights the distinction between requirements and design. Requirements describe what needs to be satisfied; design options describe different ways those requirements could be fulfilled. Organisations may use different terminology, so the analyst must clarify what each term means in context.

### Requirements Lifecycle

Milani connects requirements analysis and design to requirements lifecycle management:

- Requirements are elicited and analysed.
- They are iterated and refined.
- They are captured as models or textual descriptions.
- They are prioritised.
- Work packages or releases are proposed for approval.
- Requirements are maintained for traceability, storage, change control, and reuse.

This links Week 10 back to Week 7 requirements lifecycle management.

### Choosing Models

Milani emphasises that text alone is often insufficient for complex requirements. Models help simplify complexity and communicate different viewpoints. Matrices are useful for structured data, while diagrams are useful for relationships, flows, and complexity.

The analyst should choose models based on context, stakeholder needs, and the type of information being communicated.

### Use Cases and Prototypes

Milani treats use cases as a technology-independent way to describe how users interact with a system. Use cases can include diagrams and narratives, including actors, triggers, preconditions, postconditions, normal flow, and alternative flows.

Milani also treats prototypes and wireframes as useful design tools because they let stakeholders react to a representation of a solution before it is fully implemented. Early low-fidelity prototypes are especially useful because they are cheaper to change than implemented systems.

## Summary

- Requirements analysis and design definition turns elicitation results into usable requirements, models, and design options.
- Requirements and designs evolve together.
- Requirements should be specified, modelled, verified, validated, architected, and linked to design options.
- Good requirements are atomic, complete, consistent, concise, feasible, unambiguous, testable, prioritised, and understandable.
- Wireframes and use cases help stakeholders reason about system structure and interaction.
- Prototype fidelity matters: low-fidelity wireframes are cheap discussion tools, while higher-fidelity prototypes are closer to final design but more costly to change.
- System requirements should be distinguished from business goals or SMART objectives.
- The textbook reinforces that requirements/design work bridges strategy analysis and delivery by refining the selected solution path into usable requirements and design detail.

## Notes

Reading: Milani Chapter 15.

References:

- IIBA. (2015). _A guide to the Business Analysis Body of Knowledge_ (3rd ed.).
- Milani, F. (2019). _Digital business analysis_. Springer. https://doi.org/10.1007/978-3-030-05719-0
