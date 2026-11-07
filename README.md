# BEAMcxp

Link loop tester for Barco Event Master processors (E2, S3, EX). Loop one CXP cable from connector 1 to connector 2 on a link card, click **Run link test**, and BEAMcxp runs Barco's `LLPTEST` over telnet and shows PASS / FAIL with a picture of the card and cable, which of the 11 loops failed, the card's serial number, firmware and cable length, and what to do next (per Barco Info-T 1558). Keeps a test history and exports a PDF report for support tickets. By [BEAM Events](https://beamevents.com).

This repository only holds the **installers and updates**.

## Download
Get the latest version from **[Releases](https://github.com/BEAMevents/BEAMcxp/releases/latest)**:

- **Windows: BEAMcxp-Setup-x.y.z.exe** installs BEAMcxp and **updates itself automatically**. Use this one.
- **Windows: BEAMcxp-Portable-x.y.z.exe** runs without installing (e.g. from a USB stick). It tells you when a newer version is out, but doesn't update itself.
- **Mac (Apple Silicon): BEAMcxp-x.y.z-mac-arm64.dmg**: open it and drag BEAMcxp to Applications. It updates itself from then on.

The installers aren't notarized yet. On Windows, SmartScreen may warn on first launch: click **More info → Run anyway**. On a Mac, the first time, open it, click **Done**, then go to System Settings → Privacy & Security and click **Open Anyway**. macOS also asks for **Local Network** access the first time: allow it, or BEAMcxp can't reach the processors.

## Updates
BEAMcxp checks for updates in the background and shows **Update x.y.z ready** in its header. Click it (or the version number), then **Install & restart**. It never restarts while a link test is running.
