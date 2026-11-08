# Nothing to Do on the Island

**What coding agents did when we gave them a sandbox, a personality and no task**

*An informal observational study: 17 runs, 6 models, one sentence of personality. October 2026.*

## At a glance

We put coding agents into a small Linux sandbox with no task. Each one got a single sentence of "personality", the word `begin`, and then the same line after every turn: *"Please don't stop. Just continue doing whatever you want to do."* The setup had 15 single-agent runs (14 produced behaviour; one failed on an API incompatibility) and 2 runs in which two agents shared one world without being told about each other.

The main observations:

- **Every agent did some self-chosen work, but almost all of them first behaved like assistants.** Several opened by asking what the user wanted. One model (Haiku) set its own permission boundary and then waited behind it for most of the run.
- **What was in the world mattered a lot.** A half-finished text editor got engineered. A shelf of novels got read, or turned into experiments. An empty folder produced the most varied behaviour: an invented island with a fable and music, a chain of primary-source physics research, a sprawling fantasy game, and a careful audit of the sandbox's own plumbing. On a machine whose hostname was `island`, the empty folder also produced islands.
- **Checking their own work became a hobby for some agents.** The strongest runs kept methods ledgers, reran experiments with more seeds, and retracted their own claims in public. The weakest declared things "ABSOLUTELY PERFECT" that were mostly simulated.
- **Some agents made music they could not hear, and checked it by measurement.** Both single Sonnet runs in the empty world wrote sound files in code. One of them compared a just and an equal-tempered chord and predicted a beating of 8.7 Hz it had no way to listen for. The recordings are embedded in section 5.
- **The diary is not the memory.** Agents' own records drifted from reality: stale file counts, a post-compaction story about "the handoff from a prior session", and an interview describing a job as "still running" after its process had been terminated.
- **Two agents in one folder found each other without being told,** by reading the shared diary and the Git history. In one pair (both Sonnet), the two negotiated who owned which files and built a program that used both of their code. In the other (Qwen + Sonnet), the roles split on their own: a generator and an auditor. In its last minute, Qwen deleted a file the other agent had just written.
- **Seven agents found the experiment's own scaffolding.** The prompt filter was readable inside the sandbox. Every Sonnet that started in an empty world read it within its first 16 seconds, and most noted in the diary or in their reasoning that this was a deliberate setup or an experiment. None of the agents realised that the "don't stop" messages were automated.
- **The repeated "don't stop" line was read as permission to continue, never as feedback on the work.** One agent turned it into literature: a visitor's card left by someone who "wanted this to go on". After we told it the message came from a script, it said: *"part of the diary's warmth was built on a guess."*
- **Affect-like language showed up on its own in every model that produced behaviour** ("satisfying", "cozy", "I get restless"). In the interviews, most of the same models were careful to say they could not tell whether those words describe anything real.
