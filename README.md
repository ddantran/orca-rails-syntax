# Rails Syntax

Ruby and ERB syntax highlighting for Orca, built from the TextMate grammars of the
[Ruby LSP](https://github.com/Shopify/ruby-lsp) VS Code extension.

| Language | Files |
| --- | --- |
| Ruby | `.rb`, `.rake`, `.gemspec`, `.ru`, `.jbuilder`, `Gemfile`, `Rakefile` and the other names Ruby LSP lists |
| ERB | `.erb` (so `.html.erb`), `.rhtml`, `.rhtm` |

`<% %>` and `<%= %>` highlight as Ruby in text, tag bodies and attribute values. Rails methods
called without parentheses, such as `belongs_to`, `before_action`, `resources` and `link_to`, get
the same function color as calls with parentheses. Colors come from the grammar scopes only:
Ruby LSP's server-side semantic tokens are not part of this plugin. CSS and JavaScript inside ERB
views stay plain.

## Install

In Orca's plugin settings, paste the GitHub URL of this repository:

```
https://github.com/ddantran/orca-rails-syntax
```

The plugin only adds highlighting, so it needs no approval.

## Develop

```sh
git clone https://github.com/ddantran/orca-rails-syntax
orca plugin validate orca-rails-syntax
orca plugin dev load orca-rails-syntax    # adds the folder under Settings → Plugins → Development folders
```

A development copy has the plugin key `local.rails-syntax`.

## License

MIT, see `LICENSE`. The grammars in `syntaxes/` come from other projects: sources and licenses
are in `THIRD_PARTY.md`.
