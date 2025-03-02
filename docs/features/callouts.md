---
title: Callouts
tags:
  - feature/transformer
---

Quartz supports the same Admonition-callout syntax as Obsidian.

This includes

- 12 Distinct callout types (each with several aliases)
- Collapsable callouts

```
> [!info] Title
> This is a callout!
```

See [documentation on supported types and syntax here](https://help.obsidian.md/Editing+and+formatting/Callouts).

> [!warning]
> Wondering why callouts may not be showing up even if you have them enabled? You may need to reorder your plugins so that [[ObsidianFlavoredMarkdown]] is _after_ [[SyntaxHighlighting]].

## Customization

- Disable callouts: simply pass `callouts: false` to the plugin: `Plugin.ObsidianFlavoredMarkdown({ callouts: false })`
- Editing icons: `quartz/plugins/transformers/ofm.ts`

## Showcase

> [!info]
> Default title

> [!question]+ Can callouts be nested?
>
> > [!todo]- Yes!, they can. And collapsed!
> >
> > > [!example] You can even use multiple layers of nesting.

> [!note]
> Aliases: "note"

> [!abstract]
> Aliases: "abstract", "summary", "tldr"

> [!info]
> Aliases: "info"

> [!todo]
> Aliases: "todo"

> [!tip]
> Aliases: "tip", "hint", "important"

> [!success]
> Aliases: "success", "check", "done"

> [!question]
> Aliases: "question", "help", "faq"

> [!warning]
> Aliases: "warning", "attention", "caution"

> [!failure]
> Aliases: "failure", "missing", "fail"

> [!danger]
> Aliases: "danger", "error"

> [!bug]
> Aliases: "bug"

> [!example]
> Aliases: "example"

> [!quote]
> Aliases: "quote", "cite"
