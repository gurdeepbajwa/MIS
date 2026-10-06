# Week 04 Tutorial Distillation: Clusters 2 and 5

- Course: Skills for IS Research and Development (ISYS90118)
- Chosen clusters: Cluster 2 and Cluster 5
- Parent tutorial: [[Week 04 - Theories Frameworks and Models Tutorial]]
- Reading list: [[Week 04 - Theory Reading Clusters Reference]]

## What to Learn

Do not memorise every detail. For each paper, know:

1. What problem it addresses.
2. What its theory, model, or framework helps explain or do.
3. How it adds to earlier work.
4. Its Gregor theory type and research level.
5. One useful limit or question.

## Cluster 2: Business Process Analysis

### Main Idea

Cluster 2 studies how organisations can use recorded process data and process models to understand, check, manage, and improve how work occurs.

### Process Mining Manifesto

#### Core Point

Process mining uses event logs from information systems to study real processes instead of relying only on how people think the processes work. An event log records activities linked to a case and may include time, person, device, or other data.

#### Three Types of Process Mining

| Type | Input and task | Output |
| --- | --- | --- |
| Discovery | Uses an event log without a prior model | Builds a model of the process found in the data |
| Conformance checking | Compares an event log with an existing model or rule | Finds matches, gaps, and breaches |
| Enhancement | Combines an event log with an existing model | Repairs or extends the model with facts such as delays, frequency, or service time |

The paper also shows that process mining can examine:

- the order of activities;
- people, roles, systems, or departments;
- properties and paths of cases; and
- timing, delays, demand, and bottlenecks.

#### Contribution

The manifesto defines and organises the field, gives six principles for sound use, and sets out research challenges. One key principle is that event data must receive proper care because poor, incomplete, unclear, or unsafe logs weaken the result. Another is that a model should serve a clear purpose and show the level of detail its user needs.

#### Gregor Classification

- **Main type:** Type V, design and action, because the manifesto guides sound process-mining work and system development.
- **Other elements:** Type I analysis, because it classifies process-mining forms, perspectives, principles, and challenges.
- **Research level:** Mainly organisational, though some processes may cross organisations.

#### Limit

Process mining depends on the scope, meaning, completeness, and quality of recorded events. A system log records what the system captured, which may omit informal work, reasons, feelings, or actions outside the system.

#### Thirty-Second Answer

> The Process Mining Manifesto explains how event logs can help us discover, check, and improve real business processes. Discovery builds a model from the log, conformance checking compares the log with an expected model, and enhancement improves a model with recorded facts. I would classify the manifesto mainly as Gregor Type V because it gives principles for using and developing process-mining methods, with Type I elements because it also classifies the field.

### Business Process Querying Framework

#### Core Point

Organisations hold many designed process models and records of executed processes, but ordinary business intelligence tools may not understand process structure and behaviour. The Process Querying Framework guides the design of methods that search, filter, compare, create, change, or remove items in process repositories.

A process query is a formal instruction for managing a process repository. The framework offers parts that designers can configure for different querying problems. It aims to link process-centred analysis with business intelligence and support strategic, tactical, and operational decisions.

#### Contribution

Polyvyanyy et al. (2017):

- define the process-querying problem and method;
- derive needs from business process management use cases;
- design a configurable framework;
- review prior research to check the framework; and
- use the review to identify gaps for later work.

The paper uses a design science approach. Its main product is a framework that other researchers and developers can use to create process-querying methods.

#### Gregor Classification

- **Main type:** Type V, design and action, because it develops an artefact for designing process-querying methods.
- **Other elements:** Type I analysis, because it structures the field and its research gaps.
- **Research level:** Organisational and, where repositories cover shared work, inter-organisational.

#### Limit

The value of a query depends on clear process meaning, sound data, suitable models, enough computing power, and results that decision-makers can understand. A technically correct query may still give little practical value if users cannot interpret it.

#### Thirty-Second Answer

> The Process Querying Framework addresses the problem of searching and managing large stores of process models and execution records. It gives configurable parts for building different query methods and links process analysis with business intelligence. It is mainly Gregor Type V because it creates a design artefact and guidance for later methods. It also offers Type I analysis by organising existing work and exposing gaps.

### How the Two Cluster 2 Papers Connect

The manifesto defines what process mining is, what it can do, and the principles needed for sound use. The Process Querying Framework focuses on how researchers and organisations can search and manage many process models and records. Both seek useful facts about organisational work, but process mining focuses on learning from event traces while process querying focuses on formal requests across process repositories.

## Cluster 5: Information and Digital Experience

### Main Idea

Cluster 5 studies how people look for and receive information, how providers communicate it, and how people may change the digital sources they depend on when their setting changes.

### Information Seeking and Communication Model

#### Core Point

Many information-behaviour models focus on the person seeking information. Many communication models focus on the person or organisation providing it. Robson and Robinson (2013) bring both sides into one conceptual model.

The model considers:

- the information user and the information provider;
- personal and situational factors;
- needs, goals, knowledge gaps, and views;
- whether the user seeks information and which sources they choose;
- whether the provider communicates, what it communicates, and how; and
- factors that affect successful communication and later use of the information.

#### Contribution

The authors review established information-seeking and communication models, find shared and missing parts, and build a new combined model. The paper therefore develops a model from prior theory rather than testing it with new field data.

#### Gregor Classification

- **Main type:** Type II, explanation, because the model explains how personal, situational, seeking, and communication factors shape information exchange and use.
- **Other elements:** Type I analysis, because it organises concepts from two research fields.
- **Research level:** Individual and group, with links to organisational information providers.

#### Limit

The paper builds the model from prior literature. Later research must test where it works, which links matter most, and how it changes across people, tasks, channels, and settings.

#### Thirty-Second Answer

> Robson and Robinson argue that information seeking and communication should be studied together. Their model includes both the user looking for information and the provider deciding what and how to communicate. I would place it mainly in Gregor Type II because it explains the information exchange process, with Type I elements because it brings concepts from several models into one structure.

### Digital Journeys Framework

#### Core Point

Chang and Gomes (2017) define a digital journey as a person's move from relying on one regular set of digital information sources to a different set. They call each regular set a digital bundle. An international student may move to a new country without making the same move online and may keep using familiar sources from home.

The framework places the international student at the centre and considers two broad sets of factors:

- **Internal factors:** self-identity, group identity, digital skill, and information skill.
- **Journey-supporting factors:** the ease and usefulness of new sites, available devices, other online users, digital guides, mentors, and communities.

The framework shows that physical travel does not ensure a digital transition. Students may keep an old bundle, add a new bundle, move between both, or rely mainly on new sources.

#### Contribution

The authors combine work on information behaviour, social media, and international student experience to develop a new framework for an under-studied issue. They also suggest practical support through digital orientation, guides, mentors, usable sources, and online communities.

#### Gregor Classification

- **Main type:** Type II, explanation, because it explains how and why students may or may not change the sources they rely on.
- **Other elements:** Type V implications, because it suggests ways institutions can support the transition.
- **Research level:** Individual, community and society, and cross-border.

#### Limit

This is a conceptual paper. The authors state that later research must map and test the framework in more detail. Different nations, platforms, languages, cultures, and student groups may produce different journeys.

#### Thirty-Second Answer

> Digital Journeys explains that moving country does not mean a person changes their online sources. International students may keep a familiar digital bundle from home, adopt a new bundle, or use both. Identity, skills, site design, devices, guides, and communities can affect that change. It is mainly Gregor Type II because it explains a cross-border digital transition, though it also offers guidance for institutions.

### How the Two Cluster 5 Papers Connect

Robson and Robinson provide a broad model that links information seekers with information providers. Digital Journeys applies related ideas to a clear setting: international students deciding which online sources and communities to rely on after moving across borders. The first model helps examine the full exchange of information; the second explains a change in a person's regular source set.

## Comparison Between the Chosen Clusters

| Point | Cluster 2 | Cluster 5 |
| --- | --- | --- |
| Main focus | Processes recorded and modelled by information systems | People seeking, receiving, and changing information sources |
| Main evidence | Event logs, process models, process repositories, and formal queries | Choices, needs, identities, skills, sources, providers, and social settings |
| Main level | Organisational or inter-organisational | Individual, group, community, and cross-border |
| Strong Gregor fit | Type V: design and action | Type II: explanation |
| Main risk | Treating incomplete system records as the whole process | Assuming a conceptual model works for every person and setting |

## Answer to “Did the Articles Use, Develop, or Expand Theory?”

> The Cluster 2 papers mainly develop frameworks for action. The Process Mining Manifesto defines and organises process mining, then gives principles and challenges. The Process Querying paper develops a configurable framework through design science and checks it against prior research. The Cluster 5 papers develop explanatory models. Robson and Robinson combine information-seeking and communication models, while Chang and Gomes bring information behaviour, social media, and international student research together to create the Digital Journeys framework.

## One-Minute Tutorial Answer

> I chose Clusters 2 and 5 because they show two different roles for theory and models in IS research. Cluster 2 is process-centred. The Process Mining Manifesto shows how event logs can support discovery, conformance checking, and enhancement, while the Process Querying Framework guides methods for searching and managing process repositories. These fit Gregor's design-and-action type. Cluster 5 is person-centred. Robson and Robinson link the information seeker with the information provider, while Digital Journeys explains why international students may keep or change the digital sources they depend on after moving countries. These fit Gregor's explanation type. The comparison shows why the research level and intended theory contribution matter.

## Questions to Ask in Class

- When does an event log give sound evidence of a process, and what parts of work might it miss?
- Is the Process Mining Manifesto itself a theory, or is it a framework that supports design and action?
- Could the Information Seeking and Communication Model help test the Digital Journeys framework?
- How could a university detect a failed digital journey without tracking students in an intrusive way?
- Could process mining study students' digital journeys, or would system logs miss too much personal and cultural context?

## Quick Recall

1. The three process-mining types are **discovery, conformance checking, and enhancement**.
2. The Process Querying Framework helps create methods for **searching and managing process repositories**.
3. Robson and Robinson join the **information seeker and information provider** in one model.
4. A digital journey is a change from one relied-on **digital bundle** to another.
5. Cluster 2 is mainly **design and action**; Cluster 5 is mainly **explanation**.

## References

Chang, S., & Gomes, C. (2017). Digital journeys: A perspective on understanding the digital experiences of international students. *Journal of International Students, 7*(2), 347–366. https://doi.org/10.32674/jis.v7i2.385

Polyvyanyy, A., Ouyang, C., Barros, A., & van der Aalst, W. M. P. (2017). Process querying: Enabling business intelligence through query-based process analytics. *Decision Support Systems, 100*, 41–56. https://doi.org/10.1016/j.dss.2017.04.011

Robson, A., & Robinson, L. (2013). Building on models of information behaviour: Linking information seeking and communication. *Journal of Documentation, 69*(2), 169–193. https://doi.org/10.1108/00220411311300039

van der Aalst, W., et al. (2012). Process mining manifesto. In F. Daniel, K. Barkaoui, & S. Dustdar (Eds.), *Business process management workshops* (Lecture Notes in Business Information Processing, Vol. 99, pp. 169–194). Springer. https://doi.org/10.1007/978-3-642-28108-2_19

