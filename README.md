# Conductor

*Ariadne, whose thread led the way through the labyrinth*

Walks a procedure across a beamline one step at a time, and refuses a step
whose hardware another walk is already holding. It announces the whole step
list before it runs anything, reports each outcome as its step ends, and closes
the walk on the way out, so a walk that dies leaves behind the steps that
finished rather than nothing at all.

A client of keeper, not a part of it. Its core names no outside system: every
adapter is named once, at the entrypoint that picks it.

## Status

Nothing here yet. The code exists and runs, including against real hardware,
and is extracted here once keeper has moved and been renamed. Doing it in the
other order would mean renaming its configuration keys twice.

## The four

| Repo | Does |
| --- | --- |
| [keeper](https://github.com/open-cora/keeper) | Records what was proposed, run and produced |
| [conductor](https://github.com/open-cora/conductor) | Conducts a procedure across a beamline, one step at a time |
| [reporter](https://github.com/open-cora/reporter) | Reports what an acquisition engine did |
| [thinker](https://github.com/open-cora/thinker) | Proposes what to run next |

## License

Apache-2.0. See [LICENSE](LICENSE).
