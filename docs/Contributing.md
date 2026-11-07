# Contributing
## Before contributing:
**READ THE [RULES](https://rules.ectf.mitre.org/about/index.html)** <br>
> Seriously Read The Rules.

Clone the repository and review the project documentation 

Verify that you can successfully build the project. The repository will strive to have a build process similar to the original [reference image instructions](https://rules.ectf.mitre.org/2026/getting_started/boot_reference.html)
any changes to the build instructions will be documented.

Review existing issues and select a task to work on.

Communicate with the team before beginning any significant changes.

New contributors are encouraged to begin with issues labeled good-first-issue or documentation.

# Development Workflow

We use a feature-branch workflow to manage contributions.

The reference branch is meant to be a read-only branch to track the progress of the "development" branch.

Create a seperate branch for any developments before pull-requesting it to "development". 

Despite poor naming, "development" should always compile and should not be directly changed.

Ensure your local development branch is up to date.

Make and test your changes.

Commit your work with descriptive commit messages.

Push your branch and open a pull/merge request.

Address and review feedback before merging.

Avoid making changes directly to development.
> Yes I could change the name, but you'll only see it on the 2027 Repo.

# Code Guidelines

Write readable, maintainable code. 

Handle errors and unexpected input appropriately.

Document complex or non-obvious behavior.
> A portion of the eCTF is proper and clear documentation, if you can't document it for us, then it won't be accepted by the organizers.

Avoid introducing unnecessary dependencies. 
> Consult with team via Discussion or Discord before adding any dependencies. 

Never commit secrets, private keys, or sensitive configuration data.


# Testing

Before submitting a contribution:

Verify that the project builds successfully.

Identify whether the changes were tested on physical hardware or emulation.

Document known limitations or unresolved issues.

If unable to test on hardware or emulator, please reach out on Discord for assistance.

# Pull/Merge Requests

Every pull/merge request should include:

A summary of the changes.

The motivation or associated issue.

A description of testing performed.

Any relevant implementation details or security considerations.

Security-sensitive changes may require additional review before being merged.

# Communication

Collaboration is encouraged. If you are unsure how to approach a task, encounter a problem, or want to propose a significant change, discuss it with the development team.

Communications are primarily handled in the computer club discord, and can also be posted to the Github Discussions page.

Questions are welcome, and contributors are encouraged to share what they learn.

# Questions:

Please direct any questions or issues to the DSU Computer Club eCTF Development Thread on Discord. 
