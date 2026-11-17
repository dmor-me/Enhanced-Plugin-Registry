# Yapfast Enhanced Marketplace

This repository is the public plugin catalog for Yapfast Enhanced. Its first listing is the pinned Ping example.

Plugin authors can propose a listing under `plugins/` and add its ID to `index.json`. Include the plugin's HTTPS repository URL, immutable commit, module SHA-256, permissions, and license. Separate GitHub and Codeberg plugin repositories can be listed here.

The Marketplace reads listing data when browsing. It shows the plugin and its permissions before installation. You can use the Yapfast plugin helper to check a listing:

```text
yapfast-plugins verify-entry plugins/com.example.ping.json
```
