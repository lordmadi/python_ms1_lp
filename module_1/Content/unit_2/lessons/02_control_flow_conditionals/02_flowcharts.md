A flowchart is a visual representation of a process in a program, using various shapes, arrows, and symbols to illustrate the steps and decision points in a sequence of operations. It provides a clear and structured way to depict the flow of control in a system, making it easier to understand, analyze, and communicate complex processes.

## The Anatomy Of A Flowchart

Each shape in a flowchart represents a specific action or step, and arrows indicate the direction of the flow. Common flowchart symbols include:
- Rectangles for processes (steps)
- Diamonds for decisions (conditions)
- Ovals for the start and end of a process.
- Arrows for the flow of control between steps.

![flow chart conditionals only](//images.ctfassets.net/nbtht4kjx2t0/4T6jFTcsG8slT6PGzEOqyo/776004b49334c1f06cb8d56ef52eed25/flow_chart_conditionals_only.png)

The above flowchart represents the flow of a simple process of permission check to some service. The program checks the user age provided as input. If it is 13 or above, it grants the user access to the service. Else, display an "ineligibility" message and deny access to the service.

The program checked if the `age` is greater than or equal 13 using the ">=" operator. In programming, this is called a comparison operator. 

In the next concept, we'll discuss comparison operators in detail.

## Exercise

Draw a flowchart for the following process:

- A user inputs two numbers `a` and `b`.
  - If `a > b`, print number `a`.
  - If `a = b`, print a message "they are equal".
  - Else, print number `b`.

