# release-sandbox

Permanent drill ground for [`codama-idl/release-tools`](https://github.com/codama-idl/release-tools): a miniature repository following the ecosystem release conventions, used to rehearse the cut → candidacy → promote flow before re-tagging release-tools.

- The dispatch wrappers deliberately reference `release-tools@main` (not a tag), so drills exercise the *next* version of the tooling.
- Never published to npm: no token is ever injected, and the scope is not ours — `changeset publish` failing at auth is the expected terminal state of every drill.
- History accumulates rehearsal majors; that is the point. Reset by deleting `N.x` branches (drop the ruleset first) and reverting `main` if a clean slate is ever needed.
