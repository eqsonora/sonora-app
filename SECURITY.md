# Security policy

## Reporting a vulnerability

If you find a security problem in the Sonora app, the website eqsonora.com, the
account system, the phone remote or the AI assistant, **please report it
privately**. Do not open a public issue or discussion.

Use GitHub's private reporting: **Security -> Report a vulnerability** on this
repository. Only the maintainers can read it.

Please include:

- what is affected (app version, page or feature),
- the steps to reproduce it,
- what an attacker could achieve,
- if you have one, a proof of concept.

## What to expect

- An acknowledgement within a few days.
- An assessment, and a fix in a new app version or a site update, depending on
  severity.
- Credit in the release notes if you want it.

Please give us reasonable time to fix the problem before talking about it
publicly, and do not access, change or delete data that is not yours while
testing.

## Scope notes

- The app is currently **not notarised by Apple**. That is known and
  documented; it is not a vulnerability by itself.
- The AI assistant is designed on the assumption that the model can be fooled.
  If you find a way for it to do anything outside audio settings, or to exceed
  its gain ceilings, that is exactly the kind of report we want.
