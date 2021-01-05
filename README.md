> Have you ever wanted to painlessly typeset runic characters in your arXiv papers? Now you can!

# arXiv-safe `allrunes` package for \*TeX

I recently attempted to typeset runic characters in a revision for a paper on arXiv. The `allrunes` package had worked flawlessly in the old version of the paper. However, I found that `allrunes` now breaks the new TeX distribution used by arXiv, as documented on [StackExchange](https://tex.stackexchange.com/questions/558058/command-swdefault-already-defined).

To fix this, I modified the `allrunes` source, removing the compatibility issues, and rebuilt it. This repository contains the resulting .sty file, so you don't have to do this.

To make the fix, all you have to do is drop allrunes.sty into your project, and import `allrunes` as normal. This can be done painlessly in Overleaf, for example. Your project should build on arXiv without issue.

## `allrunes`

Documentation for `allrunes` can be found [here](https://ctan.org/pkg/allrunes?lang=en). The only difference in this version is that the constant `\swdefault` has been renamed to `\swdefaultpatch`.
