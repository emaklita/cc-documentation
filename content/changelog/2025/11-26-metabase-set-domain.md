---
title: Set Metabase domain at creation
description: Dark mode, variables in SQL snippets, dynamic goals for progress bars, embedding Hub, new components in Embedded Analytics JS, and more
date: 2025-11-26
tags:
  - addons
  - metabase
authors:
  - name: Sébastien Allemand
    link: https://github.com/allemas
    image: https://github.com/allemas.png?size=40
  - name: David Legrand
    link: https://github.com/davlgd
    image: https://github.com/davlgd.png?size=40
excludeSearch: true
---

When you deploy a Metabase add-on on Clever Cloud, you can access its admin interface through a `<random_chars>-metabase.services.clever-cloud.com` domain. You can now set a custom domain at creation through the `base-domain` option in Clever Tools:

```bash
clever addon create metabase yourMetabaseNameOrId --option base-domain=metabase.example.com
```

- [Learn more about Metabase on Clever Cloud](/doc/addons/metabase/)
