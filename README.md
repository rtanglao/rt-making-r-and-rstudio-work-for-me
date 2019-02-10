# rt-making-r-and-rstudio-work-for-me

How i make the great R and R Studio work fabulously for me :-) NOT SUPPORTED #ymmv  #jennybryanrocks #hadleyrocks

## 09February2019 getting environment variables to work

* Create ~/.Renviron with the following lines

```bash
MONGO_PORT="27017"
MONGO_HOST="127.0.0.1"
SUMO_QUESTIONS_DB="ffdesktop20182019"
```

* restart R in R Studio

## 25January2019 how to start rstudio server in wsl
```bash
sudo rstudio-server start
```
and then from firefox on the windows side, open this url:
```
http://localhost:8787/
```

## 09January2019 Configuring gmailr


* followed https://github.com/jennybc/send-email-with-r
* in order not to have to do the oauth dance every time, you have to:

```r
install.packages("httpuv")
```

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
