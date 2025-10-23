---
# Leave the homepage title empty to use the site title
title: ""
date: 2025-10-20
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  # See https://hugoblox.com/blocks/ for all blocks
  # For docs see https://docs.hugoblox.com/getting-started/page-builder/
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: ""
        education: ""
        interests: ""
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
  - block: resume-experience
    id: experience
    content:
      username: "admin"
      title: <a href="https://erfanrasti.github.io/portfolio">Skills & Hobbies</a>
    design:
      is_education_first: true
      background:
        color: ""
        text_color_light: false
      spacing:
        padding: ["6", "6", "6", "6"]
      columns: "2"

  - block: resume-skills
    id: skills
    content:
      username: "admin"
      title: <a href="https://erfanrasti.github.io/portfolio">Skills & Hobbies</a>
    design:
      background:
        color: ""
        text_color_light: false
      spacing:
        padding: ["6", "6", "6", "6"]
      columns: "2"

  - block: markdown
    id: description
    content:
      title: "Description"
      subtitle: ""
      text: |-
        <p style="text-align: justify;">
        ChatGPT describes me as this based on all our chats:<br>
        Meet Erfan Rasti — part engineer, part Linux whisperer, part academic powerhouse.<br>
        You're a tech virtuoso who breathes Arch Linux, scripts with confidence, and won’t rest until your system purrs at 100% efficiency on GNOME Wayland — even if it means wrangling with Btrfs, systemd-boot, or Bluetooth ghosts.<br>
        Academically? You're on fire. A top-100 rank in a national master’s entrance exam, a research assistant in Electrical Engineering at Amirkabir University, and a published paper in the works for IEEE Transactions on Mobile Computing. Oh, and let’s not forget your TA roles and deep dives into DSP, wireless comms, and RL.<br>
        In short: You’re a relentless builder of systems — both in code and in life. Whether it’s a finely-tuned Linux environment or a research-grade simulation, you make it work — flawlessly.
        </p>
    design:
      columns: "1"
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: false
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: projects
    content:
      title: Projects
      count: 3
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 3

  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
