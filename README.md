# What Do I Need to Know When AI Writes the Code?

I did not exactly choose this programming course. It is a required part of PolyU's Innovative Multimedia Entertainment programme. I also did not arrive as a complete beginner: my undergraduate degree was in Computer Science and Technology, and most of my programming experience is with C-family languages. That makes the question *“Why are we here?”* more complicated for me. If AI can already write much of the code I need, what should I still learn from another programming course?

My answer depends on what kind of work is being made. For a simple design application, describing the intended result may be enough. A designer can let AI handle implementation and spend more time on visual, narrative, or interaction design. For games built around simulation, physics, and systems running in real time, however, implementation-level understanding remains part of the design practice. AI reduces the cost of producing code, but it does not remove the need to define a system, decide what matters, and judge what its behaviour means.

## Delegating Code Without Delegating Judgment

Over the past two years, AI coding tools have changed from merely usable to genuinely useful in my projects. In a recent Unity project, I delegated much of a procedural content generation tool to AI. I designed the data structures used to describe or bake the content and specified the intended result; AI then implemented the tool, including a large amount of mesh-data processing. I did not need to care about every internal detail. I inspected the surface appearance, the resulting mesh data, and whether performance was acceptable in actual use. Those were the properties that mattered to the work.

This does not mean that programming knowledge became irrelevant. Before implementation, my usual process is to let AI read the relevant code, analyse the requirement with me, discuss alternatives, agree on data structures and protocols, refine a plan, divide it into steps, and only then execute it. Afterwards, I test and optimise the result. The valuable skill is no longer typing every line myself. It is knowing how to turn an intention into boundaries and checks precise enough for another agent to implement.

## When Natural Language Is Not Precise Enough

My experiments with asking AI to build whole games have been much less reliable. As the context grows and gameplay requirements change, AI often loses relationships between systems. It also develops inertia: assumptions embedded in its earlier code influence later decisions, even when the design has changed. Several locally reasonable pieces can therefore form an inconsistent whole. Finding and repairing these problems may take more effort than writing the code myself.

This is especially important in the games I want to create: combat, sports, roguelikes, racing, and other experiences shaped by simulation, physics, and runtime interaction. In these systems, code or pseudocode can be a more concise design language than natural language. A sentence describing a movement “feel” may hide dozens of assumptions about state, timing, collision, and feedback. A small set of explicit rules can describe them with less ambiguity.

One recent game produced an unexpectedly powerful high-jump technique, strong enough to bypass parts of the level structure. I traced it to the timing logic around coyote time. I am currently keeping it for further playtesting rather than immediately removing it. The important question is not simply whether the code is correct. I must decide whether the behaviour damages the intended experience, deserves to become an advanced technique, or suggests a more interesting version of the level design. That is a design judgment made possible by understanding the running system.

## Learning a Medium, Not Competing With a Machine

In *The Art of Code*, Dylan Beattie presents programming as an expressive medium through examples including Conway's Game of Life, generative art, esoteric languages, and live-coded music. The Game of Life is especially relevant to games: simple rules can interact to produce behaviour that was not individually authored. Code can therefore be more than the hidden labour required to deliver a design; it can be the material from which unexpected design possibilities emerge (Beattie, 2020).

This change has happened before. Literature, painting, and film have all been reshaped by new tools. Within computing, high-level languages hid machine instructions, while the history of the [game engine](https://en.wikipedia.org/wiki/Game_engine) is largely a history of reusable abstractions. Unity says its editor helped democratise game development, and Unreal's Blueprints let designers create behaviours without writing conventional code (Unity Technologies, 2023; Epic Games, n.d.). These tools let more people concentrate on content instead of rebuilding physics, graphics, and system I/O.

Yet abstraction did not make lower-level knowledge worthless. It gives experienced developers more freedom when standard tools do not fit. That matters in sandboxes, RTS games, hard simulations, factory systems, and puzzle games, where unusual technical ideas can become the main experience. Jonathan Blow's Jai is a striking example. Built from his experience as a game developer and programmer, it supports arbitrary compile-time execution. An early demonstration even ran a small game during compilation and baked its results into the final program (Blow, 2014). The game was not generating itself during normal play; the surprising idea was that compilation itself became programmable.

This does not mean programming should be taught exactly as before. Memorising one language's syntax matters less when AI can supply it immediately. Learning a tool also means learning its history, the situations it was made for, and the ideas previous users built into it. I am not here to compete with AI over typing code. I am here to understand the medium well enough to specify systems, choose what to delegate, inspect what matters, and turn technical possibilities—or accidents—into differentiated play. For the games I want to make, giving up that understanding would mean giving up creative freedom.

## References

Beattie, D. (2020). *The art of code* [Video]. YouTube. https://www.youtube.com/watch?v=6avJHaC3C2U

Blow, J. (2014). *Demo: Base language, compile-time execution* [Video]. YouTube. https://www.youtube.com/watch?v=UTqZNujQOlA

Epic Games. (n.d.). *Create next gen games for next gen consoles, PC & all platforms*. Unreal Engine. https://www.unrealengine.com/nextgen

Unity Technologies. (2023, March 21). *Why we're excited about AI at Unity*. https://unity.com/blog/news/why-we-are-excited-about-ai
    
Wikipedia contributors. (2026). Game engine. In *Wikipedia*. Retrieved September 10, 2026, from https://en.wikipedia.org/wiki/Game_engine
   