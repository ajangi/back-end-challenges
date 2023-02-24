## BackEnd Developer Challenge #2
#### Title :
Vacancies Challenge
#### Description: 
Dear Candidate,

This little puzzle was created in a way to give you maximum freedom, so you can show us the best of your expertise.
Roughly you will have **one day** to do it in.

##### The Task

We would like you to implement a simple REST API, which provides information about vacancies for positions of Software
Engineers and Team leads in European cities. The following user stories should be implemented:

1) As an API user, I need to get information about a certain position by its ID  
2) As an API user, I want to find all positions at a certain location (by country or by city) and be able to sort by
seniority level and salary (ascending order only)
3) As an API user, I want to get the most interesting position for a candidate with a certain set of skills.
 Also, provide a payload which will fetch the most interesting position for you from the endpoint.
  * Feel free to define any rules to find out if a candidate matches the position (for example, the candidate should be
    on a certain seniority level and have more than N% of requested skills)
  * Feel free to define an algorithm to verify "the most interesting position"

In the file [vacancies.csv](vacancies.csv) you can find data for your future API. Treat this file as a direct data source for the task, but think of how can you abstract the source.    
Keep in mind all vacancies are fake, and the currency SVU doesn't exists in reality.

##### The constraints

We kindly ask you to commit to the following points:

- The language of implementation: Feel free ti use any language you want;
- We firmly recommend you not to switch to another data source, such as mySQL, noSQL databases. Pls stick with a plain CSV
  file.
- Provide documentation. We expect to find at least following data in your README file:
   * We need to know, how to launch your application
   * We need to know the structure of your API
- Submission: please send us your code in a compressed format; we kindly ask you not to publish your implementation, to
  avoid online spoilers;

##### Boilerplate  

  Feel free to use any framework, create a Dockerfile or use no framework and docker at all. But be pragmatic
  and focus on user stories as our review will be mainly based on their implementation.

#### Our review

The review will focus on answering the following questions:

*Architecture*
  - How cleanly can you separate concerns in your code?
  - Does the code demonstrate a good grasp of design?
  - Will your code be easily extensible?
  - Are SOLID principles violated?
  - How good your models are designed? Do they make sense?

*Clarity*
  - Are your dox clear?
  - Is your code orderly and well-commented? Or is it so human readable that documentation would be redundant?
  - Does your code follow PSR coding style recommendations?
  - Does your solution contain any dead/redundant code (including parts of this skeleton)?

*Correctness*
  - Does your application get launch?
  - Does the application do what it promises?
  - Can we find bugs or trivial flaws?

*Testing*:
  - Is your code/application fully able to test?
  - Did you provide at least some tests? Are they green? Can you provide metrics about it?

We will also highly appreciate the following:

- Production readiness: did you provide a complete product that can be simply put to production?
- Scalability: is your application ready to face the challenge of a high-load? Or is it so lightweight it could be
  running on a Raspberry PI?

The following things most probably will not impress us:

- Over-engineering
- Implementing additional features

And finally let us give you advice, which practices should you avoid in your code:

- "Fat" controllers
- Using global variables
- Typos, grammar mistakes in a variable naming

*Good luck and have fun!*
