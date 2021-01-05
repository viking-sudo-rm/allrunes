> Have you ever wanted to painlessly typeset runic characters in your arXiv papers? Now you can!

# arXiv-safe `allrunes` package for LaTeX

I recently attempted to typeset runic characters in a revision for a paper on arXiv. The `allrunes` package had worked flawlessly in the old version of the paper. However, I found that `allrunes` now breaks the new TeX distribution used by arXiv.

To fix this, I modified the `allrunes` source, removing the compatibility issues, and rebuilt it. This repository contains the resulting .sty file, so you don't have to do this.

To make the fix, all you have to do is drop allrunes.sty into your LaTeX project, and import `allrunes` as normal. This can be done painlessly in Overleaf, for example. The project should also build on arXiv without issue.