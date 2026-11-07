
# DSU eCTF Practice Development Environment.
This repository is meant to function as a sandbox before the main competition. <br> 
The goal is work out any kinks found in the development workflow as well as getting contributors/competitors on the same footing before the main competition starts.


# Communication
Communication is primarily handled through the embedded-security channel under the Interest Groups section of the DSU Computer Club. If you cannot see the channel, navigate to **Channel & Roles -> Browse Channels** and search for **embedded-security** and flip the switch to enable it. 
### Issues
Issues are meant to document tasks, starting points, and considerations for developing the firmware. Anyone is free to add an issue, but it is encouraged to check before hand that you are not repeating an issue before submitting.

### Discussions
GitHub discussions are used for more longform discussions and should include things such as documentation, research findings, and other posts that are not directly related to a code issue. Please feel free to post relevant topics as any discussions made will benefit future competitors.

# Building Firmware
Current build instructions match the reference image's instruction, found [here](https://rules.ectf.mitre.org/2026/getting_started/boot_reference.html). If build process changes, please edit this documentation.
> Good first task to rewrite/streamline the build instructions.

# Contributing
Contributions are welcome from all development team members, regardless of experience with embedded systems or the eCTF. Our goal is to encourage collaboration, maintain code quality, and provide opportunities for members to learn throughout the competition. <br>
**BEFORE ALL ELSE READ THE [RULES](https://rules.ectf.mitre.org/about/index.html)**

## Finding a Task
There are a wide variety of ways to contribute the eCTF, not all of them involve directly contributing the firmware source code. If you're unsure where to start **READ THE RULES** and then look at the [**Issues**](https://github.com/DSU-DefSec/2026-eCTF-PracticeDev/issues/) and see if there is anything that interests you. Additionally feel free to ask the embedded-security Discord for any tasks that may need to be done.
### Contributing Code
Please reference the [Contributing](./docs/Contributing.md) before making any pull requests
### Example Non-Coding Roles: 
Please reference [Low-Code](./docs/Low-Code.md) for a list of roles that require less direct programming contributions.


# Key References 
[2026 eCTF rules](https://rules.ectf.mitre.org/about/index.html) - The rules and where this repo was sourced, read them, understand it, and ask questions. This is mandatory reading for being apart of the team. 

[LP-MSPM0L2228](https://www.ti.com/tool/LP-MSPM0L2228) - Documentation for the launchpad board. While not the actual board used in the competition, this is the commercial analogue and has a lot of simularities.

[Base Build Instructions](https://rules.ectf.mitre.org/2026/getting_started/boot_reference.html) - Build instructions for the base reference image. Follow it build firmware.

## Layout
`firmware/` - Source code to build the firmware
    - `Makefile` - This makefile is invoked by the eCTF tools when creating an HSM.
    - `Dockerfile` - Describes the build environment used by eCTF build tools.
    - `secrets_to_c_header.py` - Python file to convert from global secrets to firmware-parsable header file
    - `inc/` - Directory with c header files
    - `src/` - Directory with c source files
    - `wolfssl/` - Location to place wolfssl library for included Crypto Example
    - `firmware.ld` - Defines memory layout of built firmware
- `ectf26_design/` - Pip-installable module for generating secrets
    - `src/` - Secrets gen source code
        - `gen_secrets.py` - Generates shared secrets
    - `pyproject.toml` - File that tells pip how to install this module
- `docs` - Assorted documentation
- `Makefile` - Helper script to simplify repetitive build steps

> Please reach out to yen.fan@trojans.dsu.edu if you have any issues or questions.