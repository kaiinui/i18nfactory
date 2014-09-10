i18nfactory
===========

i18nfactory

Why?
---

i18n is still dirty work.

How?
---

* Use Gengo / Google translator (for free) to obtain the i18n-ed text.
* Push GitHub to go.
* And web editor (which can commit&push to GitHub).
* (So it will be like CI server)

Concerns
---

- Contexts (i18n context)
  * Annotate `@context` to decribe a context. (Which will be translated via Googletrans).
  * Screenshot `@screenshot(https://dropbox.com/public/hodsfjfi/hoge.png)`

- Retain state in the strings file
  * comments (annotation)

```
/* @i18nfactory(auto, googletrans, 20140423, 7f9a0a4) */
"HELLO" = "こんにちは";
```

- GitHub security
  * add "i18nfactorybot" to contributor
  * then "i18nfactorybot" will push some code.

Testing
---

- GitHub push&commits will be difficult to test.
- webhook.
- gengo / google translate API.
