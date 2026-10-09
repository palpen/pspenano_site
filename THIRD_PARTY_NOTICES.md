# Third-party notices and licensing scope

The root LICENSE covers only the named Palermo-original contributions.
It does not replace licenses for components or authorize reuse of excluded
material.

## XMin theme

The bundled XMin theme is credited to Yihui Xie. Its existing notice at
[themes/xmin/LICENSE.md](themes/xmin/LICENSE.md) is preserved unchanged.
The notice below is copied verbatim from
[the bundled source at commit 8309bd3](https://github.com/palpen/pspenano_site/blob/8309bd387d92ec771e01060a56b911de6ad5ad25/themes/xmin/LICENSE.md).
Upstream project: https://github.com/yihui/hugo-xmin

The notice applies to XMin material, including its layouts, example site,
and static CSS. It is not a grant for independently sourced additions merely
because they are stored under the theme directory.

```text
The MIT License (MIT)

Copyright (c) 2017 Yihui Xie

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Excluded material and provenance limits

- The public Git submodule is a separate generated-site repository,
  https://github.com/palpen/palpen.github.io. Its pinned commit is unchanged;
  consult that repository's licensing documents for its current distribution.
- content/posts/img/first-post/myimg.png and other image assets are excluded
  from Palermo's MIT grant. No additional image permission is asserted here.
- deploy.sh follows the Hugo GitHub Pages deployment example referenced in
  README.md. Its third-party provenance has not been fully resolved; it is
  excluded rather than relicensed.
- themes/xmin/layouts/partials/mathjax_support.html contains MathJax setup code
  and cites https://github.com/mojombo/jekyll/issues/199. The provenance of these
  additions has not been fully established. No new permission is asserted for
  them. The externally loaded MathJax library has its own terms.
- Referenced articles, external resources, copied snippets, and third-party
  material are not covered by the root MIT grant. The references already in
  the posts remain in place.

This documentation does not resolve missing third-party permission. Before
redistributing excluded material, establish its applicable terms or obtain
permission from its rights holder.

## Generated-site notice retention

When publishing or regenerating the public site, preserve the applicable XMin
copyright and full permission notice in the distribution, together with any
other applicable notices. A theme-credit footer alone does not reproduce the
MIT notice. This change edits licensing documentation only; it does not alter
the build or the public submodule.
