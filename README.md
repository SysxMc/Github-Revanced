---
ReVanced APK Builder - GitHub Actions

Automated APK patching with ReVanced CLI, powered by GitHub Actions.

This project patches official APKs (like YouTube) using the latest ReVanced tools, and publishes the result as a release. No local setup required.


---

Features

Fully automated APK patching via GitHub Actions

Uses the latest:

ReVanced CLI

ReVanced Patches

ReVanced Integrations


Daily builds via scheduled workflows

Manual trigger support with one click

Patched APKs are uploaded as GitHub release assets



---

How It Works

This workflow:

1. Downloads the latest ReVanced CLI, patches, and integrations


2. Fetches the target APK (e.g., YouTube)


3. Patches the APK using ReVanced CLI


4. Uploads the result as a GitHub release




---

Usage

1. Fork the repository

git clone https://github.com/YOUR_USERNAME/revanced-apk-builder.git

2. Add APKs

Place your APK files in the apks/ folder (e.g. apks/youtube.apk)
OR modify the workflow to download them from a trusted source.

3. Trigger Workflow

Manually: Go to the Actions tab → Patch APK with ReVanced → Run workflow

Automatically: Scheduled to run daily at 12:00 UTC



---

Download Patched APKs

Patched APKs will appear in the Releases section.

Each release is tagged by the build date.


---

Example

java -jar revanced-cli.jar \
  patch \
  -b revanced-patches.jar \
  -m revanced-integrations.apk \
  -o youtube-patched.apk \
  apks/youtube.apk


---

Legal Notice

This repository does not distribute copyrighted APKs.

You must provide your own APKs or download them from legal sources.
Use at your own risk. This project is not affiliated with YouTube, Google, or ReVanced.


---

License

MIT

---
