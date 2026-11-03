# Third-party notices

The grammars in `syntaxes/` come from these sources.

| File | Source | License |
| --- | --- | --- |
| `ruby.tmLanguage.json` | [Shopify/ruby-lsp](https://github.com/Shopify/ruby-lsp) `vscode/grammars/ruby.cson.json`, converted from [atom/language-ruby @ f4082a0](https://github.com/atom/language-ruby/commit/f4082a02f467f8b253449d6998226fdea0957efa). Two rules are added after the kernel-method rule: Rails methods such as `has_many` and `link_to`, called without parentheses, get the scope `entity.name.function.rails.ruby`. | MIT (Shopify Inc.; GitHub Inc.) |
| `erb.tmLanguage.json` | Shopify/ruby-lsp `vscode/grammars/erb.cson.json`. The `injections` block is removed; its `<% %>` rules are the root patterns and the `erb-tags` rule. | MIT (Shopify Inc.) |
| `html.tmLanguage.json` | [microsoft/vscode](https://github.com/microsoft/vscode) `extensions/html/syntaxes/html.tmLanguage.json`, converted from [textmate/html.tmbundle @ 0c3d5ee](https://github.com/textmate/html.tmbundle/commit/0c3d5ee54de3a993f747f54186b73a4d2d3c44a2). The `injections` block is removed and `{ "include": "text.html.erb#erb-tags" }` is the first pattern of every rule that has a pattern list, except the `comment` rule. | TextMate Bundle License |

Orca grammars accept only `scopeName`, `patterns` and `repository` at the top level, and a plugin
can include only grammars from the same plugin. The changes above follow from that.

## MIT License (Shopify Inc.)

The MIT License (MIT)

Copyright (c) 2022-present, Shopify Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

## MIT License (GitHub Inc.)

Copyright (c) 2014 GitHub Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

## TextMate Bundle License

Copyright (c) textmate-html.tmbundle project authors

If not otherwise specified (see below), files in this repository fall under the following license:

Permission to copy, use, modify, sell and distribute this
software is granted. This software is provided "as is" without
express or implied warranty, and with no claim as to its
suitability for any purpose.

An exception is made for files in readable text which contain their own license information,
or files where an accompanying file exists (in the same directory) with a "-license" suffix added
to the base-name name of the original file, and an extension of txt, html, or similar. For example
"tidy" is accompanied by "tidy-license.txt".
