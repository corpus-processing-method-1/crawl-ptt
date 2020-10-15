# crawl-ptt

See <https://github.com/shihjyun/PTTmineR>.

```r
# Install dependencies
install.packages("remotes")
remotes::install_github("shihjyun/PTTmineR")

# Crawl PTT
library(PTTmineR)
library(future.apply)
rookie_miner <- PTTmineR$new(task.name = "Mr. Meeseeks")
mine_ptt(rookie_miner, board = "Gossiping", last.n.page = 5)

# Access crawled results
export_ptt(rookie_miner, export.type = "tbl", obj.name = "tbl_result")
tbl_result$post_info_tbl
tbl_result$post_comment_tbl
```

https://classroom.github.com/a/wwsS-UKI
