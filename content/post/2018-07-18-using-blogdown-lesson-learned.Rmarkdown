---
title: 'Using blogdown: Lesson learned'
author: Peter Baumgartner
date: '2018-07-18'
slug: using-blogdown-lesson-learned
categories: []
tags: []
authors:
  - Peter Baumgartner
header:
  caption: ''
  image: ''
  preview: no
draft: yes
summary: After almost one year of interruption I started using blogdown again and was confronted with a serie of problems. In this post I will report on my odyssean experience and --- more important --- I will suggest guidelines for the not so techie user how to start, explore and use blogdown on a daily basis. Skip the odyssean part and start immediately with the guidelines.
---

Finally --- after almost one year of interruption --- I could reorganize my responsibilities to spend more time working with blogdown and Hugo.

But (re-)starting blogging using these tools was not easy after such a long period. I did not only forget many procedures but ran also into compatibility problems with the necessary updates. It turned out for me that the R Markdown ecosphere produces not only valuable and powerful tools but is a continuously changing complex still stricken with some fragilities.

After reporting on these difficulties I will summarize the lessons I learned in the last couple of weeks.

## Report from an Odyssean Journey

### Problems with my old theme

Last year I was intrigued by the very powerful [docdock theme](https://themes.gohugo.io/docdock/). I has many dynamic features and is with it unlimited submenues especially good suited for complex structured information material. This was exactly the template I was looking for as I have learned in my previous WordPress posting career on [Gedankensplitter](http://peter.baumgartner.name) that over time new emerging subject have to be accommodated on the website. I was especially excited by using dynamic HTML slides with the [reveal.js](https://revealjs.com/#/) framework, which I used heavily for [tutorials](https://notes.peter-baumgartner.net/slide/) and teaching.

After updating my software machinery (R, R packages, Hugo) I also installed a new release of the docdock theme. And here the odyssey started! I got many error messages which I could not solve. One problem evidently was, that I tweaked the theme (sacrificing several days of my summer holiday last year) without the necessary profound knowledge of the way Hugo works. Another problem was that I had forgotten many procedures of the interplay between blogdown and Hugo.

After two full days of work I did not manage to get a functional website but and had additionally in the meanwhile destroyed my old (working) one as well. :cold_sweat: This was now for me an involuntary learning occasion to dive into Git in order to save my work and restore my repo. I had not worked on a special branch and had carelessly committed changes that destroyed my web presence.

To avoid similar issues I started a clean installation of blogdown with the docdock theme. This time I did not get error message rendering my blog, but experience another surprise! The theme style I preferred to use had other (new) problems: The display of code snippets was not correct anymore and destroyed the page layout. I reported this issue to the theme author. Only now I noticed that the author does not answer questions and issues. On the issue page of the docdock repo I found the following message from another user:

> Is this theme still maintained? Issues and PR's seem to indicate not. I'm looking to add a documentation theme but I'm not interested in adding one that's been abandoned.

This question is now unanswered for more than 20 days. :angry: I do not blame the theme author. People have to work for a living, they donate their work and experiences to us whenever it is possible. But how could I myself be so naive only to judge my theme selection by the functionality of the theme? Not taking into account the sustainability of the theme e.g. its complexity related with its life cycle (updates, bugs), the responsiveness of the author, the community of people using this theme and helping each other!

This was the moment I abandoned the docdock theme heavy-heatedly. I had put so much work into its adaption! And I like its functionality and design! Yes, I could still use my working version, but then I will loose future new features of Hugo. My trust to this theme was broken.

### Problems finding another suitable theme

This time I decided to choose a more simple theme and started with the [recommended theme list in the blogdown book](https://bookdown.org/yihui/blogdown/other-themes.html). The only one I liked from its design was [ghostwriter](https://themes.gohugo.io/ghostwriter/). I installed it without problems and began adapting it. My first project was to learn the [Xaringan package](https://slides.yihui.name/xaringan/#1) in combination with blogdown. I stumbled about it reading the new [R Markdown book](https://bookdown.org/yihui/rmarkdown/). It could be a way to replace my beloved html5 slide functionality from the docdock theme. Instead of using  [reveal.js](https://revealjs.com/#/) I had now to learn [remark.js](https://remarkjs.com/). But Yihui Xie --- the author behind all this fantastic stuff in the R Markdown ecosphere like knitr, blogdown, bookdown, xaringan etc. --- did a good case why [remark is preferable to other slide frameworks](https://yihui.name/en/2017/08/why-xaringan-remark-js/) (e.g. slidy, ioslides or beamer).

To shorten a long story: After several hours trying to bring Xaringan to work --- I followed the simple synopsis by [Tim Mastny](https://timmastny.rbind.io/)  in his blog entry [Embed Slides in Your Blog](https://timmastny.rbind.io/blog/embed-slides-knitr-blogdown/) --- it turned out that in the ghostwriter theme files in the static folder are not rendered and uploaded. This came as a big surprise for me! I thought this is a standard and obligatory feature. Only when I found an entry by [Amber Thomas on Stack Overflow](https://stackoverflow.com/questions/41176194/hugo-not-reading-rmd-files-after-using-blogdown) --- one of the co-authors of the blogdown book --- I learned that this could be possible.

The problem was --- at least for me --- a tricky one. It worked locally but not after deployed with netlify. It is true: After some trials I noticed that there are no static files uploaded in my repository. But as a novice user I always think that the problem is on my side, doing something wrong. Only after I installed the [Xmin theme](https://themes.gohugo.io/hugo-xmin/) I learned that everything I did was done correctly.

This time I abandoned the theme much easier than before as I was not yet emotionally linked to the theme and had not started with adaption work of the theme. I learned that it is a good strategy to test things out with the Xmin theme as a reference point. Should I stick with Xmin to be on the secure side? But really I do not like this theme from it appearance. My CSS knowledge is very poor and I do not want to spend much learning and working time to adapt it to me needs.

My next choice was the [academic theme](https://themes.gohugo.io/academic/). Last year I had already experimented with it and it is one of the (more complex) recommendation in the blogdown book. It is a very elaborated theme with fantastic features designed for academic usage. But exactly this was the reason why I decided against this theme. I am looking forward to my retirement and I am fed up from all the administrative university business: The thought of (re)presenting all details of my scientific work and especially to transfer my more than 200 publications from my WordPress blog Gedankesplitter to the academic framework made me furious. All I was looking for was a decent blog framework open for all the nice tools from the R Markdown ecosphere.

But incidentally just at the same time I noticed problems with some of the WordPress plugins dynamically serving my list of publications. And I am not forced to use all sections of the academic framework: I could streamline it focusing on the posts section --- and maybe later on add some other features.

So I returned to my abandoned experiments with the academic theme as I already did some configuration and had even written some content. First of all I updated it to the new version and … --- Yes, again I ran into troubles! After some trials I noticed a wired problem: It took me two days to narrow down the error. It turned out that with one of the last updates the academic theme was not compatible with blogdown anymore! I reported this issue to [RStudio community](https://community.rstudio.com/t/serve-site-creates-index-of-site-rather-than-site-preview-blogdown/11120) and to [George Cushen](https://github.com/gcushen/hugo-academic/issues/594) and [Yihui Xie](https://github.com/rstudio/blogdown/issues/315).

I am not sure if you can imagine my emotional state: It changed between desperation and depression. All in all it took me ten days with the result that I had nothing accomplished!

After taking a short nap I reconsidered my situation: Yes, it took my much time but at the same time I learned a lot. I am not referring primarily to my speed generating new blogdown websites with a GitHub repo and deployed by Netlify (60 seconds!)  Hopefully I will not need this skill frequently in the future. :smile: In addition to be more comfortable with Git/Github now I learned general strategies to avoid similar problems in the future!

And there are also some encouraging signals from the community: Both --- Georg Cushen and Yihui Xie --- responded almost immediately and in the meanwhile (as a looked up the links of the paragraphs where I reported the problem) the issue seems to be settled. In spite of the insecurity I experienced yesterday I decided to stick with the academic theme. From some other interactions (problems and questions to the theme) I began to trust the George as he is very committed to his theme and very busy to deliver the best product possible. So after a roll back to an older version I began with this article.

## Lesson learned from my own experience

The following list is an attempt to turn my Odyssean experience into constructive advises for other users, but also for myself, for my future me! I am sure it is not complete and maybe in some points faulty. If you disagree or have other, better tips please comment on this post.

In what follows I am not going into details and I take for granted some basic knowledge/experience with RStudio / blogdown / Git / Github and Netlify. To have read the [blogdown book](https://bookdown.org/yihui/blogdown/) is a another obligatory requirement.

### How to choose a theme?

> Do not _only_ focus on functionality and pleasing design. 

Additionally: 

+ Look if the author is currently active. If his/her repo was not updated for several months or later I would not choose this theme.
+ Look at the repo to decide if the author is responsive to reported issues or pull requests (_PRs_ in developer speech).
+ Look if the author provides releases from time to time. This is important if you (like me) are still not comfortable with Git/Github and instead of forking and synchronizing repos are preferring to install updates via ZIP files.
+ Look into the documentation to see if the explanations are comprehensive and up-to-date
+ Investigate if the theme is popular for the kind of community you belong to. This is not easy to be done but improves the changes for help and support trough other users. Look not only at the number of stars and forks in the repo because that could be misleading for your purpose and community. Recherche also if the theme is mentioned in blogs and forums and what kind of community is using this theme.

### How to start working with the theme?

> Do not begin with adapting the design of the theme 

Instead:

+ Start a test site with a test repository and a test netlify deployment
+ Copy the content of `themes/<your-theme-name>/exampleSite` to your project directory. Not the folder itself, but just the content inside (e.g. the folder static, content and the config.toml). Overwrite these files in your project directory --- it is only a site for testing.
+ Read accompanying instructions and go line by line trough the `config.toml` and adapt it to your needs. Make notes why you did which setting. This could helpful later on, when you have a better understanding of the theme but maybe already forgotten you originally considerations.
+ Start writing text in your test site. I recommend to work on real posts or other types of text  you want to publish some day. Choose predominantly use cases which will be typical for your every day work. This advice seems strange as your are working still on a test site. But your time for this work is not lost: You are producing standard text files which can be easily transferred to other sites or themes. And it is important to test the theme under real working conditions.
+ Establish a common workflow and get used to it. Personally I use the following workflow:
  - I start my daily routine with `blogdown:::serve_site()` using the addins plugin (CTRL-S on my machine) provided by the blogdown package. 
  - Then I start writing. After saving the file (which automatically updates the local website), I inspect the result locally in my browser. (I prefer the browser and not the RStudion pane)
  - From time to time --- or whenever something seems wrong or not updated --- I use `Build -> More -> Clean All` followed by `Build Website`
  - After I have finished work to publish I commit and pull the changes to my repo and after some seconds, when netlify has deployed the site I inspect the live result. 
+ After some day of experience with your daily working routine, get accustomed with all the other features of the theme. Even if there are functions you will not need to use it is nice to have an overview what could be possible and what not. This is also important to understand the changes of a new theme version.
+ Not until you feel comfortable with the functionality of the theme and your working habit you should start to adapt the theme. Here it is important to do all your work on your side of the project, meaning **not** under the themes directory. Copy those files your are going to change or add under your home folder of the RStudio project. So you have all your changes separated from the original theme. New versions of the theme will not conflict with your work and you will have all your changes in one place.
+ Only when you have finally arrived at a status where you work could be "officially" launched, change to the real website. Prepare a fresh installation with your theme, with a repo and a new  netlify deployment. 
+ Before you copy the work you have done into your new RStudio project, create a new Git branch and check it out / change to it. If anything goes irreparably wrong (and believe me: eventually in the long term this will be the case!) you have not destroyed your current web presence. After my Odyssey I work with two branches beside master: `config` for bigger changes (new version of the theme, changing the configuration and/or structure of my site) and `blog` for my daily (writing) work. If you decide to merge your branch with master you will have an additional security level as netlify will check **before** your branch is merged with master, if anything went correct and nothing will cause an error. If something went wrong you don't have to confirm the last step for merging your branch.  

### Strategies, if problems appear 

First of all: Keep calm and RTFM!

+ Use Google (or other search engines) to see if other users experienced the same problem. Start your search inquiry with `blogdown <name of your theme> <error message>` or other appropriate combination of content. Most of the time you will get results linked to questions in Stack Overflow or blog posts where users reported about the same or similar problems.
+ If you cannot find appropriate pairs of problem/solution I would now --- after my Odyssean experience --- not yet starting people to bother at discussion fora. Start instead a new reference (test) site with the XMin theme and try to reproduce the problem. If it works there than the problem has to do with your theme or the changes you has made. 
+ If the problem persists then there are still two possibilities: Either you did something wrong or it really is a bug in one of the pieces in the R Markdown machinery. This is now a good time to produce a reproducible example and report the problem at Stack Overflow. You replication on the otherwise empty reference site will help you to focus on the essential problem and will also provide a reproducible example.
