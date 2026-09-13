# Alatheya friend playtests

This public repository contains verified Windows friend-playtest downloads for **Alatheya**. The game source,
development history, and private operational material are not distributed here.

## Download the latest build

Open the [latest release](../../releases/latest), download **AlatheyaLauncher.exe** once, and run it whenever
you want to play. The launcher checks the latest immutable release, downloads every package part only when an
update is needed, verifies GitHub and manifest SHA-256 digests, installs the build in a versioned folder under
your local app-data directory, and starts the game. `Install-Alatheya.cmd` remains a version-specific fallback.

Windows may show a reputation warning because development playtests are not code-signed. Continue only when
the installer was downloaded directly from this repository and its verification succeeds.

## Join a friend

Choose **Join a game**, enter the host's public IPv4 address or hostname, paste the unused invite code the host
sent you privately, and keep the port at **9999**. Each invite enrolls one installation's server-specific
cryptographic identity; later joins from that installation need no code. The host and every player must use the
same release. Hosting over the internet requires inbound UDP 9999 in Windows
Firewall and a router forwarding rule to the host PC. Carrier-grade NAT can prevent direct inbound hosting.

Every release is a development friend-playtest candidate. It is not a production release or a dedicated-server
distribution. Release notes name current limitations and provide manual download/checksum instructions.

The launcher and game are intentionally unsigned for this friend-playtest track. Package hashes protect the download;
the host-side allowlist controls who may enter a game. Neither mechanism is DRM, and neither hides assets that
must be present on a player's computer.
