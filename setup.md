---
title: Setup
---


{% include setup_r.html %}


{% include setup_bash_git.html %}

## Checks
Open RStudio. Click in the 'console' window. (It's the one with the '>')

Install the packages `blogdown`, and `xaringan` with the function `install.packages()`,
and the package `xaringanthemer` with the function `install_github()`.

Load them into your workspace with `library()` or `require()`.

When in doubt, follow the code chunk below.

**Hint**


If you do not want to load the packages you can call functions by specifying their package followed by two colons and the function, like this: `package_name::function_name()`.

This implies more typing but it gives more clarity to reproduce the workflow later. So we will use that syntax for this tutorial.

An exception to this are functions from packages that are "preloaded" --such as `library()` from the package `base`, or `install.packages()` from `utils`; these can simply be called by their name because these packages are preloaded when you open R.


**Code chunk**

```{r}
install.packages(c("blogdown", "xaringan"))
library(blogdown)
library(xaringan)
devtools::install_github("gadenbuie/xaringanthemer")
library(xaringanthemer)
```


{% include links.md %}
