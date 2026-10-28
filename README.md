# Match Pulse research tracker

Aggregate progress for Red Half Lab's private research into Liverpool form,
cards and match style. Target public release: Q1 2027, subject to review.

`status.json` is the dataset. Historical forward replays and prospective
locks/reconciliations are separate. Counts are by research track and must not
be added together as a number of distinct matches. Three-match windows overlap.
Historical model confidence is a probability assigned in that replay; it is
not a measured live success rate. For style, lower log loss is better, while
top-class hits may favour the baseline. Missing metrics mean unavailable.

No match forecasts, raw provider data, state scores, exact state errors, player
records, model weights, training inputs, local paths or credentials are included.
Only our aggregate status dataset and this documentation are intended to be
shared. This does not grant rights to third-party data or the private codebase.

Data licence: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
Attribution: Red Half Lab, Match Pulse research tracker, evidence timestamp in
status.json. Evidence time and controller heartbeat have different meanings.

## GitHub and model release plans

The public repository is [liv-ynwa/Matchpulse](https://github.com/liv-ynwa/Matchpulse).
It publishes dated snapshots of the verified aggregate research record.
Check the evidence timestamp in status.json to see how current a snapshot is;
this repository is not a continuous live feed.

We plan to open-source the models here once they are stable and have passed
review. Model code and weights have not been released yet. The Q1 2027 target
is an estimated product release date, not a guaranteed model release date.

## Maintainer updates

Generate an allowlisted export in the private research workspace, then publish
only README.md, LICENSE.txt, schema.json, status.json and SHA256SUMS. Never give
GitHub Actions access to private research artifacts or credentials.
The local development website reads the verified projection on demand.
A production build serves a dated snapshot; website deployment is separate
from updating this repository.
