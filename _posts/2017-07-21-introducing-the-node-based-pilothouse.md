---
layout: post
title:  "Introducing the Node-based Pilothouse"
date:   2017-07-21 17:18:00 -0400
---

Pilothouse 0.1.0 has just been released [on NPM](https://www.npmjs.com/package/pilothouse). The Bash-based Pilothouse is now deprecated.

The NodeJS version of Pilothouse is a complete rewrite, with a number of exciting improvements, but also some breaking changes from older Bash-based versions of Pilothouse.

There are a few notable things you should be aware of:

1. Pilothouse is now managed by [NPM](https://www.npmjs.com/). Instead of pulling down the latest commits using git from the Pilothouse repo in order to update to a new version, simply run `npm update -g pilothouse`.
2. All sites now have SSL support automatically available out-of-the-box. You no longer need to generate an SSL certificate on a per-site basis.
3. All site's Nginx configurations are now generated dynamically for each local site. While you shouldn't normally need to override the auto-generated config, [advanced users can do so if desired](https://github.com/Pilothouse-App/pilothouse/wiki/Customizing-a-Local-Site's-Nginx-Configuration).
4. All site-specific settings, such as the [config.yml settings file](https://github.com/Pilothouse-App/pilothouse/wiki/Customizing-a-Local-Site's-Settings) or the site-specific nginx override config file are now contained in the site's root directory.
5. The Pilothouse service configuration directory is now `~/.pilothouse`. Any [configuration file overrides](https://github.com/Pilothouse-App/pilothouse/wiki/How-to-Override-Configuration-Files) should be placed there.