# I can make anything
## I can debug anything

### Reflect: What does it mean to be able to debug anything?

To have a methodical approach to debugging that you can apply in any situation.

My process:
1. Read and understand what the error message is telling you
2. Follow the stack trace to find the point in your code that's giving you the error
3. Get visibility - dump out bits of context using Ruby's `p`, JavaScript's `console.log`, Java's `System.out.println()` etc.
4. Find what isn't what it should be
5. Follow the problem back in your code
6. Tighten the loop - investigate different points in your code to find two points between which the problem is arising
7. Repeat from point 3 until you've located the issue
8. Fix it

Other useful tactics:
- Comment out chunks of code and see if the issue is still happening - can use this to isolate the part of your code which is causing the problem
- Take a break, make a cup of tea, work on something else, get 10 minutes of fresh air... coming back to your code after a break you will sometimes see something glaring that you overlooked before.

### Plan: List evidence you aim to collect that would together show you have credibly achieved this goal

Exercises from the two debugging workshops. Document debugging process and ask coaches if they show a good methodological approach. 

### Can you say this about yourself? Yes / No

### Reflect: How does each of the following examples of your best work show evidence of achieving this goal? (e.g. Diode projects, Github repos)

### What feedback have you had?

I [documented my process when fixing two bugs](https://github.com/Hives/makers-notes/blob/master/week-1/workshops/debugging-workshop.md#3-apply-the-process) in Alice's debugging workshop in week 1. I showed this to Alice and she said:

> "I think you described the process well, and can definitely see that you get the debugging process."