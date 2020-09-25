## __cfbscrapR-data__ 
[![Twitter Follow](https://img.shields.io/twitter/follow/cfbscrapR?style=social)](https://twitter.com/cfbscrapR) [![Twitter Follow](https://img.shields.io/twitter/follow/saiemgilani?style=social)](https://twitter.com/saiemgilani)

### __cfbscrapR data 2014-2020__
![cfbscrapr-tile-1-300.png](https://raw.githubusercontent.com/saiemgilani/cfbscrapR/master/man/figures/cfbscrapr-tile-1-300.png)

```
seasons <- 2014:2020
pbp <- purrr::map_df(seasons, function(x) {
  readRDS(
    url(
      glue::glue("https://raw.githubusercontent.com/saiemgilani/cfbscrapR-data/master/pbp_players_pos_{x}.RDS")
    )
  )
})
```
