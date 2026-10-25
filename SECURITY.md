# Security policy

## What belongs here

This tap only holds Homebrew casks that point at release binaries published by other repositories. Report a vulnerability in a tool itself to that tool's repository, using its security policy. Report it here when the problem is the tap, for example:

- a cask whose download URL points somewhere other than the tool's own GitHub releases
- a `sha256` that doesn't match the published release asset
- a cask step (such as `postflight_steps`) that runs something unsafe on install

## Supported versions

Only the latest version of each cask on the `main` branch is supported. Run `brew update && brew upgrade rossedman/tap/<package>` to get it.

## Reporting a vulnerability

Do not open a public issue. Report it privately through GitHub's private vulnerability reporting:

**<https://github.com/rossedman/homebrew-tap/security/advisories/new>**

Include the cask and version, what an attacker could do, and how to reproduce it.

## What to expect

- An acknowledgement within 3 business days.
- A fix, or a plan with a timeline, within 30 days.
- Credit in the published advisory, unless you would rather stay anonymous.
