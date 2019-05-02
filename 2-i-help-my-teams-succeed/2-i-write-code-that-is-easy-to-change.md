# I help my teams succeed
## I write code that is easy to change

### Reflect: What does it mean to write code that is easy to change?

- SRP: 'a class should only have one reason to change'. If this is true of your code it means knock-on effects of any change will be minimised, simplifying the process
- Encapsulation: only the minimum functionality of a class should be exposed, meaning it can be changed internally without affecting other parts of the code
- DRY: if you need to change something, you only want to change it one place.
- Naming: use names which reveal why something exists and what it does.
- Methods should be small - 5 lines is good, 3 lines is better. Refactor if they get too long.
- Use a linter to ensure code reads consistently
- Write detailed, comprehensive tests. This will allow yourself and others to change your code with confidence.

### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

Give examples (3?) of refactorings which improved the extensibility of my code.
Get feedback on two projects from coaches, asking them if they think the code is easy to change.

### Can you say this about yourself?

Yes

### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

#### Chitter

Refactored one line of logic in my Chitter contoller into a method on the model: [Github commit](https://github.com/Hives/acebook-business-logic/commit/e5415ec11c9cb571240c4f8e13e31880ec08a815). Better from SRP point of view, and made the controller more readable.

Refactored a method in [this commit](https://github.com/Hives/chitter-challenge/commit/ade44edce177111e628643bfc33c73ed29841d29#diff-fb67188b0b305cc43fa91d3b80687e15) by choosing a more specific name for a variable holding the result of a database query (`allUsersWithUsername`).

I showed these to Alice and she said:
> "they are clear readability and extendibility (ease of change) improvements. ... hiding complexity in that other method makes it easier to change the code".

### What feedback have you had?