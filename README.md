# End Semester Examination, Set 2, Question 1
# Recover an Incorrect Shared Release Setting

**Total: 30 marks | Submit one PDF**

## Problem

An incorrect commit changed the shared release settings. A later documentation update is valid and must remain. Recover the correct setting without erasing published history, then review and integrate the recovery.

Starter: https://github.com/kalviumcommunity/endsem-release-recovery

Your assigned repository contains the complete starter history. Work only in that copy. Read RELEASE-POLICY.md. Change only release.env during recovery; do not edit README.md, RELEASE-POLICY.md or deployment-notes.txt.

## Requirements

Release environment must be staging and approval must be required. Keep the deployment checklist added by the later documentation commit. The original incorrect commit and the later valid commit must remain visible in history, with a new recovery commit. Do not reset or rewrite shared history.

## Task 1: Investigate the shared changes

Show clean main, current release.env and deployment-notes.txt, policy and commit history. Inspect the commit that introduced incorrect release settings and the later documentation change. Identify the incorrect commit and explain required final values and work that must survive.

Evidence: initial status, files/policy, history, both commit diffs and short explanation.

## Task 2: Prepare a safe recovery

Create a recovery branch from main. Inspect the incorrect commit's parent version of release.env and compare it with current values. Confirm the later documentation commit is present and the working tree remains clean before recovery. Explain why a new reversal commit is appropriate for published history.

Evidence: branch creation, parent/current comparison, later commit history, clean state and explanation.

## Task 3: Reverse and verify

Reverse only the incorrect settings commit using a history-preserving Git operation, not a manual replacement commit. Show the resulting recovery commit and its patch. Verify release.env satisfies policy, deployment-notes.txt still includes the later checklist, all original commits remain in history and working tree is clean. Explain how the recovery differs from deleting the original commit.

Evidence: actual reversal operation, recovery commit/diff, correct final files, retained history, clean status and explanation. No force push or destructive reset.

## Task 4: Review and integrate

Push recovery branch and open a PR into main in the same repository. Capture open state, title/direction and description covering incorrect change, recovery method, preserved documentation and checks performed. Leave an ordinary self-review comment confirming policy and preservation. Merge PR, pull local main and verify correct release values, retained checklist and clean state. Capture comment, merged state and local result.

Evidence: push, open PR/description/direction, actual self-review, merged PR, pull, final files and clean status. Self-review is not independent approval.

## Submission

Submit one PDF containing solutions for all four tasks. Organise it into Task 1 to Task 4. Include the screenshots requested in each task, with a one- or two-sentence label explaining the result and answering any requested short question. Multiple readable screenshots per task are allowed. Do not include credentials.

