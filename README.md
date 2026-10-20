# Jarvis Private — Windows updates

Windows installers and updates for a Discord voice assistant that runs on your own PC. Every installation uses its owner’s Discord bot, OpenAI account, payment method, and chosen spending limits.

## Install

1. Open [the latest release](https://github.com/TheBaldAndFurious/jarvis-updates/releases/latest) and download the `Jarvis-Private-Setup-…exe` file.
2. Run it on a Windows 11 Intel/AMD 64-bit computer. Follow the browser setup guide. Node and voice components are included.
3. Create your own accounts, choose a name and wake phrase, select a text channel for silent answers and web sources, and enter your own daily and monthly caps. No spending amounts are preselected.
4. Enable automatic startup if you want the assistant to run after Windows restarts without signing in.

## Updates

Keep **Keep my assistant updated automatically** enabled during setup. The assistant checks for published releases periodically, downloads them in the background, and waits for a quiet minute before briefly disconnecting, updating, and reconnecting. You do not need to stop it manually for normal updates. Settings and spending history are preserved.

Downloaded releases are checked against the publisher verification key included in the installer. If a replacement cannot start, the previous version is restored. You can pause updates from the first **Set up Jarvis** screen. Major Windows prerequisite or update-host changes may require a manual installer upgrade.

The installer does not yet have a Windows publisher certificate, so Windows may show an unknown-publisher notice. Update signatures are separate from Windows publisher signing.

## Accounts and privacy

Ordinary channel chatter is processed locally for the wake phrase. Addressed questions use your own OpenAI account. Update checks send no Discord secrets, OpenAI keys, questions, or spending records to this repository; GitHub receives normal download connection information.

Share only the clean installer. Never upload an installed folder, `installation.json`, `.env`, recordings, usage data, or signing keys. This repository hosts public downloads; it is not a private account or data store.
