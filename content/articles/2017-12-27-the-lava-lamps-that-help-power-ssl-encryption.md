---
categories:
- Design &amp; UX
- Technology
date: '2017-12-27'
permalink: /the-lava-lamps-that-help-power-ssl-encryption/
title: The lava lamps that help power SSL encryption
url: /2017/12/27/the-lava-lamps-that-help-power-ssl-encryption
---

File this one under "crazy stuff I learned this week": [Cloudfare uses streaming images of a wall of lava lamps](https://www.youtube.com/watch?v=1cUUfMeOijg) in their San Francisco office to partially generate the salts in the encryption keys that power their SSL services.

<iframe width="560" height="315" src="https://www.youtube.com/embed/1cUUfMeOijg?rel=0" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>

Why? Computers suck at generating random number, and Cloudfare has to create a lot of them.

Lava Lamps are unpredictable. Images of them create tons of tiny variances in the data behind the image (as do things like the lighting conditions in any particular moment), and that data is used to help create randomness in encryption key generation.

Super weird. Super rad.