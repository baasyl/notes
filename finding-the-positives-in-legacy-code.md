# finding-the-positives-in-legacy-code

This is personal note about legacy-code and it's positive impacts.

## What is legacy code ?

- Code everyone hates and avoids to work on
- Platform/Infra it-self example an old/deprecated framework like WCF and it's not dotnet core / No K8S or Docker infrastructure and build pipeline is not complete CI/CD.

So in simple definition, Legacy code is the code which is way too old?

### Great code

Let’s work out in the opposite direction for legacy code, What's great code?

- Testable
- Tested
- Readable
- Maintainable
- Newer tech stacks

Above brings the definition of legacy code as the code that everyone is scared to change.

Let’s say, how can someone get joy working with legacy code ?

![dung-beetle, image credit: national geographic](images/dung-beetle.png)

No one wants to be a dung-beetle and wanting to push shit around all day?

But it’s all too easy to fall into this situation, like, if a method already takes 5 parameters, adding another one is all too easy or if the test is already written for one method/end to end scenario(journey test) then it’s too easy to copy pasta the same and change values without understanding it.

Basically it’s too easy to become a victim of [Stockholm syndrome](https://en.wikipedia.org/wiki/Stockholm_syndrome).

So, how to transform from a dung beetle into someone who enjoys the challenges of legacy code?
(_Side note: Dung beetle teaches us How to deal with obstacles and stay focused on the mission._)

### How to overcome legacy challenges?

Let’s establish some basics to overcome legacy challenges

- Having CI/CD
- Tests to increase our confidence
- Fast feedback
- Easy onboarding for new members

All of the above is really hard, the cost of getting a first test written for legacy code base is sometime high in terms of investing time - means someone is destined to forever be pushing that dung around.

#### What’s in the legacy code to love about?

- Code is the biggest asset about legacy code - It might be messy but it's working and there’s gold buried (business logic) in there.
- Mining the code base - we will learn more interesting things
- Often we think instead of understanding the existing code, it’s too easy to rewrite a particular class or module (and in some cases changing the whole architecture) but sometimes (many) rewrites often miss out the edge cases and strange behavior that's captured in legacy systems. Example Netscape 6.0, [They decided to rewrite the code from scratch.](https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/)
- In addition to the code base, version control systems can reveal lots of other details such as which files have changed the most and least? Helps to guide decisions such as which parts of the system are worth getting under test first.
- Biggest advantage is the rate at which we can learn new techniques.
  - Package hell (All dependencies and their dependencies and more dependencies)
  - Patterns in Code
  - Any in-house developed tools
  - Infrastructure deployment and more knowledge on cloud services.
  - Rather than writing a new code, you able to read the code.
  - Learning many downstream/upstream services.
  - Artifactory and package building
- Learning the Impact of the mistakes
  - Such as not regularly updating dependencies
  - Complexity of real business applications (helps in exploratory testing)
  - If the code is old and running successfully means it is well covering all (most) edge cases

##### References

My notes are taken mainly from the below references.
- https://medium.com/ingeniouslysimple/learning-to-love-legacy-code-e5e5459dd2eb
- https://www.joelonsoftware.com/2000/04/06/things-you-should-never-do-part-i/
- https://prezi.com/qe7_jln7mzff/learning-to-love-legacy-code/
