# Microservice Design Playbook

In this playbook we have 18 section which help to reap most of the benefits of microservice.

## Section 1: Bounded Context

This is a strategic pattern to define boundary of a microservice. To understand bounded context, we need to
understand Domain Driven Design(DDD). 


The first term we should define here is domain, which is the business problem to be addressed, inclusive 
of the socio-technical environment in which a solution must exist. Thus, legacy systems, organization structure,
and business process are important elements of the domain. This fundamental embrace of systems thinking is what
makes the DDD community so intellectually rich and diverse. The domain is like core concepts, which contains
one or more concepts.

DDD implies domain decomposing into sub-domains, to ease their modelling and comprehension.The very fact that 
you run a business infers that there is at least one predominant business-value. The one you earn money with.
The one we started out our business for. So even if you do not know such a word like “Core domain”, it is still 
present. The same applies to sub-domains: probably you gonna need a bookkeeping, human resources, technical 
support — but it is secondary.

Then we define boundary of each core concept and divide our concept(sub-domains) between the core concepts, 
sometimes these concepts are much bigger so we can divide into other core concept and put the related concept in 
umbrella of it. Also sometimes in the boundary we found our core concepts contains a very small value or 
we have special requirements like reporting or performance improvement for the core concept then we also
aggregates multiple core concepts in one. 

The bounded context define a ubiquitous language between domain experts and developers so these domain and 
sub-domains are understandable by both of them, and this will build a better model to represent in both 
business and technical aspects.


## Section 2: Asynchronous Microservices

This is design level pattern to establish asynchronous communication between our microservices. In this section
we are going to learn why this required and how we can achieve this, we will also talk about 1-2 pattern to get
benefits of this and trade-off between them.

