# R.U.N.E.
## A visual command center for AI-assisted development
**Realm-based Unified Network of Executors** · Independent project · Active development

[Back to Sean's profile](../README.md) · [Portfolio](https://seansteuer.com)

### The problem

When development work spans multiple repositories and AI agents, it becomes difficult to see who is doing what, which tasks are blocked, and what evidence supports a reported result. Chat transcripts and disconnected dashboards make that context hard to follow.

### The approach

R.U.N.E. represents projects as realms and agents as characters in an interactive, isometric world. Stations represent development activities. The interface connects that visual layer to inspectable development state rather than treating animation alone as evidence of progress.

The dark-fantasy presentation is an interaction-design experiment: make orchestration understandable while retaining access to the underlying work.

### Documented capabilities

- A central hub and project realms with navigation and interactive panels.
- Agent roles, messages, handoffs, and activity represented in a shared world.
- Optional read-only access to local agent transcripts, with scrubbing, to expose delegation prompts and reports.
- Session recording and replay, explicitly labeled as replay.
- Local telemetry integrations, with unknown states when an optional source is unavailable.

These describe the repository documentation reviewed for this overview. They are not a claim that arbitrary tasks run autonomously or that the system is enterprise-ready.

### Architecture

| Layer | Responsibility |
| --- | --- |
| React + PixiJS interface | Interactive world, project navigation, and inspection |
| Local Node service | Connect the interface to local development information |
| Shared TypeScript contracts | Consistent representation of system state |
| World-state reducer | Agent activity, messages, handoffs, and meetings |
| Navigation and realm themes | Movement, project environments, and scene layout |
| Session recorder | Capture activity for clearly labeled playback |

### My contribution

I define the product vision, interaction model, agent responsibilities, and acceptance criteria, and build the system using AI-assisted development tools. My focus is on making delegated work observable, keeping claims tied to evidence, and testing whether the interface helps a person understand and direct the work.

### Design decisions

**Observed versus inferred activity:** transcript-backed details and inferred handoffs need distinct treatment so a visualization does not imply evidence it lacks.

**Replay versus live execution:** a replay must be recognizable as a recording.

**Missing data:** unavailable telemetry should show an unknown state rather than a fabricated success.

**Separate interface from state:** shared contracts and a reducer help keep the visual representation consistent with the underlying events.

### Current boundary

R.U.N.E. is an independent system in active development. The implementation remains private. This overview contains no source code, local transcripts, credentials, or employer material. A recorded demonstration is not included in this version.

For a project conversation, contact [Sean Steuer](mailto:sean@steuer.com).
