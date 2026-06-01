# New Machine Setup

This document describes the steps to set up a new machine for development.

Combine the contents of linux-setup and windows-setup into a singlke repo with both repo's contents superimposed over the same exact direvcotry strucutre.

## Requirements

- R1 User should be able to clone new-machine-setup repo and either call widnows-setup.bat on Windows platforms or setup-linux.sh on Linux platforms to complete a full setup of their machine for development.
R2- it hsould contain all features inthe set of the unoin of features form btoh repos.

- R3 The setup scripts should be idempotent, suppoort -Whatif, etc.
- R4 Duplicaiton of code should reduced to a miniumm, with shared code factored into common scripts where possible.
- R5 Both setups should be able to complete without error on Debian 13 and Windows 11 (with Powershell v >= 7.6 installed.)

- R6 Include options for installing powershell v7.6 via the initial setup ,bat and .sh scripts if not already present, to ensure the validation scripts can run on both platforms.. Make it idempotent, so if powershell is already present, it should skip the installation step and continue with the rest of the setup.
- R7 R6 superceds R5 by removing the prerequisite of having Powershell v7.6 pre-installed on the machine, by virtue of the setup scripts being able to install it if not already present.
