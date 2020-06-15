# Hindsight Experience Replay
## Marcin Andrychowicz, Filip Wolski, Alex Ray, Jonas Schneider, Rachel Fong, Peter Welinder, Bob McGrew, Josh Tobin, Pieter Abbeel, Wojciech Zaremba

* OpenAI, NIPS 2017
* Basic idea: Use experience from not just the current coal but multiple goals
* This is essentially off-policy experience replay
* Avoids reward engineering, by maintaining the overall sparse reward structure.
* Speculation on why this works - you still learn how to get to interesting states
* TLDR always use multi-task learning instead of single task. HER can be thought of as *implicit curriculum learning*
