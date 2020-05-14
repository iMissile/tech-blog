# Общие по блогу
- [Мой сайт на Netlify](https://app.netlify.com/sites/upbeat-fermi-2897d4/deploys).
- [Мой домен](www.ishutov.ru)

- [Как сделать редирект: подробный обзор для гуманитариев](https://texterra.ru/blog/kak-sdelat-redirekt-podrobnyy-obzor-dlya-gumanitariev.html)
- [Как вручную выполнить переадресацию и маскировку домена или субдомена](https://ru.godaddy.com/help/kak-vruchnuyu-vypolnit-pereadresaciyu-i-maskirovku-domena-ili-subdomena-422)
- [How to build a website with Blogdown in R](https://www.storybench.org/how-to-build-a-website-with-blogdown-in-r/)
- [R Blogdown Setup in GitHub (2)](https://aurora-mareviv.github.io/talesofr/2018/02/r-blogdown-setup-in-github-2/)
- [Setting up our blog with RStudio and blogdown I: Creating the blog](http://estebanmoro.org/post/2019-02-02-setting-up-your-blog-with-rstudio-and-blogdown-i-creating-the-blog/)
- [Day 1: Getting started with blogdown](https://djnavarro.net/post/starting-blogdown/) by by Danielle Navarro, 27 Apr 2018

# Настройка темы
После экспериментов оказалось, что лучше остаться на штатной `hugo`, другие темы находятся в непонятной фазе развития, чтобы еще и их не править на первых шагах.

- [Change your {blogdown} fonts](https://www.rostrum.blog/2018/11/29/fontface-lithium/). На [самом гугле](https://google-webfonts-helper.herokuapp.com/fonts/roboto?subsets=cyrillic,latin) смотрим на шрифты и читаем как настроить css.
- [Кирилличские шрифты Google](https://fonts.google.com/?subset=cyrillic)
- COOL! [Using themes with blogdown: Lesson learned](https://portfolio.peter-baumgartner.net/2018/07/19/blogdown-using-themes/). См. "Problem solving strategies" и сслыки внизу статьи.
- [Kiera theme](https://themes.gohugo.io/theme/hugo-kiera/). Как оказалось, расположение директорий не совсем штатное.
```
install.packages("blogdown")
blogdown::update_hugo()
library(blogdown)
blogdown::hugo_version()
blogdown::new_site(theme = "funkydan2/hugo-kiera")
blogdown::build_site()
blogdown:::serve_site()
servr::daemon_stop(1)
```

