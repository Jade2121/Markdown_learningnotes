## handbook for look up:

https://bookdown.org/yihui/rmarkdown/

https://xianbai.me/learn-md/index.html

https://bookdown.org/xiao/RAnalysisBook/


## 1.Rmd输出pdf报错
    
### 报错：
output file: Han_Homework3.knit.md

! Package inputenc Error: Unicode character 杞?(U+8F7D)
(inputenc)                not set up for use with LaTeX.

Try other LaTeX engines instead (e.g., xelatex) if you are using pdflatex. See https://bookdown.org/yihui/rmarkdown-cookbook/latex-unicode.html
错误: LaTeX failed to compile Han_Homework3.tex. See https://yihui.org/tinytex/r/#debugging for debugging tips. See Han_Homework3.log for more info.
此外: Warning message:
In grepl("==> Fatal error occurred", x[i], fixed = TRUE) :
  输入的字符串1不适用于此语言环境
停止执行

    
### 解决：
在文件头部pdf输出上配置下列文件

```{r}
 output:
     pdf_document:  
         latex_engine: xelatex
```

#### Reference:
https://stackoverflow.com/questions/32794157/package-inputenc-error-unicode-char-u8-in-rstudio  
https://github.com/rstudio/rmarkdown/issues/1450


## 2. mathematics in markdown
https://rpruim.github.io/s341/S19/from-class/MathinRmd.html
https://blog.csdn.net/Katherine_hsr/article/details/79179622
note: if there is more than one symbol, use $$ ranther than $.

         


#### Other Helpful:
https://blog.csdn.net/adan_journal_of_data/article/details/78900476

