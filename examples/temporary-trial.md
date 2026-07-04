# Temporary Trial Example

Use this when you want to test the skill without letting it participate in normal chats.

## Install

Windows PowerShell:

```powershell
$src = "C:\path\to\paper-mentor-skill\paper-mentor"
$dst = "$env:USERPROFILE\.codex\skills\paper-mentor"

New-Item -ItemType Directory -Force "$env:USERPROFILE\.codex\skills"
if (Test-Path $dst) { Remove-Item -Recurse -Force $dst }
Copy-Item -Recurse -Force $src $dst
```

## Test

```text
Use $paper-mentor in Paper Health Check mode.

Field: [field]
Target venue or reader: [venue]
Artifact type: abstract
Claimed contribution: [claim]
My biggest concern: [concern]

Text:
[paste text]
```

## Remove

```powershell
Remove-Item -Recurse -Force "$env:USERPROFILE\.codex\skills\paper-mentor"
```
