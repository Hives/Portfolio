# I can make anything
## I can refactor anything

### Reflect: What does it mean to be able to refactor anything?

- Understand why you refactor - improve code quality while leaving functionality unchanged. What does it mean to improve code quality?
  - Make code easier to modify or extend in future
  - Make code more readable
  - Make program flow more easily understandable
  - Reduce code complexity
  - etc...?
  - These points are not mutually exclusive
- Understand the value of TDD for refactoring - detailed and comprehensive feature and unit tests allow you to refactor in confidence that you aren't breaking anything

Tactics:
- Work in small steps, checking tests after every change
- SRP: If a class or method is doing more than one thing, break it up.
- Be careful about the responsibilities of your model, view and controller. Skinny controllers FTW. Presentational logic only in your views. (This is SRP again.)
- Code should be understandable without commenting. Choosing class and method names that accurately describe their responsbiity helps with this.
- Simplify conditionals. Consider extracting checks out into well-named (private?) predicate methods.
- Encapsulation: classes/objects should expose the minimal amount of information necessary to fulfill their function. Makes it easier to change later. Also minimises the amount of testing required.

### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

Three examples of good refactoring commits, stating what was done and why this was an improvement. Try and cover a broad range of improvements.

Gilded Rose!? 🤯

### Can you say this about yourself?

Yes

### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

#### Airport Challenge in Java

<https://github.com/Hives/java-stuffs/commit/08cbaa548aebbb963cf1ee7e98eda32daa15e831>

Refactored my Airport class's builder constructor to use an overloaded constructor. Much simpler construction, and an improvement in terms of readability and ease of change. It still involves adding a constructor method specifically for testing (so I can pass in my Weather double), but since Java doesn't have default arguments I think this is the best (only?) option.

#### Acebook

Refactored Jeremy's HTML/CSS for semantics and readability on Acebook. From [this](https://github.com/Hives/acebook-business-logic/commit/81dbbeba8ea21301d9fc6de030dbe2e83ec273f7) to [this](https://github.com/Hives/acebook-business-logic/commit/e5415ec11c9cb571240c4f8e13e31880ec08a815).

Refactored routes on posts controller to get the post author and recipient directly from the post, rather than making a separate database call to get them. Reduced the amount of logic in the controller, and reduced the responsibility of the controller methods. <https://github.com/Hives/acebook-business-logic/commit/2b27ebe4d44bf5a9c27c91c49147f72900c12616>

#### Chitter

Refactored one line of logic in my Chitter contoller into a method on the model: [Github commit](https://github.com/Hives/acebook-business-logic/commit/e5415ec11c9cb571240c4f8e13e31880ec08a815). Better from SRP point of view, and made the controller more readable.

Refactored a method in [this commit](https://github.com/Hives/chitter-challenge/commit/ade44edce177111e628643bfc33c73ed29841d29#diff-fb67188b0b305cc43fa91d3b80687e15) by choosing a more specific name for a variable holding the result of a database query (`allUsersWithUsername`).

I showed these to Alice and she said:
> "they are clear readability and extendibility (ease of change) improvements. ... hiding complexity in that other method makes it easier to change the code".