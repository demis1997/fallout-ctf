# fallout-ctf

Educational Solidity Fallout CTF example of unsafe ownership initialization.

## Source and reproduction

Inspected Solidity: `fallout.sol`. Contracts include `Fallout`. Source compiler pragmas: `^0.6.0`.

No complete pinned compiler/dependency build harness was found in the inspected files. Import resolution and automated execution are unverified; an isolated local test harness is required before running the example.

This is a prototype/security-study example. Do not interpret the source as audited production code or execute it against third-party deployments. No on-chain transaction was performed.

No repository-wide license file was found; no license has been assigned by this maintenance change.

## Existing notes and attribution

# fallout-ctf
my solution for a fallout ctf
This CTF took 4 minutes to solve, simply look at the code and notice which function is made public. That's right "owner = msg.sender;
    allocations[owner] = msg.value;"
