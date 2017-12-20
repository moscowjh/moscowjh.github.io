---
layout: post
title:  "Perceived Complexity!"
---
One of the reasons I created this blog is that a number of tech sites have recommended Jekyll as simpler, faster and cheaper than popular CMS systems such as WordPress.  The goal is to test whether that is true for a technically savvy, but inexperienced developer.

Writing and deploying these first few posts has taught me that complexity is "in the eye of the beholder."

- Writing posts in Markdown using a text editor is indeed drop-dead simple assuming the user has a standard developer set-up on her machine. Most tech-savvy editorial, media or executive workers do not have this and are probably disinclined to learn yet another new tool.
- Ran into my first "gotcha" when I decided to include a photo on my About page. Jekyll includes very basic handling of images or other "static assets."  More advanced image handling such as responsive images, photo galleries or optimizing image size requires wading through documentation, installing plug-ins and adding parameters to front-matter.  I used the basic method to include a photo of me.
- Using the default "minima" theme requires only installing Jekyll itself, done by running a few simple command-line scripts. However, as the name suggests, "minima" is very basic.  Installing other themes is another project to be covered later.
- So far, the site has been running on a local webserver on my development machine. Next step is to figure out how to deploy remotely to AWS and GitHub pages.
