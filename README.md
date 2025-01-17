# zinit-annex-link-man<a name="zinit-annex-link-man"></a>

<!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=2 -->

- [Usage](#usage)
- [How it works](#how-it-works)
- [Ice Modifiers Provided By The Annex](#ice-modifiers-provided-by-the-annex)
  - [`lman`](#lman)

<!-- mdformat-toc end -->

A Zsh-Zinit annex (i.e. an extension) that provides functionality, which allows to:

1. Run programs and scripts without adding anything to `$PATH` via the automatic creation of **links** in `$ZPFX/bin`

## Usage<a name="usage"></a>

Simply load like a regular plugin, i.e.:

```zsh
zinit light zdharma-continuum/zinit-annex-linkman
```

After executing this command you can then use the new ice-mods provided by the annex.

## How it works<a name="how-it-works"></a>

## Ice Modifiers Provided By The Annex<a name="ice-modifiers-provided-by-the-annex"></a>

There is one ice-modifier provided and handled by this annex. They are:

1. `lman''` – creates `links` for binaries and scripts.

**The ice-modifier in detail:**

### `lman`<a name="lman"></a>

It creates the `link` that calls the actual binary. The link is created always under the same, standard and single
`$PATH` entry: `$ZPFX/bin` (which is `~/.zinit/polaris/bin` by default).
