---
title: Set Keycloak domain at creation
description: Dark mode, variables in SQL snippets, dynamic goals for progress bars, embedding Hub, new components in Embedded Analytics JS, and more
date: 2025-11-27
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

When you deploy a Keycloak add-on on Clever Cloud, you can access its admin interface through a `<random_chars>-keycloak.services.clever-cloud.com` domain. You can now set a custom domain at creation through the `base-domain` option in Clever Tools:

```bash
clever addon create metabase yourMetabaseNameOrId --option base-domain=keycloak.example.com
```

This domain DNS configuration needs to point to Clever Cloud's servers. For example, if the Keycloak add-on is deployed in the `par` (Paris) region, you need to create a CNAME record pointing to `domain.par.clever-cloud.com.`.

- [Learn more about Keycloak on Clever Cloud](/doc/addons/keycloak/)
- [Learn more about DNS and custom domains on Clever Cloud](/doc/administrate/domain-names/)
