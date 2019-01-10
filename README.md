# rt-making-r-and-rstudio-work-for-me

How i make the great R and R Studio work fabulously for me :-) NOT SUPPORTED #ymmv  #jennybryanrocks #hadleyrocks

## 09January2019 Configuring gmailr

* followed https://github.com/jennybc/send-email-with-r

## 07January2019 how to calculate time differences for support

```r
interval(ymd_hms("2019-01-04 18:40:00", 
  tz = "America/Vancouver"), 
  ymd_hms("2019-01-07 12:59:00", 
    tz = "America/Vancouver")) / hours(1)
[1] 66.31667
```

* The above ^^^^ is the most accurate! 
You can also use lubridate durations, but 
durations aren't accurate when you transition 
from month to month or year to year
