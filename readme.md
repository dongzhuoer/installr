# lightweight installation of fake R package

Some projects format theirselves as R packages to provide a standard and convenient way to install denpendencies. Like [hadley/r4ds](https://github.com/hadley/r4ds), which contains a `DESCRIPTION`, one just needs `remotes::install_github("hadley/r4ds")`, then happily builds the book with **bookdown**. 

However, cloning the whole project may take too long, especially for Chinese (thanks to GFW). So I create this _tiny_ repo to automatically synchronize `DESCRIPTION`, enabling `remotes::install_github("dongzhuoer/installr/hadley/r-pkgs")`

By the way, R package name can only use `.` to separate words, so I might modify a package's name, like [r-pkgs](https://github.com/hadley/r-pkgs) -> `r.pkgs`


# Copied from GitHub

- https://github.com/tidyverse/tidyeval/blob/master/DESCRIPTION


r4ds add `devtools`

# compiled by Zhuoer Dong

- [rstudio/bookdown](rstudio/bookdown/DESCRIPTION)   
  from [here](https://github.com/rstudio/bookdown/tree/master/inst/examples) I extract `setup` chunk of `index.Rmd` and search `@R-` for all cited R packages. So there may be some redundency, but anyway I just want that the book can be built, the exact dependency should be specified by the author.

- [rstudio/blogdown](rstudio/blogdown/DESCRIPTION)  
  from [here] I mainly search `@R-` for all cited R packages and search `::` for all mentioned packages. So there may be some redundency, but anyway I just want that the book can be built, the exact dependency should be specified by the author.

- [rstudio/rmarkdown-book](rstudio/rmarkdown-book/DESCRIPTION)  
  Mainly copied from `knitr::write_bib()` in `20-references.Rmd`, plus my personal experience. So there may be some redundency, but anyway I just want that the book can be built, the exact dependency should be specified by the author.

- [yihui/r-ninja](yihui/r-ninja/DESCRIPTION)  
  Actually, even if you don't install this package, yihui has written some code in `index.Rmd` to automatically install dependencies. Later I find that **formatR** needs to manually install.


-----------------------

[![Creative Commons License](https://i.creativecommons.org/l/by-nc/3.0/88x31.png)](http://creativecommons.org/licenses/by-nc/3.0/)  
This work is licensed under a [Creative Commons Attribution-NonCommercial 3.0 Unported License](http://creativecommons.org/licenses/by-nc/3.0/)
