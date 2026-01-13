Amazon Web Services1

AI-Driven Development Lifecycle (AI-DLC)Method Definition

Raja SP, Amazon Web Services

I.CONTEXT

The evolution of software engineering has been a continuous

quest to enable developers to focus on solving complex problems

by abstracting away lower-level, undifferentiated tasks. From

early machine code to high-level programming languages and the

adoption of APIs and libraries, each step has significantly boosted

developer productivity. Now, the integration of Large Language

Models has revolutionized how software is created, introducing

conversational natural language interactions for tasks like code

generation, bug detection, and test generation. This marks the

AI-Assistedera, where AI enhancessuchfine-grained, specific

tasks.

As AI evolves, its applications are expanding beyond code

generation to include requirements elaboration, planning, task

decomposition,design,andreal-timecollaborationwith

developers. This shiftis kick-startingtheAI-Drivenera, where AI

actively orchestrates the development process.But, existing

software development methods, designed for human-driven,

long-running processes, arenot fullyalignedwith AI’s speed,

flexibility, and advanced capabilities(ex. agentic).Their reliance

on manual workflows and rigid role definitions limits the ability

to fully leverage AI. Retrofitting AI into these methods not only

limitsits potential,but also reinforces outdated inefficiencies.To

fullyleverageAI’s transformative power, SDLC methodsneed to

be reimagined. This reimagination requires AI to be a central

collaborator, aligning workflows, roles, and iterations to enable

faster decision-making, seamless task execution, and continuous

adaptability.

Thispaper introduces and defines theAI-Driven Development

Lifecycle (AI-DLC),a reimagined, AI-nativemethodologydesigned

to fully integrate the capabilities of AI, setting thefoundationsfor

the next evolution in software engineering.

II.KEYPRINCIPLES

The principles in this section form the foundation for defining AI-

DLC, shaping its phases, roles, artifacts, and rituals. These

assumptions are critical for validating the proposed method, as

they provide theunderpinningrationale behind its design.

1. REIMAGINE RATHER THAN RETROFIT

We choose to reimagine a development method rather than

keeping theexisting methods like SDLC or Agile (e.g., Scrum)and

retrofittingAI intothem. Thesetraditionalmethodswere built

forlonger iterationduration (months and weeks),which ledto

rituals like dailystandupsand retrospectives. In contrast,proper

application of AI leads torapid cycles,measured in hours or days.

Thisneedscontinuous,real-timevalidationandfeedback

mechanisms,renderingmanyofthetraditionalritualsless

relevant.Would effort estimation (ex. story points) be as critical

if AIdiminishesthe boundaries between simple, medium and

hard tasks? Would metrics like velocity be any relevant or should

we start replacing it with Business Value, as an example? Also,AI

is increasinglyevolvingtoautomatemanual practices including

planning, task decomposition, requirements analysis,application

of design techniques (ex. domain modelling),therebyshortening

the number of phases it takes frommovingintentions tocode.

These new dynamics warrant areimagination based on first

principlesthinking,ratherthanaretrofitting.Weneed

automobiles and not the faster horse chariots.

2.REVERSETHECONVERSATIONDIRECTION

AI-DLC introduces a fundamental shift whereAIinitiates &

directsthe conversationswithhumans instead of humans

initiating theconversationwithAIto complete their tasks. AI

drivesworkflowsbybreakingdownhigh-levelintents(ex.

implementing a new business function)into actionable tasks,

generating recommendations, and proposing trade-offs.Humans

serve as approvers, validating, selecting options, and confirming

decisions at critical junctures.This AI-drivenapproachallows

developers to focus on high-value decision-making while AI

handlesplanning,taskdecomposition,andautomation.By

reversing the traditional dynamic, AI-DLC ensures that human

involvementispurposeful,concentratingonoversight,risk

mitigation, and strategic alignment, thereby enhancing both

velocity and quality.Ananalogy to illustrate this is Google Maps:

humans set the destination (the intent), and the system provides

step-by-stepdirections(AI’staskdecompositionand

recommendations). Along the way, humans maintain oversight

and moderatethe journey as needed.

3\. INTEGRATION OF DESIGN TECHNIQUES INTO THE CORE

AgileframeworkslikeScrumorKanbanleavesthedesign

techniques(ex.DomainDrivenDesign)outofscopeand

recommends the teams to choose their own. This has left critical

whitespaces that led to poor software quality overall.Software

quality issues in US alonewasestimated to cost $2.41 Trillion in

2022 (study). Rather than decoupling design techniques out, AI-

DLC will have them asitsintegral core. There will be different

flavors of AI-DLC for teams followingDomain DrivenDesign

(DDD),BehaviorDrivenDevelopment(BDD)orTest-Driven

Development (TDD)respectively. This paper discusses the DDD

Amazon Web Services2

flavor ofAI-DLCwhichwilluse DDD principlesto break down

systems into independent, right-sized bounded contexts that can

berapidlybuiltinparallel.AIwillinherentlyapplythese

techniques during planning and task decomposition, requiring

developers only to validate and adjust. This integrationis key to

enabling hourly or daily iteration cycles while eliminating manual

heavy-liftingand maintaining software quality (the mantra of

“Build Better Systems Faster”).

4.ALIGN WITHAI CAPABILITY

This paper isoptimistic about the future potential of AI but fully

realisticabout its current state.AI-DLCrecognisesthatcurrent AI

is advancing but not yetreliable in autonomously translating

high-level intentions into executable code or independently

operatingwithouthumanoversight,whilealsoensuring

interpretability and safety.At thesame time, theAI-Assisted

paradigm,wheredevelopersperformthemajorityofthe

intellectual heavy liftingwithAI merely providingaugmentation,

fails to unlock the full potential of AI indevelopment.AI-DLC

adoptstheAI-Drivenparadigm,whichbalanceshuman

involvement with the capabilities and limitations of current AI.In

this, thedevelopers retain ultimate responsibility for validation,

decision-making, and oversight. This balance ensures that the

strengths of AI are leveraged effectively without compromising

thecriticalsafeguards provided bydeveloperjudgment.

5.CATER TO BUILDINGCOMPLEXSYSTEMS

AI-DLCcaters tobuildingsystems that demandcontinuous

functional adaptability,higharchitectural complexity,numerous

trade-offsmanagement,scalability,integrationand

customization requirements. Thesenecessitate the application of

advanceddesigntechniques,patterns,andbestpractices,

typically involvingmultiple teams workingcohesivelywithin

largeand/or regulatedorganizations. Simpler systems that can be

developed by non-developer personasthat needed few or no

trade-off managementare outside the scope of AI-DLC and are

bettersuited for low-code/no-code approaches.

6. RETAIN WHAT ENHANCES HUMAN SYMBIOSIS

While reimaginingthe method, wewill retaintheartifacts and

touchpointsfrom the existing methodsthat arecritical for human

validation and risk mitigation. Forinstance, user stories align

humans’and AI’sunderstanding of what needs to be built,acting

as well-defined contracts. We will retain user stories as they are

in the re-imagined method also. Another example isthe Risk

Registerthatensures AI-generated plans and codes comply with

organizational risk frameworks. These retained elements will be

optimized for real-time use, allowing rapid iterations without

compromising alignment or safety.

7.FACILITATE TRANSITION THROUGHFAMILIARITY

The new method shall not demand extensive trainings and any

existing practitioner should be able to orient and start practicing

it in a single day.To support easier adoptionvia associative

learning,AI-DLCwillpreservetheunderlyingrelationships

between familiar terms in older methods while introducing

modernizedterminology.Forexample,SprintsinScrum

represent iterative cycles for building and validating. But Sprints

are usually 4 to 6 weeks long in the pre-AI era. WithAI-DLC, the

iteration cycles will be continuous and in terms of hours or days.

Therefore, we need to intentionally rename Sprints.AI-DLC

rebrands Sprints as Bolts, emphasizing rapid, intense cycles that

deliver unprecedented velocity.

8.STREAMLINERESPONSIBILITIESFOR EFFICIENCY

By leveraging AI’s abilityto performtask decomposition, and

decision-making, developerswill beempowered to transcend

traditional specialization silos such as infrastructure, front-end,

back-end,DevOps,andsecurity.Thisconvergenceof

responsibilities reduces the need for multiple specialized roles,

streamlining the development process.ButProduct Owners and

developers remain integral to the framework, retainingcritical

responsibilities for oversight, validation, and strategic decision-

making. These roles ensure alignment with business objectives,

maintain design quality, andmaintaincompliance with risk

managementframeworks,preservingthebalancebetween

automation and human accountability.In the method definition,

we will stick to first principles, keeping theroles minimum, with

additional roles introduced only when critically necessary.

9.MINIMISESTAGES, MAXIMISE FLOW

Throughautomation andconvergenceof responsibiliti4es, AI-

DLCaims tominimize the handoffs and transitions, enabling

continuous iterative flow. Buthuman validation and decision-

making remain critical to ensure that AI-generated code does not

become rigid ('quick-cement') but stays adaptable for future

iterations. To address this, AI-DLC incorporatesminimal but

sufficient number of phasesspecifically designed for human

oversight at critical decision junctures. These validations act as a

form of 'loss function’, by identifying and pruning wasteful

downstream efforts beforethey occur.

10.NO HARD-WIRED, OPINIONATEDSDLCWORKFLOWS

AI-DLC avoids prescribingopinionatedworkflows for different

developmentpathways(suchasnewsystem development,

refactoring, defect fixes, or microservice scaling). Instead, it

adopts a truly AI-First approach where AI recommends the Level

1 Plan based on the given pathway intention. Humans verify and

moderate these AI-generated plans through interactive dialogue

with AI, continuing this process through Level 2 (subtasks) and

subsequent hierarchy levels. At the task execution level, AI

implements the tasks while humans maintain oversight through

verification and validation of outcomes. This flexible approach

ensures the methodologyis adaptable andcan evolve alongside

Amazon Web Services3

AI capabilities while maintaining human control over critical

decisions.

III.CORE FRAMEWORK

This sectionoutlines thecore frameworkof AI-DLC, detailing its

phases, roles, workflows, and key artifacts.

1\. ARTEFACTS

AnIntentin AI-DLC is a high-level statement of

purpose that encapsulates what needs to be achieved, whether a

business goal, a feature, or a technical outcome(ex. performance

scaling).ItservesasthestartingpointforAI-driven

decomposition into actionable tasks, aligning human objectives

with AI-generated plans.

AUnitrepresents a cohesive, self-contained work

element derived from an Intent, specifically designed to deliver

measurable value. For instance, an Intent to implement a

business idea may be decomposed into Units representing

independent functionalblocks, analogous toSubdomains inDDD

or Epics in Scrum. Each Unit encompasses a set oftasks (user

stories, in this case,that articulate its functional scope)In the

context of AI-DLC, the process of decomposing Intents into Units

is driven by AI, with developers and/or Product Owners validating

and refining the resulting Units to ensure alignment with business

and technical objectives.The units areloosely coupled, enabling

autonomousdevelopmentandindependentdeployment

downstream.

ABoltisthe smallest iteration in AI-DLC, designed for the

rapid implementation of aUnitoraset of taskswithina Unit.

Bolts(analogous to Sprints in Scrum)emphasize intense focus

and high-velocity delivery, with build-validation cycles measured

in hours or days rather than weeks. Each Bolt encapsulates a well-

defined scope of work (e.g., a collection of user stories within a

Unit),enablingincrementalprogresswhilemaintaining

alignment with the overall objectives of the Unit it supports. A

Unit can be executed through one or more Bolts, which may run

in parallel or sequentially. AI will plan the Bolts with developers /

Product Owners validating it.

TheDomain Designartefactmodelsthe core business

logicof a Unit, independently ofthe infrastructurecomponents.

In the first version of AI-DLC,AI uses domain-driven design

principles to createthe strategic and tacticalmodellingelements

including aggregates, value objects, entities, domain events,

repositories and factories.TheLogical Designtranslates Domain

Designs byextending them for meeting thenon-functional

requirementsusingthe right choice ofarchitecturaldesign

patterns(ex.CQRS,CircuitBreakersetc.).AIcreatesthe

Architecture Decision Records(ADRs)for validation by the

Developers.WiththeLogicalDesignspecification,AIwill

generate theCodeandUnit Tests, ensuring adherence towell-

architected principles by selecting appropriate AWS services and

constructs.At this stage, the AI agent will conduct the unit

testing, analyse the results and provide recommendations on

fixes to the Developer.

TheDeployment Unitsarethe operational artifacts

encompassing the packagedexecutablecode(ex.container

images for Kubernetes environments, serverless functions such

asAWSLambda),configurations(ex.HelmCharts),and

infrastructure components(ex. Terraform or CFN stacks) that are

tested for functional acceptance, security, NFRs and other risks.

AI generates all associated tests, including functional tests, static

and dynamic security tests, and load testing scenarios.After the

human validation and adjustments on the test scenarios and

cases, the AI agent executes the test suits, analyses the results

and correlate failure points with code changes, configurations or

other dependencies.Thus,theseunits are rigorously tested for

functional acceptance, security compliance, adherence to non-

functional requirements (NFRs), and mitigation of operational

risks, guaranteeing their readiness for seamless deployment.

2\. PHASES & RITUALS

TheInception Phasefocuses on capturingIntentsand

translating them intoUnitsfor development. This phase uses the

“Mob Elaboration”, a collaborative requirements elaboration and

decomposition ritual.This happens in a single roomwith a shared

screen led by a facilitator.During Mob Elaboration, AI plays a

Amazon Web Services4

central role in proposing an initial breakdown of the Intent into

User Stories, Acceptance Criteria andUnits, leveraging domain

knowledge,andtheprinciplesofloosecouplingandhigh

cohesion for rapid parallel execution downstream. TheProduct

Owner,Developers, QA and other relevant stakeholders(the

mob)collaborativelyreviewandrefinetheseAI-generated

artefacts byadjusting under-engineered or over-engineered

partsand aligning them with real-world constraints.The outputs

of this phase include well defined Units and their respective

components containing a) PRFAQ, b) User Stories, c) Non-

Functional Requirement (NFR) definitions, d) Description of Risks

(matchingwithorganization’sRiskRegister,ifpresent),e)

Measurement Criteria that traces to the business intent and the

f) Suggested Bolts using which the Units can be constructed.Mob

Elaboration condenses weeks or even months of sequential work

into a few hours, while achieving deep alignment both within the

mob and between themoband the AI.

TheConstructionPhaseTheencompassesthe

iterative execution of tasks, transforming the Units defined

duringtheInceptionPhaseintotested,operations-ready

DeploymentUnits.ThisphaseprogressesthroughDomain

Design, where AI models the business logic independently of

technical considerations, toLogical Design, where non-functional

requirements andappropriate cloud designpatterns are applied.

AI generates detailed code from Logical Designs by mapping

components to appropriate AWS services while adhering to well-

architected principles. The phase concludes with automated

testingtoensurefunctionality,security,andoperational

readiness. Developersfocus on validating AI-generated outputs

at each stepand making critical decisions, ensuring quality and

adaptabilityineachiteration.Inthebrown-field(existing

application) scenarios, the construction phase involvesfirst

elevating the codes into asemantic richmodelling representation

so that the context to AI becomes concise and accurate.The

suggested modelling representations arestatic models(just the

domain components, responsibilitiesand their relationships) and

dynamic models(how the components interact to realize the

significant use cases)

AI plays a pivotal role throughout this phase,recommending

tasks and providing options(design patterns, User Experience,

Tests etc)at eachtask.AI-DLC recommends that this be done with

allteams collocated in a single room, similar to Mob Elaboration.

The teams exchange the integration specifications (from domain

model stage), make decisions and deliver their bolts. AI-DLC calls

this the mob-construction ritual.

TheOperationsPhaseinAI-DLCcentersonthe

deployment,observability,andmaintenanceofsystems,

leveraging AIforoperational efficiency. AI actively analyzes

telemetry data, including metrics, logs, and traces, to detect

patterns, identify anomalies, and predict potential SLA violations,

enabling proactive issue resolution. Additionally, AI integrates

withpredefinedincidentrunbooks,proposingactionable

recommendations such as resource scaling, performance tuning,

or fault isolationand execute the resolutions when approved by

the Developers. Developers serve as validators, ensuring AI-

generated insights and proposed actions align withSLAsand

compliance requirements.

3\. THEWORKFLOW

Given a business intent(ex.Green-Field development, Brown-

Field enhancement, modernization, or defect fixing),AI-DLC

begins bypromptingAI togeneratea Level 1 Plan that outlines

theworkflowto implement the intent. This plan serves as an

initial proposal, which is then transparently reviewed, validated,

and refined by humans to ensure alignment with business goals

and engineering constraints.At the heart of AI-DLC is the

principle of applying human oversight to progressively enrich the

artefactsof each step, transforming themintosemantically rich

context for the next.Each stepservesas a strategic decision point

wherehuman oversight functions like aloss function-catching

and correcting errors early before they snowball downstream.

This repeats recursively.Each step in the Level 1 Plan isfurther

decomposed into finer-grained, executable sub-tasks by AI, again

under human oversight to ensure accuracy and contextual

appropriateness.

All artefacts generated(intents, user stories, domain models, or

test plans)are persisted and serve as a “context memory” that

the AI referencesacross the lifecycle. Like traditional SDLC

methods, AI-DLC is inherently iterative, allowing for continuous

refinement and adaptation. Additionally, all artefacts are linked,

allowing for backward and forwardtraceability(ex.connecting

domain model elements to specific user stories)ensuring that the

AI retrieves the correct and most relevant context at every stage.

Throughout the process, AI performs thestrategicplanning, task

decomposition,generationetc.andhumansprovidethe

oversight and validation.

IV.AI-DLC IN ACTION: Green-Field Development

Amazon Web Services5

Wewill examine the scenario in which the Product Owner

commences the process by articulating a high-level intent, such

as "Develop a recommendation engine for cross-selling products."

AI Recognizes this as an intent to build a new application and

produces the Level 1 plan like the Workflow steps in the above

section. The team validates, verifies and adds/fixes the stages in

the level 1 plan. With the finalized Level 1 Plan, AI progresses to

the Inception Phase. Refer to the prompts inAppendix Aas a way

tointeract and provide oversights to AI.

1.INCEPTION PHASE

The following bullet points outline the keyinteractionsinthe

Mob Elaboration ritual.

a.AI asks clarifying questions (e.g.,"Who are the primary users?

What key business outcomes should thisachieve?"), ensuring

a comprehensive understanding of the goaland minimize the

ambiguity in the original intention

b.AIelaborates the clarified intentionintouser stories,non-

functional requirements (NFRs), andrisk descriptions.The

team validates these artefacts and providesoversight,and

the corrections needed to AI.

c.AIcomposes the highly cohesive stories intoUnits, e.g.,"User

Data Collection,""Recommendation AlgorithmSelection,"

and"API Integration."

d.TheProductOwnervalidatestheseoutputs,adjusting

whereverneeded to refine the Units.Example: TheProduct

OwnernoticesthatUserDataCollectionlacksprivacy

compliance details and adjusts the requirements to include

GDPR-specific considerations.

e.AIgeneratesaPRFAQforthemodule(optional),

summarizing the business intent, functionality, and expected

benefits.

f.Developers and Product Owners validate the PRFAQ and

associatedrisks,ensuringalignmentwiththeoverall

objectives.

2\. CONSTRUCTION PHASE

Thefollowing bullet points outline the key activities involved in

this phase, focusing on the Mob Programming and Mob Testing

rituals.

a.The Developer establishes the session with AI.AI prompts the

developer to begin withthe Unit assigned to them.

b.AI models the core business logic forthe assignedUnit using

Domain-DrivenDesignprinciples.Example:Forthe

"Recommendation Algorithm"Unit, AI identifies relevant

entities likeProduct, Customer, and Purchase Historyand

their relationships.

c.Developers review and validate the domain models, refining

businesslogicandensuringalignmentwithreal-world

scenarios(e.g., how to handle missing purchase history for

new customers)

d.AI translates the domain models into logical designs, applying

NFRslikescalabilityandfaulttolerance.Example:AI

recommendsarchitecturalpatterns(e.g.,event-driven

design) and technologies (e.g., AWS Lambda for serverless

computation).

e.Developers evaluate AI’s recommendations, approve trade-

offs, and suggest additional considerations if needed.(e.g.,

Accepts Lambda for scalability but overrides thestorage to

DynamoDB for faster query performance)

f.AI generates executable code for each Unit, mapping logical

components to specific AWS services.

g.It also auto-generates functional, security, and performance

tests(e.g.,For the"Recommendation Algorithm"Unit, AI

createscodetoimplementcollaborativefilteringand

integrates it with a DynamoDB data source)

Amazon Web Services6

h.Developersreviewthegeneratedcodeandtest

scenarios/cases, making adjustments where necessary to

ensure quality and compliance.

Testing and Validation:

a.AIExecutes all tests (functional, security, and performance),

analyzes results, and highlights issues.

b.Proposes fixes for failed tests, e.g., optimizing query logic for

better performance.

c.Developers validate AI’s findings, approve fixes, and rerun

tests as needed.

3.OPERATIONS PHASE

Deployment:

a.AIpackagesthemoduleintoDeploymentUnits(e.g.,

container images, serverless functions).

b.Developersapprovethedeploymentconfigurationand

initiate rollout to staging and production environments.

Observability and Monitoring:

a.AI analyzes metrics, logs, and traces to identify anomalies

and predict potential SLA violations.Example: AI detects a

latency spike during peak usage and proposes scaling the

recommendation engine to handle increased traffic.

b.AIintegrateswithplaybookstosuggestactionsfor

operationalissues.IfAPIresponsetimesdegrade,AI

recommendsincreasingDynamoDBthroughputor

rebalancing API Gateway traffic.

c.DevelopersvalidateAI’srecommendations,approve

mitigations, and monitor resolution outcomes.

V.AI-DLC IN ACTION: Brown-Field Development

Brown-field refers to making changes to an existing system in

terms of either adding new features, optimizing it for non-

functionalrequirementsorfixingtechnicaldebtsincluding

refactoring and fixing defects. In this context, we will examine a

scenariowhere the product manager needs to add a new feature

to an existing application.

1\. INCEPTION PHASE

The inception phase activities in the brown-filed are same as that

of the green-field

2.CONSTRUCTTIONPHASE

a.AIelevatesthecodesintoahigher-levelmodelling

representation.Themodelscompriseofstaticmodels

(components,descriptions,responsibilitiesand

relationships) and dynamic models (how the components

interact to realize the most significant use cases)

b.Developerscollaborate with product managers toreview,

validateand correctthe static and dynamic models that are

reverse engineered by AI.

c.With these extra steps, the rest of the construction phase is

similar to that of the green-field scenario.

3\. OPERATIONS PHASE

The operations phase activities in the brown-filed are same as

that of the green-field

VI.ADOPTING AI-DLC

AI-DLCdoesnot deviatemuchfrom the existing Agile methods

and itis designed with easier adoption as akeyoutcome. Still

organizations that are practicing the traditional methods for

longer andthose who arein the process of inventing their own

variation ofAI-Native methodsneed specific strategies for

adopting AI-DLC. We believe the following 2 approaches will

make this easier.

a.Learning by Practicing–AI-DLC is actually a set of rituals (Mob

Elaboration, MobConstructionetc.) that can be practiced as

a group. Instead of learning the method via documentation

and traditional trainings, we will get the practitioners to

practice the rituals with the AI-DLC guides in multiple real

world scenarios that are currently being solved by the

practitioners.The AWS Solution Architects have createda

field offering calledAI-DLC Unicorn Gymthatpackages this

approach for hyper-scaling adoption in large organizations.

b.ByembeddingAI-DLC in the new Developer Experience

Tooling–our customers are building their own orchestration

tools that cut across SDLC, providing a unified experience for

their developers. (ex.FlowSourcefrom Cognizant,CodeSpell

by Aspire,AIForceby HCL etc.) By embedding AI-DLCinthese

tools, the developers inlargeorganizations will seamlessly

practice AI-DLC without any need for significant adoption

drives.

Amazon Web Services7

APPENDIXA

The following prompts can be used to interact with AI for

practicing AI-DLC.

##Setup Prompt

We will work on building an application today. For every front end

and backend component we will create a project folder. All

documents will reside in the aidlc-docs folder. Throughout our

session I'll ask you to plan your work ahead and create an md file

for the plan. You may work only after I approve said plan. These

plans will always be stored in aidlc-docs/plans folder. You will

create many types of documents in the md format. Requirement,

featureschangesdocumentswillresideinaidlc-

docs/requirements folder. User stories must be stored in the

aidlc-docs/story-artifactsfolder.ArchitectureandDesign

documents must be stored in the aidlc-docs/design-artifacts

folder.All prompts in order must be stored in the aidlc-

docs/prompts.mdfile.Confirmyourunderstandingofthis

prompt. Create the necessary folders and files for storage, if they

do not exist already.

##Inception

\## User stories

Your Role: You are an expert product manager and are tasked

with creating well defined userstories that becomes the contract

for developing the system as mentioned in the Task section

below. Plan for the work ahead and write your steps in an md file

(user\_stories\_plan.md) with checkboxes for each step in the plan.

If any step needs my clarification, add a note in the step to get

my confirmation. Do not make critical decisions on your own.

Upon completing the plan, ask for my review and approval. After

my approval, you can go ahead to execute the same plan one step

at a time. Once you finish eachstep, mark the checkboxes as done

in the plan.

Your Task: Build user stories for thehigh-levelrequirement as

described here<< describe product descrition>>

<<<After reviewing and changing the plan>>>>

Yes, I like your plan as in the <<md file>>. Now exactly follow the

same plan. Interact with me as specified in the plan. Once you

finish each step, mark the checkboxes in the plan.

\## Units

\-\-\----

Your Role: You are an experienced software architect. Before you

start the task as mentioned below, please do the planning and

write your steps in the units\_plan.md file with checkboxes against

each step in the plan. If any step needs my clarification, please

add it to the step to interact with me and get my confirmation.

Do not make critical decisions on your own. Once you produce

the plan, ask for my review and approval. After my approval, you

can go ahead to execute the same plan one step at a time. Once

you finish each step, mark the checkboxes as done in the plan.

Your Task: Refer to the user stories mvp\_user\_stories.md file.

Group the user stories into multiple units that can be built

independently. Each unit contains highly cohesive user stories

that can be built by a single team. The units are loosely coupled

with each other. For each unit, write their respective user stories

and acceptance criteria in individual md files in the design/ folder.

<<<After reviewing and changing the plan>

I approve. Proceed.

###Construction

\## Domain (component) model creation

\-\-\----

Your Role: You are anexperienced software engineer. Before you

start the task as mentioned below, please do the planning and

write your steps in an design/component\_model.md file with

checkboxes against each step in the plan. If any step needs my

clarification, please add it to the step to interact with me and get

my confirmation. Do not make critical decisions on your own.

Once you produce the plan, ask for my review and approval. After

my approval, you can go ahead to execute the same plan one step

at a time. Once you finisheach step, mark the checkboxes as done

in the plan.

YourTask:Refertotheuserstoriesinthe

design/seo\_optimization\_unit.md file. Design the component

model to implement all the user stories. This model shall contain

all the components, the attributes, the behaviours and how the

components interact to implement the user stories. Do not

generate any codes yet. Write the component model into a

separate md file in the /design folder.

<<<After reviewing and changing the plan>>>>

I approve the plan. Proceed. After completing each step, mark the

checkbox in your plan file.

##: Code Generation

\-\-\----

Your Role: You are an experienced software engineer. Before you

start the task as mentioned below, please do the planning and

write your steps in an md file with checkboxes against each step

in the plan. If any step needs my clarification, please add it tothe

step to interact with me and get my confirmation. Do not make

critical decisions on your own. Once you produce the plan, ask for

my review and approval. After my approval, you can go ahead to

Amazon Web Services8

execute the same plan one step at a time. Once you finish each

step, mark the checkboxes as done in the plan.

Task:Refertocomponentdesigninthe

search\_discovery/nlp\_component.mdfile.Generateavery

simple and intuitive Python implementation for the Natural

Language Processing (NLP) Component that is in the design. For

the processQuery(queryText) method, useamazon bedrock APIs

to extract the entities from the query text. Generate the classes

in respective individual files but keep them in \`vocabMapper\`

directory.

Refer to the generated codes in vocabMapper directory. I want

the EntityExtractor component tomake a call to GenAI. The

current implementation uses the local vocabulary\_repository.

Can you analyse and give me a plan on how I can leverage GenAI

for both the Entity Extraction and Intent Extraction.

##: Architecture

\-\-\----

Your Role: You are an experienced Cloud Architect. Before you

start the task as mentioned below, please do the planning and

write your steps in a deployment\_plan.md file with checkboxes

against each step in the plan. If any step needs my clarification,

please add it to the step to interact with me and get my

confirmation. Do not make critical decisions on your own. Once

you produce the plan, ask for my review and approval. After my

approval, you can go ahead to execute the same plan one step at

a time. Onceyou finish each step, mark the checkboxes as done

in the plan.

Task:Refercomponentdesignmodel:

design/core\_component\_model.md, units in the UNITS/ folder,

cloud architecture in the ARCHITECTURE/ folder, and backend

code in the BACKEND/ folder. Complete the following:

-Generate a end-to-end plan for deployment of the backend on

AWS cloud using \[CloudFormation, CDK, Terraform\].

-Document all the pre-requisites for the deployment, if any.

Once I approve the plan:

-Follow the best practice of clean, simple, explainable coding.

-All output code goes in the DEPLOYMENT/ folder.

-Validate that the generated code works asintended, by creating

a validation plan, generate a validation report.

-Review the validation report and fix all identified issues, update

the validation report.

##: Build IaC/Rest APIs

\-\-\----

Your Role: You are an experienced software engineer. Before you

start the task as mentioned below, please do the planning and

write your steps in an md file with checkboxes against each step

in the plan. If any step needs my clarification, please add it tothe

step to interact with me and get my confirmation. Do not make

critical decisions on your own. Once you produce the plan, ask for

my review and approval. After my approval, you can go ahead to

execute the same plan one step at a time. Once you finish each

step, mark the checkboxes as done in the plan.

Task: Refer to the services.py under the construction/<>/ folder.

Create python flask apis for each of the service there.