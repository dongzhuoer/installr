# lightweight installation of fake R package

Some projects format theirselves as R packages to provide a standard and convenient way to install denpendencies. Like [hadley/r4ds](https://github.com/hadley/r4ds), which contains a `DESCRIPTION`, one just needs `remotes::install_github("hadley/r4ds")`, then happily builds the book with **bookdown**. 

However, cloning the whole project may take too long, especially for Chinese (thanks to GFW). So I create this _tiny_ repo to automatically synchronize `DESCRIPTION`, enabling `remotes::install_github("dongzhuoer/installr/hadley/r-pkgs")`

By the way, R package name can only use `.` to separate words, so I might modify a package's name, like [r-pkgs](https://github.com/hadley/r-pkgs) -> `r.pkgs`



-----------------------

[![Creative Commons License](https://i.creativecommons.org/l/by-nc/3.0/88x31.png)](http://creativecommons.org/licenses/by-nc/3.0/)  
This work is licensed under a [Creative Commons Attribution-NonCommercial 3.0 Unported License](http://creativecommons.org/licenses/by-nc/3.0/)
