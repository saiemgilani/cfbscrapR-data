# cfbscrapR-data
 cfbscrapR data 2014-2020

```
seasons <- 2014:2020
pbp <- purrr::map_df(seasons, function(x) {
  readRDS(
    url(
      glue::glue("https://raw.githubusercontent.com/saiemgilani/cfbscrapR-data/master/pbp_players_pos_{x}.rds")
    )
  )
})
```