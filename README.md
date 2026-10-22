# Watchtower — downloads

A network vulnerability scanner for small businesses and the people who look after their IT. It
finds what is on the networks you're responsible for, what is exposed, and what is known to be
exploited, tells you what changed since last time, and writes the report. It runs on your Mac;
your scan results stay there.

**[Download the latest release →](https://github.com/0100-1010/watchtower-releases/releases/latest)**

- **Apple silicon** — `Watchtower-mac-arm64.dmg`
- **Intel** — `Watchtower-mac-x64.dmg`

macOS 12 or later. The two are not interchangeable: the Apple silicon build will not run on an
Intel Mac. Watchtower uses nmap, so install it first: `brew install nmap`.

A 14-day trial is built in, with everything on and no card. Licences are sold at
[pixel-labs.dev/watchtower](https://pixel-labs.dev/watchtower).

## First launch

Watchtower isn't signed with a paid Apple Developer certificate yet, so macOS won't open it the
first time. Open it once and choose **Done**, then go to System Settings → Privacy & Security and
click **Open Anyway** beside Watchtower. That's Gatekeeper doing its job, not a fault.

## Sensors

To scan a client's network from the inside, run a sensor there. The `watchtower-sensor-…` binaries
and the install files on each release are for that: Docker, Raspberry Pi, Debian or Ubuntu,
Windows and macOS. You don't need to pick them by hand: make a pairing code on the client's card in
Watchtower and it shows the one command to run on that kind of machine. Sensors only ever connect
outward, so nothing on the client's network is exposed. The sensor binaries aren't code-signed
either, so Windows may ask before running one.

## Only scan what you're allowed to

Use Watchtower only on networks you own or have written permission to test. It asks you to record
that permission for each target and puts it on every report.

## This repository

Downloads only. There is no source code here. Made by [PixelLabs](https://pixel-labs.dev).
