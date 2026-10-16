Subject: details on the sim function block
From: Bruce Caslow <abcaslow@gmail.com>
To: Unitedwithcode <unitedwithcode@gmail.com>
Messages: 1

--- Bruce Caslow <abcaslow@gmail.com> (Sat, 10 Oct 2026 12:12:09 -0700) ---
No, not every Sim.ai Function block generates a result output. [1, 2, 3]

 - Executed branches: When a Function block runs normally, it produces
 standard outputs including <function.result> (the return value),
 <function.stdout> (console output), and <function.files> (files written
 to /tmp/sim/outputs). [1, 2, 4]
 - Unexecuted or branched paths: If a Function block is placed on a
 conditional branch or router path that is skipped during a workflow run, it
 does not execute and produces no output (referencing its tag returns
 empty). [3, 5]
 - Errors and exceptions: If a Function block throws an unhandled error
 or fails execution, downstream blocks cannot read a normal result unless an
 error handler or error path is explicitly configured. [6, 7]

[1] https://docs.sim.ai <https://docs.sim.ai/workflows/blocks/function>
[2] https://docs.sim.ai <https://docs.sim.ai/workflows/connections>
[3] https://docs.sim.ai <https://docs.sim.ai/workflows/how-it-runs>
[4] https://docs.sim.ai <https://docs.sim.ai/workflows/blocks/function>
[5] https://docs.sim.ai <https://docs.sim.ai/workflows/connections>
[6] https://docs.sim.ai <https://docs.sim.ai/workflows/blocks/condition>
[7] https://docs.sim.ai <https://docs.sim.ai/workflows/how-it-runs>
