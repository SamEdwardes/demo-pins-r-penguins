# demo-pins-r-penguins

A demo of using pins with RStudio pro products.

![](app/imgs/connect-screenshot.png)

## Usage

Render the report in RStudio:

```r
rmarkdown::render("app/report.Rmd")
```

## Deployment

Update the *manifest.json* file:

```r
rsconnect::writeManifest("app", appFiles = c("report.Rmd", "imgs"))
```

Then commit any changes to git. The report will automatically redeploy.
