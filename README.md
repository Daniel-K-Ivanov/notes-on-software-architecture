# Notes on Architecture and Patterns
In this repo you can find some useful notes on Software Architecture and design patterns that I stumbled upon that I think are worth writing down.

## Useful websites:

- Blog of Martin Fowler - [https://martinfowler.com/videos.html](https://martinfowler.com/videos.html)

## Tech Notes:

### Event-driven Architecture

([https://www.youtube.com/watch?v=STKCRSUsyP0](https://www.youtube.com/watch?v=STKCRSUsyP0)) 

- Events are generally used to reverse the dependencies between 2 systems. When we have events, we have a "thing" an object that we can talk about.
- The price paid on Availability is lack of consistency - a.k.a Eventual Consistency

### Microservices

([https://www.youtube.com/watch?v=wgdBVIX9ifA](https://www.youtube.com/watch?v=wgdBVIX9ifA))

- Don't get to microservices if you don't understand your module boundaries well

**Important Characteristics**
- Componentization via Services
- Organized around Business Capabilities
- Products not Projects
- Smart endpoints and dumb pipes
- Decentralized Governance
- Decentralized Data Management
- Infrastructure Automation
- Design for failure
- Evolutionary Design
- Choreography over orchestration

**Mandatory things for microservices:**

1. Rapid provisioning
2. Monitoring
3. Rapid Application Deployment
4. DevOps culture

**Netflix Principles:**
- Buy vs Build - use of-the-shelf-components; only build what you have to
- Services must be stateless (except for persistence and caching layers)
- Scale out instead of Scale up

**Good enough Architecture**:
- There is no good or bad architecture without context; architecture needs to take specific quality attributes into account
- Highly specific code is preferable to sophisticated configuration
- Small is not always beautiful
- Centralised responsibility hurts
- Lack of standartization leads to vast differences in API style, formats, documentation etc -> which creates needles extra work. 
- You cannot decide to not have architecture; if you don't actively create it, be prepared to deal with the one that emerges
- Extremely loose coupling requires very few rules, but they need to be enforced strictly
- Smart endpoints, dumb pipes (2) (Never put too much logic and too much inteligence in Infrastructure)
- Choose the simplest thing that will work <&> Create evolvable structures
- Manage your system's architectural evolution

**Common Failures of Sofware Architects**
1. Over generalisation drive -> Seeing commonalities in everything and turning them into generic solutions.
2. Over specialisation -> believing that your problem is unique although its solved 1000 times.
3. Unheathly complexity Attraction -> Being so smart, you can't be bothered by simple approaches.
4. Analysis Paralysis -> Taking longer to evaluate than to actually do it
5. Innovation Addiction
6. Severe tunneling fixation -> Enforcing an architectural approach that clashes with the framework, libraries you use.
7. Asset Addiction -> Becoming so attached to a particular tool/library/framework it becomes a fit for every problem
8. Exaggarated Risk Aversion -> Sticking to horrible tools
