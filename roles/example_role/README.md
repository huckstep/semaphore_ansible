# Role: Example Role
# This is a template role showing best practices

---
# defaults/main.yml
# Default variables for the role
defaults:
  enabled: true
  version: "latest"

---
# vars/main.yml
# Variable overrides and computed values
# (secrets should come from vault files, not here)

---
# meta/main.yml
# Role dependencies and metadata
galaxy_info:
  author: your-name
  description: Your role description
  company: Your Company
  license: MIT
  min_ansible_version: "2.9"
  platforms:
    - name: Ubuntu
      versions:
        - focal
        - jammy
    - name: Debian
      versions:
        - bullseye
        - bookworm
    - name: CentOS
      versions:
        - "7"
        - "8"
        - "9"
  galaxy_tags:
    - development
    - infrastructure

dependencies: []

---
# tasks/main.yml
# Main tasks for the role
- name: Example task
  debug:
    msg: "Example role task"

---
# handlers/main.yml
# Handlers for the role
- name: Restart service
  debug:
    msg: "Restart service handler"

---
# templates/
# Place templates here

---
# files/
# Place static files here

---
# tests/
# Role tests
# (optional)

---
# README.md
# Role documentation
