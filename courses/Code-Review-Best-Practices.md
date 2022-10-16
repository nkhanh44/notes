
This is a takeaway after completing this cource [Code Review: Best practices](https://app.pluralsight.com/library/courses/code-review-best-practices/table-of-contents).

# 1. Why Code Reviews Exist

## Why?

- The later you catch a bug, the more expensive it is to fix. 
- It is practically a law that quality decreases as the software grows in size and complexity. If developers don't want their progress to grind to a halt, it is in their best interest to maintain code quality. 
- Review code before any official testing and even before the code is merged. Catch bugs.
- Code review is also a learning opportunity for the developer and the reviewer. It's meant to be a process that leads to a win-win situation, as well as an exchange of best practices and experiences. How to write better, cleaner code.  In essence, code reviews should serve you and your team to write better software.

## When Code Reviews Go Wrong

- There is a dark side to code reviews, however. Poor company culture, difficult personalities and unprofessional behavior may get amplified through code reviews as well. 

# 2. Establishing the Fundamental Processes for Code Reviews

## Apply Style Guides

- Some hot debates materialize out of thin air. Where to place the curly braces, the format of comments, and other miscellaneous things. One might argue that it doesn't matter.
- Let everyone commit using their own style. But consider this: imagine you are reading a book that doesn't have any punctuation at all.
- You don't have to invent anything; you can just reuse or tweak many of the existing style guides, like those by Google or Twitter. The important thing is to enable everyone to just import the style configuration in a few clicks and forget about it.

## Don't Waste Valuable Time

- Arguing about commenting on and fixing style issues is not time well spent. 
- Established style guides fix only part of this, but we can still make styling and similar mistakes, and someone needs to spot it, comment on it, and you need to fix it.
- Automation tools are perfect for this.

## Automate Static Code Analysis

- It's not just the spotting of style issues that can be delegated to tools.  A typical bug is an infinite loop. Standard bugs, security vulnerabilities, code smells and many others can be detected by static analysis tools.

## Have at Least Two Reviewers

- Two code reviewers is a reasonable number, but there's an important condition to this: **at least one should know the business logic behind the code**.
- It's important to have a second person who understands the domain and has looked at the requirements.

## Code Reviews Are Classless

- If you're a senior developer, encourage everyone to review your pull requests.
- Being the most senior person on the team does not imply that your code is perfect. If you're new to the team, don't be afraid to leave comments on things you think should be corrected.

## Accept That There Are Different Solutions

- If you're a reviewer, you might have your favorite solution, but the author's solution may also be valid. Distinguish between common best practices and your personal taste, and don't force your solution on the author if theirs is also fine.

## Don't Let the PR Hang for Days

- A code review should be done within hours. It shouldn't stay open for days.

## Wrap Up

- The less you spend on setting up the basic rules and processes, the more time and effort you will spend on each code review, and it accumulates fast. Try to have a second person on every major feature or component who at least knows the basics. 
- With the exception of most critical bugs, PRs shouldn't hang for three days or a week for whatever reason.

# 3. Submitting a Great Pull Request

- Not getting any comments PR after PR is not normal. Unless it's a trivial, one-line change like a property update, the default attitude should be to expect comments and improvement suggestions.

## It's Not Your Code

- You've spent several days writing it up, you gave it your best, and you're trying to contribute your code. **It's not your code, it's the team's code**.
- The team will be responsible for maintaining it, fixing it and refactoring it when necessary. 
- All of these points are reasons why the code you're submitting is the team's codes and that it will be collectively owned.

## Make Your PRs Small

- Make your PRs small
- Small PRs bring numerous benefits. They are easier to review, it's easier to spot bugs and issues, small PRs are also faster to fix if they get comments, and you get to deal with fewer merge conflicts
- A large PR is likely to make people reluctant to dedicate so much time to review your PR correctly.

## Split Changes into Commits

- It is possible and normal to split the changes that you are pushing into several commits.
- For example, implement a new DTO, or data transfer object class, in one commit. Refactor a function or a method that you need to handle that new class. And finally, update the function to handle the DTO that you created.

- You may have found a small opportunity to improve some code that isn't directly related to what you're doing. Ideally, you should make that part of a separate commit.

## Double-check Your Work

- If you like, take **a small break**, **come back to the code in 10 minutes**, and then review it, not only is it a best practice, but it's respectful towards your peers.
- Doing things right the first time is almost always cheaper and more efficient.

## Don't Explain Things in PR Comments

- Write code that is reasonably self‑explanatory.
- Add comments or documentation into the code itself so that they are permanently part of the code base and thus immediately available to read next to the code in question.

## Explain Things in PR Comments

- A comment may help reviewers understand why you're doing something in a particular way.
- What happened, Insight, PoWs in iOS - template.

## React to Every Comment

It is polite and professional to always reply to all comments before merging.

## Wrap Up

Coding is part of a lot of social interaction. As someone who creates code that other people should review, we have the responsibility to make code reviews smooth

# 4. Providing Effective Feedback as a Reviewer

## A Bad Example

- **Your implementation is wrong. What were you thinking? Redo it**
- It is a rhetorical question that adds nothing positive or constructive to the conversation

## Frame Feedback as Requests or Questions

- **Tip number one:** Frame feedback as requests or questions
- In fact, you should be slightly more polite because there is no voice
_Examples:_
- Don't say, "Rename this variable." Say, "Can you rename this variable?" 
- Don't say, "Move this method to another class." Instead, say something like, "Should this method be moved to another class?
We can make our first improvement to the initial example:
- Instead of "Break up this function into two smaller ones," you can say, "Consider breaking up this function into two smaller ones.

## Never Say "you"

- **Second tip**, never say you.

- You bring ego into the discussion by saying me or I. Try to replace you with either me, we or the code.
_Example:_
- Instead of saying _you need to write unit tests for this code, you could say, this code needs to be covered by unit tests_. After all, you're directing your comments at an objective thing, not the author. _Did you mean or can you please?_.

## Apply the OIR Rule

- **Next tip**, apply the **OIR** rule when giving feedback. OIR stands for **observation**, **impact**, and **request**.

_Example_: Imagine a function or a method that is 100 lines long. In this case, we can observe. "This function seems too long." We can explain the impact by saying, "This makes it hard for me to understand it." And notice we are making use of the previous tip and use "me" and focus on our own impressions. And finally request, the specific call to action. "I suggest to extract some parts into separate functions and give them expressive names."

_Example_: Here's another example. "This class seems to be misplaced. It would be hard for others to find it if they wanted to use it. Consider moving it to another package or directory along with such‑and‑such classes that logically belong together."

## Help with Code Examples Where Appropriate

- Help with code examples or concrete alternatives where appropriate.

- If it's simple, provide a concrete full example that they can _copy/paste_ or reuse most of it. Let the PR get merged, and then organize an upscaling workshop later.

- let the code get merged with a refactoring TODO, and then still organize an upscaling workshop.

## Don’t Try to Fix Everything

- Did you spot 10 unrelated minor things that could be improved? Suggest improving the most important 2 at most. And if the other issues bother you, create a refactoring follow‑up task.

## Use Labels

- If you want to ask for a _minor_ improvement, whether directly related to the PR or the surrounding code, it's a good idea to communicate that it's minor and it's not the end of the world if the reviewee doesn't accept the suggestion.

- **Prefix** your suggestion with nitpick or just nit or minor.

## Offer Sincere Praise

- Praise the author.
- Is the code of high quality? Give it a quick compliment. Say _well done_.

## Review Atomically

- Review everything and fully in **one go**.
- If you spot five issues, highlight them, allow the person to fix them, and then approve. If you happen to spot a critical issue in the next review iteration, sure, go ahead and comment some more
- Avoid changing your mind how the entire design could be improved through a major refactoring.
- The stress level increases with every iteration, and in practice => Another tip is to try and get all things fixed in _one or two iterations_, max.

## Don't Disappear

- Do not leave comments without willing to monitor for replies and fixes, and eventually approving.
- If you don't think you can complete a review in time, please let the committer know right away so they can find someone else.

## Wrap Up

- As code reviewers, we have a responsibility to provide constructive and helpful feedback.
- Don't block code until it's perfect - that's the wrong attitude. 
- Frame feedback as requests or questions. Apply the observe impact request rules where necessary, especially with junior colleagues who need more guidance.

# 5. Navigating Challenging Code Review Situations

## Build Trust and Relationships

- Build trust and relationships in your team.
- Chat to each other about life, discuss common interests and hobbies, go out for lunch together.
- If you're working from home, have occasional short virtual meetings that are not work related.
- You leave a comment on something minor, prefixed with nitpick, for example, and if you find nothing major, you go ahead and approve the PR and move on to other things, without having to come back to that PR, because you trust the reviewee to consider your comment and reply, and fix.
=> So when you build trust, your code reviews get much faster. As a reviewee, you accept feedback better, and you don't imagine it as something aggressive, because you had a nice chat with the other person just yesterday.

## Take Things Offline

- The initial comments by the reviewer, pushback, and then another pushback. The moment you notice this, consider taking things offline. If you are both in the office, a face‑to‑face talk is best.
- Whenever you come to an agreement, either the reviewee or the reviewer should then close the conversation on the pull request by saying as per our discussion with X offline, we decided to go for solution.

## Handling Difficult Reviewees and Reviewers

- Who blocks pull requests, someone unwilling to implement suggestions at all, makes the same mistakes over and over and refuses to learn, forcing the reviewers to leave the same comments trying to correct the same issues…->  _try to discuss one on one_ to gain the deepest possible understanding of the other person and find common ground -> If you can't come to an agreement, _seek an outside opinion_ ->  if you get two out of three, agree that X should be done, or three out of four are in favor of that other thing, then you go with the solution chosen by the majority -> If all else fails, escalate to a senior and let them handle it.

## Further Study

- Providing Quality Feedback path.
- Course Applying Feedback Sharing Techniques Effectively teaches specific feedback techniques.
- Debugging Teams: Better Productivity Through Collaboration.
