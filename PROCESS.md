# Process

This file records how I developed Assignment 1 and how I used AI during the process.

## Work Log

### 6 September 2026: Initial setup and discussion

- Created `PROCESS.md` and confirmed that the final essay would be written in the repository's `README.md`.
- Used ChatGPT/Codex to read the assignment brief and ask me questions about my position, game-development background, and experience with AI-assisted programming.
- Organised my answers in the local working file `.midwork/assignment1/ASSIGNMENT1_DRAFT.md`. At this stage, no English essay had been generated.
- Kept the suggestion to structure the essay around the difference between simple design applications and tightly coupled real-time game systems. This reflected my actual experience more accurately than discussing whether AI will replace programmers in general.


### 6 September 2026: Developing personal examples

- Used further questions from ChatGPT/Codex to identify concrete examples from my work: a Unity procedural content generation tool, a Yarn Spinner workflow editor, experiments in asking AI to build whole games, and an unusually high jump caused by coyote-time logic.
- Kept the AI-proposed contrast between delegating clearly bounded modules and retaining more human control over cross-system work. I kept it because it accurately describes how I decide whether using AI will save time.
- Rejected the suggestion to explain the exact trigger for the high-jump technique. The game will later be playtested by my professor, so disclosing the method could affect that experience. The behaviour remains in the game for now and will be evaluated later.
- Defined my checks for the AI-generated PCG tool as surface appearance, mesh data, and acceptable performance in actual use. I do not inspect unrelated implementation details when these project-specific criteria are satisfied.

### 6 September 2026: First English draft

- Used ChatGPT/Codex to turn the confirmed Chinese outline into the first English draft of `README.md`.
- Kept the high-jump example but removed the triggering steps. It remains useful because it shows the difference between technical correctness and deciding whether an unexpected behaviour is a bug or an emergent mechanic.
- Framed “understanding programming” as being able to define system boundaries, choose relevant checks, and judge runtime behaviour—not as reading every line of AI-generated code.
- Did not use Jai as a formal example in the essay. Its technical details would require more verification, and it distracted from the stronger examples drawn from my own practice.
- Reviewed the first draft and found its overall argument and structure consistent with my position.

## AI Use Summary

I used ChatGPT/Codex for:

- reading and extracting the assignment requirements;
- interviewing me to clarify my position and personal examples;
- organising my answers into an outline;
- researching and checking a potentially inaccurate reference;
- drafting and editing the English essay;
- checking the word count and Markdown structure.

One AI contribution I kept was the distinction between **delegating implementation** and **delegating judgment**. It was useful because it connected my successful use of AI for bounded tools with my reluctance to use it for tightly coupled game systems.

One AI contribution I rejected was the suggestion to describe the high-jump technique in technical detail. I rejected it because the specific mechanism is not necessary for the argument and could influence a future playtest. I also left the Jai example out of the essay because the initial description of its behaviour was not sufficiently verified.

### 10 September 2026: Historical context and Jai

- Decided to add Jonathan Blow's Jai as a supporting example after further research. I wanted to connect the language to Blow's experience as both a game developer and programmer, and to the idea that learning a tool includes learning its history, intended situations, and inherited ideas.
- ChatGPT/Codex checked the original Jai demonstration and a newer presentation. We corrected my initial description: the demonstration ran a small game **during compilation** and baked its results into the program; it did not show a complete game generating itself during normal gameplay.
- Added the development of high-level languages and commercial engines as historical parallels to AI abstraction. Unity and Unreal allow developers to produce strong results without first implementing physics, rendering, or system I/O, but this has not removed the creative value of understanding those layers.
- Kept the examples of sandboxes, RTS games, hard simulations, factory systems, and puzzle games because they show where deeper technical freedom can produce differentiated gameplay.
- The earlier decision to omit Jai applied only to the first draft. I later reversed it after verifying a narrower and more accurate claim.
- Removed the Yarn Spinner example from `README.md` after the historical section pushed the essay slightly over 1,000 words. The Unity PCG example already supports the same point with more relevant technical detail.
