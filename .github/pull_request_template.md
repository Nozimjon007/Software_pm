<!--
TITLE   [RL-123] type(scope): short summary
        e.g. [RL-42] fix(booking): free a cancelled seat immediately
        types: feat · fix · refactor · test · docs · chore · ci · style · perf
        The Jira key in the title links this PR to its ticket.

Open as a Draft while you're still working, then click "Ready for review".
Acceptance criteria and test steps stay in the Jira ticket. Don't copy them here.
Delete any section that doesn't apply. Comments like this one don't show in the PR.
-->

## What & why
<!-- 1–3 sentences. Name the requirement IDs touched, e.g. FR-02, NFR-03. -->


**Jira:** RL-
<!-- Also fixes a GitHub issue? Add a line:  Closes #123 -->

## Risk map
<!-- Only the files worth slowing down on, as a small tree.   ⚠ = read carefully   ✎ = worth a look
     List your changed files with:   git diff --name-only main...HEAD

     Hot spots in RideLine:
       lib/services/app_state.dart          every screen rebuilds from it
       lib/data/mock_data.dart              the demo script depends on its sample data
       lib/services/compliance_service.dart legal driver-hour limits
       lib/services/invoice_service.dart    money, VAT, billing period
       lib/models/*                         data shapes used everywhere
       pubspec.yaml                         dependencies

     Example:
       lib/
       ├── services/
       │   └── app_state.dart          ⚠ cancelBooking() frees the seat after a delay, not instantly
       └── screens/
           └── bookings_screen.dart    ✎ snackbar text changed
-->
```text

```
**What could break / how to undo:** 

## Review checklist
<!-- 1. Request people in the Reviewers sidebar.
     2. Keep only the lines below that apply and delete the rest.
     3. The person named ticks their box when done. The PR list then shows "1 of 2 tasks",
        so everyone can see what's still open, and every tick is kept in the edit history. -->
- [ ] QA: @___ checked the acceptance criteria in the Jira ticket
- [ ] Discussed with the team before merging
- [ ] Second approval for a high-risk change: @___
- [ ] @___: please check ___
