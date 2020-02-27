Single purpose — each service should focus on one single purpose and do it well.

Loose coupling — services know little about each other. A change to one service should not require changing the others. Communication between services should happen only through public service interfaces.

High cohesion — each service encapsulates all related behaviors and data together. If we need to build a new feature, all the changes should be localized to just one single service.

# Comparison
![microservice-monolithic](/docs/imgs/microservice-monolithic.png)



# Solution Structure
![microservice](/docs/imgs/microservice.png)

Respect Failures Because They Will Happen

In a distributed environment, more things can fail, and they will. Failures of mission-critical services, when not handled well, could be catastrophic. We should always think about how to test failures and gracefully handle failures.
First and foremost, we should expect everything will fail at some point.

- For RPC calls, put extra effort to handle failure cases.
- Make sure we have good observability (mentioned above) to failures when they happen.
- Always test failures when bringing a new service online. It should be part of the new service check-list.
- Build auto-recovery if possible.


Avoid Microservice Syndromes from Day One

- Microservice is not a panacea — it solves some problems, but creates some others, which we call “microservice syndromes”. If we don’t think about them from day one, things can get messy fast and it costs more if we take care of them later. Here are some of the common symptoms.
- Poorly modeled microservices cause more harm than good, especially when you have more than a couple of them.
Allow too many different choices of languages/technology, which increase the operational cost and fragment the engineering organization.
- Couple running services with building services, which dramatically increases the complexity of each service and slow the team down.
- Overlook data modeling and end up with microservices with monolithic data storage.
- Lack of observability, which makes it difficult to triage performance issues or failures.
- When facing a problem, teams tend to create a new service instead of fixing the existing one even though the latter may be a better option.
- Even though the services are loosely coupled, lack of a holistic picture of the whole system could be problematic.



> Referência: https://medium.engineering/microservice-architecture-at-medium-9c33805eb74f