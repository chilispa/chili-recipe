# Test-Driven Development methodology
<i>One must learn by doing the thing; for though you think you know it, you have no certainty, until you try. (Sophocles)</i>

## What is TDD?
Test-Driven Development is a misleading simple idea: <b>Write the test for code <i>before</i> writing the code itself.</b> 
This transforms the role testing plays in the development process and challenges our industry's assumptions about what testing is for.

With TDD, testing is no longer just about keeping defects from the users; instead, it's about helping the <b>team</b> to
understand the features that the users need and to deliver those features reliably and predictably.

TDD changes the way we develop our software and, in our experience, improves the quality of the systems we build,
in particular their flexibility in response to new requirements.

## How does it work?
TDD revolves around a short iterative development cycle that goes something like this:

![tdd-cycle](https://miro.medium.com/max/996/1*pP8Ks6tlt718jJg3fqrtvw.jpeg)

1. <b>RED</b>: Before writing any code, you must first write an automated test for your code. 
   The first time you run your automated test, the test should fail—indicating that the code is not yet ready.
2. <b>GREEN</b>: Afterward, you can begin programming. Since there's already an automated test, as long as the code fails it, 
   it means that it's still not ready. The code can be fixed until it passes all assertions.
3. <b>REFACTOR</b>: Once the code passes the test, you can then begin cleaning it up, via refactoring. 
   As long as the code still passes the test, it means that it still works. 
   You no longer have to worry about changes that introduce new bugs.
