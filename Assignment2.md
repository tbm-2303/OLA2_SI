links: 
- https://www.enterpriseintegrationpatterns.com/index.html 


# Questions on Enterprise and Solution Architecture

## Q1
**What are the main differences between Enterprise and Solution Architecture?**  
Describe the different roles that these play in designing large-scale systems. You can use resources like the video *Enterprise Architecture vs Solution Architecture* to help you answer.

## Q2
In his video called *Practical Architecture*, what does Stefan Tilkov say about the role of teams in modern architecture? He refers to a book *Team Topologies* – what “team topologies” does the book describe? Do you agree from your own experience that the team is a core part of a successful project?

## Q3
Also in this video, Stefan Tilkov explains why some things are best done centrally (for example at 23 min 30 seconds). Why do you think he is saying this? What does he claim are the benefits?

## Q4
In the video *Architecting for Outcomes*, Simon Rohrer describes old-fashioned and modern enterprise architecture. He talks about the A B C D E of modern architecture to compare modern and legacy ways of working. Do you find his arguments persuasive, and if so, why?

## Q5
In the same video, he explains the concept of the “Continuous Conversation.” In what ways does he say it benefits Saxo Bank? How does he connect the Continuous Conversation to the DevOps Infinity Loop?

## Q6
In the course, we will focus on building integrated enterprise-scale applications using messaging, and there are a number of core Integration Patterns for messaging. Using the PowerPoint presentation for this week called *Enterprise Architecture and Integration Patterns*, describe 5 integration patterns for messaging and provide a use case for them. You can add more depth to your answer by coding the examples (you may have done some of this for OLA1). You should include Pipes and Filters and the Request Reply patterns as part of your answer.

## Q7
In Gregor Hohpe’s talk *Enterprise Integration Patterns 2*, he describes the idea of conversations in a messaging architecture (from 18 minutes). He explains how a ‘messaging’ and ‘conversation’ architecture are different. What differences are there, and what challenges does he describe for conversation-based solutions (for example, what is the difference between pub-sub and subscribe-notify)?

## Q8
Also in Gregor Hohpe’s video, he explains the history and role of the idea of Patterns and Pattern Languages. How would you summarize what he explains – what do you see as the core requirements for patterns to be useful (see about 45 minutes in)?

## Q9
In Simon Rohrer’s article on modern enterprise architecture ([link](https://modernenterprisearchitecture.substack.com/p/modern-enterprisearchitecture-a), also on Moodle in the folder for slides for this week), he goes into more detail about the ABCDE of modern EA. He discusses the ‘strangler’ pattern for moving away from legacy systems – why is this seen as a complex problem, and what does the strangler pattern do to help?

## Q10
In Jesper Lowgren’s video *Solution vs Enterprise Architecture Tutorial*, he describes three core diagrams that can be used to describe an architecture. What are they, and what role do they play? Include examples.

---

# Answer 1 
Enterprise Architecture (EA) and Solution Architecture (SA).

### 1. Scope and Focus
- **Enterprise Architecture (EA):**
  - **Scope:** EA focuses on the entire organization, encompassing the overall structure, strategy, and direction of the enterprise.
  - **Focus:** Deals with aligning technology with business goals and ensuring that IT investments support the organization’s mission and vision. 
EA is concerned with long-term planning and governance.

- **Solution Architecture (SA):**
  - **Scope:** SA is focused on specific projects or solutions within the organization, looking at how to implement particular systems or applications.
  - **Focus:** Focuses on the design of individual systems, including software, hardware, and networking components. 
SA ensures that the solution fits within the EA framework and meets specific business requirements.

### 2. Timeframe
- **EA:** Has a long-term perspective, typically spanning multiple years, involving the strategic planning of technology and its evolution to meet future business needs.
- **SA:** Has a shorter-term perspective, concerned with the design and implementation of solutions within the constraints of the EA.

### 3. Level of Detail
- **EA:** Works at a high level of abstraction, providing a holistic view of the organization’s IT landscape, including frameworks, standards, and policies.
- **SA:** Provides detailed design specifications, including data models, system interfaces, and technology stacks required for implementation.

### 4. Stakeholders
- **EA:** Involves high-level stakeholders, including executives, business leaders, and enterprise architects, focusing on aligning IT strategy with business objectives.
- **SA:** Engages technical stakeholders, such as project managers, developers, and systems engineers, focusing on delivering specific solutions that meet user requirements.

## Roles in Designing Large Scale Systems

### 1. Enterprise Architecture Role
- **Strategic Planning:** EA defines the overarching strategy for technology adoption and integration across the organization.
- **Governance:** Establishes policies and guidelines to ensure that all technology initiatives align with business goals and comply with standards.
- **Framework Development:** Creates models and frameworks that describe the organization’s IT landscape, including data architecture, application architecture, and technology architecture.
- **Change Management:** Plays a crucial role in managing change within the organization, helping to navigate transitions in technology and business processes.

### 2. Solution Architecture Role
- **System Design:** SA designs specific solutions that meet business needs while adhering to EA principles and standards.
- **Technology Selection:** Responsible for selecting appropriate technologies and tools that will be used in the implementation of the solution.
- **Integration:** Ensures that the solution integrates seamlessly with existing systems and adheres to the overall architectural framework set by the EA.
- **Technical Documentation:** Produces detailed technical documentation that guides the development and implementation teams, ensuring that the project remains on track and aligned with business objectives.

___

# Answer 2


1. **Teams as Core Components:** 
   - Teams are fundamental to the success of modern architectural practices. The architecture should be designed with the capabilities, strengths, and communication styles 
of the teams in mind. Effective collaboration among team members can lead to better outcomes and more innovative solutions.

2. **Communication and Collaboration:**
   - Clear communication fosters collaboration and helps ensure that everyone is aligned with the 
project goals. Poor communication can lead to misunderstandings, inefficiencies, and ultimately, project failure.

3. **Adaptability:**
   - Adaptable in response to changing project requirements and market conditions. The architecture should facilitate this adaptability, 
allowing teams to pivot as needed without being hindered by overly rigid structures.

## Team Topologies from the Book "Team Topologies"

Four fundamental team topologies are described, each with distinct responsibilities and interactions:

1. **Enabling Teams:**
   - These teams help other teams improve their capabilities. They provide guidance, support, and tools to enable other teams to deliver their work more effectively.

2. **Complicated Subsystem Teams:**
   - These teams focus on areas of the system that require specialized knowledge or expertise. They handle complex parts of the architecture that may be difficult 
for other teams to manage.

3. **Stream-aligned Teams:**
   - These teams are aligned to a specific flow of work, often corresponding to a particular product or service. Their goal is to deliver value quickly and continuously, 
ensuring that the architecture supports their workflows.

4. **Platform Teams:**
   - These teams create and maintain platforms that other teams can use to build their solutions. They focus on providing reusable services and components, reducing duplication 
of effort across teams.

## Personal Agreement on Team Importance

Team can achieve much more then any individual can. In terms of enterprise integration i tend to emphasize good communication and colaboration skills, when inter-organisational groups
have to work together. Someone working in Research and development might think and act alot different from someone from production. Therefore communication becomes even more important 
in order to convey ideas to one another. Overall, the structure and dynamics of teams significantly influence the effectiveness of the architecture and the success of the project.


___
# Answer 3 

He argues that while decentralization is important for agility and innovation, some functions and responsibilities are better handled centrally. 

1. **Consistency:**
   - Centralization helps ensure consistent practices, standards, and tools across the organization. 
This uniformity can reduce confusion and enhance the quality of work, especially when multiple teams are involved.

2. **Efficiency:**
   - Centralizing specific functions can lead to more efficient use of resources. For example, shared services can avoid duplication of efforts, 
streamline processes, and reduce costs.

3. **Expertise:**
   - Some areas require specialized knowledge that may not be present in every team. Centralizing these functions allows organizations to leverage 
the expertise of a dedicated team, ensuring that best practices are followed.

4. **Governance and Compliance:**
   - Certain activities, such as security, data management, and compliance, often benefit from centralized oversight. This approach helps maintain 
control and ensures that the organization meets regulatory requirements.


- **Improved Collaboration:** Centralized teams can facilitate better collaboration and communication across different departments and teams, 
promoting knowledge sharing and collective problem-solving.
  
- **Faster Decision-Making:** Having a centralized function can expedite decision-making processes by providing a clear point of authority, 
which can reduce delays caused by coordination among multiple teams.

- **Enhanced Focus:** Centralized teams can focus on specific areas without the distractions of multiple projects, leading to deeper expertise 
and more innovative solutions.

- **Scalability:** Centralization allows organizations to scale their operations more effectively. A centralized function can adapt and grow 
in response to changing demands without needing to reconfigure multiple decentralized teams.

---

# Answer 4 and 5
He talks about traditional monolithic enterprices vs modern enterprice architecture and he gives a rough outline of how that transition occured. 
Some big and old enterprices, using legacy software and systems, might have a harder time comverting to microservice oriented architecture. 
These things take time and some services and teams are being developed, but much of the enterprise is still monolithic in nature.

continuous conversation:
instead of phase based review, continuous conversations allows for designing and architecting during development. Teams 
can reach out and talk to dedicated architects. Adding new services could introduce unwanted complexity and it could be worth discussing 
wether or not to invest in new services or find ways to combine features with existing services. They are there to help ensure the business value
chain is operating as efficiently as possible.In terms of the devops loop, he says the Continuous conversation slots in perfectly.




# Answer 6
Messaging
Message Channel
Message
Pipes and Filters
Message Router
Message Translator
Message Endpoint

# Integration Patterns for Messaging

## 1. Pipes and Filters
The Pipes and Filters pattern is a method for processing data streams where each filter processes the data and passes the results to the next filter through a pipe. 
This pattern is highly modular, allowing independent filters to be reused and maintained separately.
Usecase:
In a data analytics system, raw data is ingested from various sources (e.g., sensors, logs) and passed through multiple filters that perform transformations 
(e.g., cleaning, aggregating, enriching). Each filter processes the data independently, and the final output can be stored in a database or sent to a reporting tool.

## 2. Request-Reply
The Request-Reply pattern is a synchronous messaging pattern where a sender sends a request message and waits for a corresponding reply. 
This pattern is commonly used in client-server interactions.
Usecase:
In a web application, a client (such as a browser) sends a request to a server (e.g., for user authentication). The server processes the request and sends back a response 
indicating whether the authentication was successful or not. This synchronous interaction ensures that the client receives the necessary information before proceeding.

## 3. Publish-Subscribe
The Publish-Subscribe pattern allows messages to be sent from publishers to multiple subscribers without the publisher needing to know who the subscribers are. 
This pattern decouples the message producers from the consumers, promoting scalability and flexibility.
Usecase:
In an e-commerce application, when a new product is added to the catalog, a publish-subscribe mechanism can notify multiple subscribers, 
such as inventory management, pricing services, and customer notification systems, ensuring that all relevant systems are updated without direct dependencies.

## 4. Message Queue
The Message Queue pattern uses a queue to store messages that need to be processed asynchronously. Producers send messages to the queue, and consumers read 
and process those messages at their own pace, allowing for decoupled communication.
Usecase:
In an online retail platform, when a customer places an order, the order details are sent to a message queue. Various consumers (e.g., inventory service, 
payment service, shipping service) pull messages from the queue to handle the order fulfillment process. This approach ensures that the system can handle 
varying loads without losing messages.

## 5. Scatter-Gather
The Scatter-Gather pattern involves sending a request to multiple services or components in parallel (scatter) and collecting the results (gather) to provide a unified response. 
This pattern is useful for aggregating responses from multiple sources.
Usecase:
In a search engine, when a user submits a query, the search request can be sent to multiple data sources or microservices (e.g., product database, user reviews, external APIs) 
simultaneously. Each service processes the query and returns results, which are then aggregated to present a comprehensive search result to the user.


# Answer 7 
- differences between ‘messaging’ and ‘conversation’ architecture
- difference between pub-sub and subscribe-notify