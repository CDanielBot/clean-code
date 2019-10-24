# clean-code
Clean Code Principles

Intro
- who do we write code for? for machines or for future people to understand?
- there is only one valid metric for code review: no of swears per minute (show image)

Clean Code Principles

General ones:
- SRP: Single Responsibility Principle: a module/class/function should have only one single reason to change
- DRY: Don't Repeat Yourself. Extract duplicate code to reusable functions/classes.
- KISS: Keep It Simple Stupid. Code should be very easy to read: almost in plain english. (choose proper names for functions, variables, constants, etc)
- YAGNI: You Ain't Gonna Need It. Don't write code that you think you might need in the future. Write the minimum to achieve your task.
- OCP: Open Closed Principle. A module/class should be Open to extensions and Close to modifications.
- SOC: Separation Of Concerns. You should keep your code flow clear, structured and separated by concerns. Eg: Don't mix data validation with saving the data to the DB.

More spefific ones:
- guardian statements + early returns: helps reduce the cyclomatic complexity and also the needed tests for a method.
- methods length: keep it small, smaller.
- passing parameters to methods: as few as possible (> 3 means SRP violation), no booleans (split instead in 2 methods)
- utilities classes
- DTOs: Data Transfer Objects
- Comments: should explain why something is needed not how it works. The code should explain the hows.
- Writing platform independent code. Eg: file path separators in Java instead of "/"
- Constants: use them for magic numbers & hardcoded strings,
- Avoid methods with side effects as much as possible: more like pure functions that operate on some input and return an output
- Avoid swtich cases in multiple places in code. If switch case is needed, keep it in one place. Eg: Factory Pattern.

How to refactor
- baby steps + often commits.
- don't try to refactor all at once: you will fail, miserably. Instead, try to take a big mess and make it smaller, one step at a time.

When to refactor
- on a daily basis: there is always room for small improvements
- don't be afraid to change the code in order to make it more readable. Put emphasis on the need of having good unit tests.
- be aware that too much refactoring can lead to too much abstractizations, which will make the code more harder to understand. Keep a fine balance between them.

What to refactor
- take some code from the project and try to apply the principles together with the team

Conclusion
- Continuous Refactoring: refactoring your code whenever you work on some feature/task.

Future discussion:
- null vs exception,
- concurrency & imutability
- low coupling & high cohesion
- architectural designs
