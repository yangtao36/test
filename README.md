# 安裝說明

請在R console貼上下列script:

```r
deps <- available.packages("http://54.92.61.128/R")[1,"Depends"]
pkgs <- strsplit(gsub("\\s", "", deps), ",")[[1]]
for(pkg in pkgs) {
  # You can change your favorite repository
  install.packages(pkg, repo = "http://cran.csie.ntu.edu.tw")
}
install.packages('DSC2014Tutorial', repo = 'http://54.92.61.128/R', type = 'source')
```

# 投影片

```r
slides("Basic")
slides("ETL")
```

# 資料

- `cl_info_other` 
    - 可以直接使用`data(cl_info_other`載入data.frame
    - 可以使用`system.file("Basic/cl_info_other.csv", packages="DSC2014Tutorial")`來access .csv原始檔

# 範例

## R Basic

- 練習1, `system.file("Basic/exercise1.R", packages="DSC2014Tutorial")`
