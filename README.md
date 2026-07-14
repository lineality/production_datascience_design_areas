#### production_datascience_design_areas

### Production Data-Science Design Areas & Questions

# Connected areas:
- needs and goals evaluation
https://github.com/lineality/needs_goals_assessment_disambiguation 
- Project Areas https://github.com/lineality/project_areas_for_project_and_product_management 
- project-definition: definition behavior studies
https://github.com/lineality/definition_behavior_studies 
- coordinated decisions
https://github.com/lineality/Networked_Voting_and_Decisions_Including_One_Time_Pads 


# Production Data-Science Design Areas:

1. internal-use or external-use?

2. Local, On-Edge, Distributed, Networked, Cloud, Etc.

3. full end-to-end process or on-call tool?

4. stateless or stateful?

5. Latency more than 30-sec or not?

6. UI, API, CLI? 

7. Backend/Tech-stack requirements?

8. REST-ful endpoints?

9. "Serverless" or Servers?

10. Modular, Monolyth, or Micro-Service?

11. Scale and Scalability

12. Requirements of optima for optimization and efficiency

13. Rust vs. Python: If python is absolutely required, how?

14. Third Party Dependencies: If third party dependencies are absolutely required, how? 

15. Unit-Tests

16. User-Level Workflow-Tests

17. Test/Debug/Production Error-Case-Handling Separation Policy

18. Failure-Handling Policy

19. Security Considerations, e.g. pii-data

20. If databases are involved, myriad database design questions, e.g. No-SQL vs. SQL-Type.

21. Criticality of Feature/Functionality: see NASA's 2006 'Power of 10' and 2026-interpretations

22. CPU/GPU, Other

23. Atomics, Parallelism & Concurrency (including threads and workers) (e.g. avoid WSGI servers)

24. Servers: Myriad server design and selection questions, with custom Rust servers being more long-term maintainable.

25. Clear policies on communication, code-commenting, doc-strings, and documentation

26. Clear Project Area Definitions

27. Clear Needs and Goals evaluation BEFORE production-build.

28. Input and Output Sanitizing and Guardrails


# Generative-Model Specific Questions

1. local, batch, at-scale, cloud,

2. Output structuring and details of deployment
- self-hosted, 
- .gguf,
- hidden api-service
- specific api-services

3. Classic NLP, GOFAI, "Deterministic" approach, 

4. Crawling vs. large-chunk

5. Parallelization
- also for debugging

6. Language Choice
- third party dependencies

7. Third Party dependencies
- a serious and escalating liability
- See the 'where can be used' issue for pydantic + output_format structuring.

8. Full automation vs. semi-automating tool
- the fact that this dummy-project generates an unstructured text-field is suspicious, suggesting that this a solution in search of a problem, automatically and verbosely generating possibly useless and illogical documentation-word salad that some human being will manually need to inspect, as opposed to a tool designed to be used by a person for something more specific.

Small-Clear-Task-Doer: Good, Best
Big-automated-task-doer: Dubious, but can be good.
Task-Helper: Good, flexible.
Automated-Unchecked-Documentation-Generator: Very Bad. 

9. Definition, Testing, Evaluation, Benchmarking, Auditing:
Is something designed so that what it is doing is clearly defined in such as way that it can, effectively, be 
- unit-tested
- workflow-tested
- performance benchmarked (as in live month-to-month performance with potential changes to the system or to inputs)
- given a meaningful evaluation test (not a mismatched test, or a dubious or overly-indirect test)

10. Error logging and error/case handling 
- also gets into language choice

11. Atomics, Parallelism and Concurrency
- can it be optimized, does need to be
- debugging
- maintainability
- the project-scope and time required
- Language Rust vs. Python

12. scalability

13. maintainability

14. deployability
- on edge
- in a serverless endpoint
- consistently fast enough to be an endpoint under 30-sec. (backend-frontend latency, the need for 'step functions' etc.)

15. Design Maturity
Is the whole project/product design mature or is this a theoretical 'solution in search of a problem,' with hopes of a deployment and affordability pathway, and with a dream of maintainability? 

16. A case for a "Small" vs. "Large" Foundation model

17. Input data type ambiguity:
For document processing in real life this can be the most critical issue, yet it can be overlooked all the way until eventual project-collapse.

18. "Platform" and Hardware: Where will this be used and deployed?

19. Dependencies, Black-Box Services, & 'primative' tools
- It is probably broadly misunderstood that models are not the same as service-bundles:
-- input format and parts
-- output format
-- the loss of parameter setting



# Questions about Production Practices


1. Projects
A first introductory general question:

What project areas do you think are especially or most important?
https://github.com/lineality/project_areas_for_project_and_product_management 


2. Production
What Production areas do you think are especially or most important?
(link)
- third party dependencies
- maintainability of code
- policy on comments, doc-strings, 

3. Process
How do you handle:
- Errors
- Churn
- Misalignment
- Reporting issues within Agile (problems with project areas, e.g. standard predictable schedule problems)

4. Accountability, Communication and Contact
Basically a Whistleblower Question:
- Is there someone accountable to report to when process is not being followed?
(e.g. standard schedule breakdown areas)

5. 
- Explainability
- Reproducibility
- Testability, evaluation, benchmarks

6. 
- Managing structured and unstructured data
- Managing scope of decomposition and re-integration

