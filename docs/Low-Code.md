# Getting Started

Not everyone needs to make a code commit to contribute. This page lists some example roles that can help contribute.

> [!NOTE]
> Read the Rules. Really. Read the Rules. It'll help you figure out where you fit in and almost all these roles require it. <br>
> They can be found [here](https://rules.ectf.mitre.org/about/index.html), go there.

## Documentation Maintainer
 Maintain onboarding materials, technical documentation, and explanations of the project's components.

<details>
<summary><h3><strong>Role Details & Guidelines</h3></strong></summary>

### Example Tasks:
- Document how to build the firmware.
- Write a Git tutorial. 
- Explain a module's purpose.
- Improve confusing setup instructions.
### Impact:
The eCTF directly rewards/requires good documentation of the project, but also the team also benefits from clear documentation in order to onboard hands and operate cohesively. 
### Guidelines:
- Read [`docs/Contributing.md`](../docs/Contributing.md) and follow the same branch/pull request method of contribution as contributing code 

- Please place documentation inside the `docs/` folder. 

- Documentation should be written in a `.md` or markdown file.  

- Documentation can also be placed in Github Discussions, but it's recommended that a `.md` copy be added to `docs/` as well.

</details>

## Secure Designer 
Help design secure firmware by identifying potential security risks, proposing technical specifications, and documenting security requirements before implementation.

<details>
<summary><h3><strong>Role Details & Guidelines</h3></strong></summary>

### Example Tasks: 
- Propose security requirements for individual firmware components.
- Develop threat models identifying potential attack surfaces and trust boundaries.
- Evaluate proposed designs and identify security tradeoffs.
- Define expected security behavior for developers to implement and testers to verify.
- Research relevant security practices and recommend their application to the project.

### Impact:
Helps developers make informed security decisions early in development, reducing the likelihood of architectural vulnerabilities and costly redesigns. Provides clear security specifications that guide implementation and testing.
Sugguest 
Review code and do security research. Please document findings and weak point considerations for the team. Suggest fixes, but do not just rely on agent code reviews, we are already doing that.
Review previous Year's 

### Guidelines:
- Focus on design, not just code review. Identify potential weaknesses in the system's architecture, assumptions, and intended behavior.

- Make recommendations actionable. Specify what the system should guarantee, rather than simply recommending that it be "secure."

- Consider constraints. Account for hardware capabilities, memory limitations, performance, and development complexity. Simple is generally better.

- Explain your reasoning. Document the risks being addressed, proposed mitigations, and relevant tradeoffs.

- Collaborate with developers. Discuss proposals before implementation and be open to alternative solutions.

- Define verifiable requirements. Whenever possible, describe how the proposed security properties can be tested.

Use research and AI tools critically. AI-generated assessments may assist research but should not substitute for independent reasoning or evidence.

</details>

## Technical Researcher
Investigates unfamiliar technologies and produces concise, actionable research notes for developers.

<details><summary><h3><strong>Role Details & Guidelines</strong></h3></summary>

## Example Tasks:
- Research Hardware capabilities

- Explain a crytographic API (Point out specific functions, patterns, or code snippets)

- Investigate odd hardware behavior

- Compare approaches to persistent storage

## Impact:
Investigates the weird and obscure parts of the system and draws in as much context as possible to help the team stay up to date and aware of security considerations.

## Guidelines:
- Please post findings to the [Discussions](https://github.com/DSU-DefSec/2026-eCTF-PracticeDev/discussions) pages.

- Try to document sources for extended research.

- Try to keep it pertinent. 
> We're all nerds, but attention span is a precious commodity.
- Don't rely on AI summaries. 
> Don't make me read AI summaries, they are very long and it defeats the point of taking this role.
 

</details> 


--- 

#### Template for adding more roles.

```
## Role Name
Oneline Description

<details>
<summary><h3><strong>Role Details & Guidelines</strong></h3></summary>
## Example Tasks:
Short list of things one can do

## Impact: 
How the role contributes to the eCTF Team

## Guidelines:
Guidelines on how to perform the role.

</details> 
```

