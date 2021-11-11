Reproducible example for https://bugs.r-project.org/show_bug.cgi?id=16644

```r
install.packages("testUnload", repos = NULL, type = "source")
library("testUnload")
unloadNamespace("testUnload")
install.packages("testUnload", repos = NULL, type = "source")
library("testUnload")
```
