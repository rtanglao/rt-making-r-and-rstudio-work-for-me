# rt-making-r-and-rstudio-work-for-me

How i make the great R and R Studio work fabulously for me :-) NOT SUPPORTED #ymmv  #jennybryanrocks #hadleyrocks

## 07 January 2019 how to calculate time differences for support

```r
> interval(ymd_hms("2019-01-04 18:40:00", tz = "America/Vancouver"), ymd_hms("2019-01-07 12:59:00", tz = "America/Vancouver")) / hours(1)
[1] 66.31667
```

* the above is accurate you can use use lubridate lubridate durations, but good enough if we don't wrap around a month
