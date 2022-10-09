---
name: Bug report
about: Create a report to help us to improve things
title: "|BUG|"
labels: "bug"
  
---

body:
  - type: markdown
    attributes:
      value: |
        Thanks for fill out this bug report! Fill out the following form to your best ability to help us to fix the problem.
        Only use this if you're absolutely sure that you found a bug and can reproduce it. For anything else, use: [our Discord server](https://discord.gg/WYz7Qck) or [the wiki](https://github.com/trainerlord/WorldSystem/wiki).
        Do NOT use the public issue tracker to report security vulnerabilities!

  - type: dropdown
    attributes:
      label: Server Software
      description: Which server software are you using? No support if the version isn't listed. Switch to a supported software first.
      multiple: false
      options:
        - PurPur
        - Paper(spigot)
        - Spigot
    validations:
      required: true

  - type: dropdown
    attributes:
      label: Server Version
      description: Which server version do you use? No support if the version isn't listed. Update to a supported version first.
      multiple: false
      options:
        - '1.19.2'
        - '1.19.1'
        - '1.19'
        - '1.18.2'
        - '1.18.1'
        - '1.17.1'
        - '1.16.5'
        - '1.15.2'
    validations:
      required: true

  - type: textarea
    attributes:
      label: Describe the bug
      description: A clear and concise description of what the bug is.
    validations:
      required: true

  - type: textarea
    attributes:
      label: To Reproduce
      description: Steps to reproduce this behaviour
      placeholder: |
        1. Go to '...'
        2. Click on '...'
        3. Scroll down to '...'
        4. See error

  - type: textarea
    attributes:
      label: Expected behaviour
      description: A clear and concise description of what you expected to happen.

  - type: textarea
    attributes:
      label: Screenshots / Videos
      description: If applicable, add screenshots to help explain your problem.

  - type: input
    attributes:
      label: Error log (if applicable)
      description: If you are reporting a console error, upload any relevant log excerpts to either https://paste.gg/, https://pastebin.com or https://gist.github.com, save and the paste the link in this box.

  - type: input
    attributes:
      label: WorldSystem Version
      description: What WorldSystem version are you running? (`/ws help`)
      placeholder: "For example: WorldEdit version 2.4.31-3"
    validations:
      required: true

  - type: checkboxes
    attributes:
      label: Checklist
      description: Make sure you have followed each of the steps outlined here.
      options:
        - label: I have looked if this is already a issue
          required: true
        - label: I am using the newest build from https://github.com/CrazyCloudCraft/worldsystem-updated-old and the issue still persists.
          required: true

  - type: textarea
    attributes:
      label: Anything else?
      description: You can provide additional context below.
