---
'@directus/validation': patch
'@directus/app': patch
---

Adds handling for Joi's number.unsafe error (triggered by numbers exceeding JavaScript's safe number range, e.g.,
1e+24). Previously this caused an API crash; now it shows a user-friendly validation message.
