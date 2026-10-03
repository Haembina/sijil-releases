<p align="center">
  <img src="icons/icon.png" alt="Sijil logo" width="128">
</p>

# Sijil — downloads

The Windows installers for [Sijil](https://github.com/Haembina/Sijil), and
nothing else. **There is no source code in this repository.** Every file here is
build output, published by the release workflow in the source repository, which
is private.

## Getting it

The permanent link always resolves to the newest release:

```
https://github.com/Haembina/sijil-releases/releases/latest/download/Sijil-x64-setup.exe
```

Each release also carries the same installer under its version number, an MSI
for anyone who prefers one, and `latest.json` — the version, the download URL
and a detached signature that an installed copy checks before it accepts an
update.

## What the signature is, and is not

The `.sig` beside each installer is an **updater** signature. A running copy
verifies it against a public key compiled into the app, which is what proves an
update came from this pipeline and from nowhere else.

It is **not** an Authenticode certificate. It identifies no publisher to
Windows and earns no SmartScreen reputation, so a fresh download shows an
unknown-publisher warning until a code-signing certificate exists.

## The app

An offline, encrypted, Arabic-first psychiatric records app. It works on a
machine that has never touched a network: no CDN, no remote font, no analytics,
no telemetry, no licence check.
