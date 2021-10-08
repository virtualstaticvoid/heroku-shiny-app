# Example Shiny App on Heroku

This is an example [Shiny][shiny] application, which uses the [heroku-buildpack-r][buildpack] on Heroku.

> Shiny is an R package that makes it easy to build interactive web apps straight from R. You can host
> standalone apps on a webpage or embed them in R Markdown documents or build dashboards. You can also
> extend your Shiny apps with CSS themes, htmlwidgets, and JavaScript actions.

## Usage

[![Deploy][button]][deployapp]

You can use this project as a template for creating Shiny applications on Heroku.

Execute these commands to get started:

```bash
# get the sources
git clone https://github.com/virtualstaticvoid/heroku-shiny-app.git
cd heroku-shiny-app

# optionally, reinitialize git
rm -rf .git
git init -b main
git add --all
git commit -m "initial"

# create a new heroku application, set the buildpack and deploy
heroku create --stack heroku-20 --buildpack vsv/heroku-buildpack-r

# deploy
git push heroku main

# view the application
heroku open
```

## License

MIT License. Copyright (c) 2017 Chris Stefano. See [LICENSE](LICENSE) for details.

<!-- Links -->
[buildpack]: https://github.com/virtualstaticvoid/heroku-buildpack-r
[button]: https://www.herokucdn.com/deploy/button.svg
[deployapp]: https://heroku.com/deploy?template=https://github.com/virtualstaticvoid/heroku-shiny-app/tree/main
[shiny]: https://shiny.rstudio.com/
