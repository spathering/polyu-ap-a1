# What Do I Need to Know When AI Writes the Code?

I did not exactly choose this programming course. It is a required part of PolyU's Innovative Multimedia Entertainment programme. I also did not arrive as a complete beginner: my undergraduate degree was in Computer Science and Technology, and most of my programming experience is with C-family languages. That makes the question *“Why are we here?”* more complicated for me. If AI can already write much of the code I need, what should I still learn from another programming course?

My answer depends on what kind of work is being made. For a simple design application, describing the intended result may be enough. A designer can let AI handle implementation and spend more time on visual, narrative, or interaction design. For games built around simulation, physics, and systems running in real time, however, implementation-level understanding remains part of the design practice. AI reduces the cost of producing code, but it does not remove the need to define a system, decide what matters, and judge what its behaviour means.

## Delegating Code Without Delegating Judgment

Over the past two years, AI coding tools have changed from merely usable to genuinely useful in my projects. In a recent Unity project, I delegated much of a procedural content generation tool to AI. I designed the data structures used to describe or bake the content and specified the intended result; AI then implemented the tool, including a large amount of mesh-data processing. I did not need to care about every internal detail. I inspected the surface appearance, the resulting mesh data, and whether performance was acceptable in actual use. Those were the properties that mattered to the work.

I used a similar division of labour for a workflow-management tool built around Yarn Spinner. After I established its data structures and responsibilities, AI handled implementation work such as the web-editor front end. These tasks were suitable for delegation because their scope, interfaces, and success conditions were relatively clear.

This does not mean that programming knowledge became irrelevant. Before implementation, my usual process is to let AI read the relevant code, analyse the requirement with me, discuss alternatives, agree on data structures and protocols, refine a plan, divide it into steps, and only then execute it. Afterwards, I test and optimise the result. The valuable skill is no longer typing every line myself. It is knowing how to turn an intention into boundaries and checks precise enough for another agent to implement.

## When Natural Language Is Not Precise Enough

My experiments with asking AI to build whole games have been much less reliable. As the context grows and gameplay requirements change, AI often loses relationships between systems. It also develops inertia: assumptions embedded in its earlier code influence later decisions, even when the design has changed. Several locally reasonable pieces can therefore form an inconsistent whole. Finding and repairing these problems may take more effort than writing the code myself.

This is especially important in the games I want to create: combat, sports, roguelikes, racing, and other experiences shaped by simulation, physics, and runtime interaction. In these systems, code or pseudocode can be a more concise design language than natural language. A sentence describing a movement “feel” may hide dozens of assumptions about state, timing, collision, and feedback. A small set of explicit rules can describe them with less ambiguity.

One recent game produced an unexpectedly powerful high-jump technique, strong enough to bypass parts of the level structure. I traced it to the timing logic around coyote time. I am currently keeping it for further playtesting rather than immediately removing it. The important question is not simply whether the code is correct. I must decide whether the behaviour damages the intended experience, deserves to become an advanced technique, or suggests a more interesting version of the level design. That is a design judgment made possible by understanding the running system.

## Learning a Medium, Not Competing With a Machine

In *The Art of Code*, Dylan Beattie presents programming as an expressive medium through examples including Conway's Game of Life, generative art, esoteric languages, and live-coded music. The Game of Life is especially relevant to games: simple rules can interact to produce behaviour that was not individually authored. Code can therefore be more than the hidden labour required to deliver a design; it can be the material from which unexpected design possibilities emerge (Beattie, 2020).

This does not justify teaching programming exactly as before. Memorising the syntax and tricks of one language may offer less value when AI can supply them immediately. Software engineering, system design, decomposition, validation, and the philosophy behind computation now offer a better return. AI may even help learners reach those ideas sooner by letting them build and test more examples.

I am therefore not here to compete with AI over who can produce code faster. I am here to understand the computational medium well enough to specify systems precisely, choose what to delegate, inspect what matters, and recognise when an accident becomes a possibility. For the kind of games I want to make, giving up that understanding would also mean giving up creative control.

## References

Beattie, D. (2020). *The art of code* [Video]. YouTube. https://www.youtube.com/watch?v=6avJHaC3C2U
