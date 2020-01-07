---
title: "Static Sites"
weight: 2
---

# Static Sites

One of the fastest and easiest ways to get content online is with a static site generator. Particularly for textual content, static site generators like hugo and jekyll allow you to work primarily with markdown documents and minimally (if at all) with code while still having a fairly large amount of control over your site. The main advantage of static site generators is that they are incredibly lightweight and fast. Static sites are, as the name implies, static copies of the html and css needed to produce the page; they therefore do not need to be fetched or built by a server when someone looks at the page and so require minimal resources to serve over the internet. 

## Try it out: at a glance
1. Follow the Quickstart guide for [hugo](https://gohugo.io).
2. Try changing the theme from the default, in order to create a personal portfolio to show off your work. Some themes that you might look at include the [Academic theme](https://themes.gohugo.io/academic/), the [freelancer theme](https://themes.gohugo.io/freelancer/), the coder theme, any of the blog themes -- really, any theme can serve as a starting point. 
3. Add content and customize the page

## The Details

### Set up Hugo

{{< tabs "uniqueid" >}}
{{< tab "MacOS" >}}
# MacOS
The instructions for Mac and Linux are fairly straightforward. For Mac, if you have not installed homebrew, then you should do so. It will make everything much easier: https://brew.sh/
{{< /tab >}}

{{< tab "Linux" >}}

# Linux
If you are using Linux, then you don't need me to explain it to you. 

For the rest of you, switch to Linux (or BSD). It will make this so much easier. 
{{< /tab >}}

{{< tab "Windows" >}}

# Windows
For Windows, the steps are sometimes more complicated, particularly if you are not used to doing things on the command line or in your file structure. A few pointers: 
- make sure to scroll down to the Windows section of the instructions
- familiarize yourself with your directory structure. Most likely you have a main C: directory but then your files are all in C:\Users\yourusername\. This is important as you may get confused when adding the necessary file folders (C:\Hugo, C:\Hugo\bin) in the instructions.
- to help get a feel for the directory structure on your computer AND to help learn the ocommand line, I strongly suggest that you open up your console (or terminal -- just search for it in the search bar or push the windows key while holding r, then type cmd). See hwere you are at the prompt (it will list your current directory). Then use the following commands to navigate a bit:
1. dir will list the contents of a directory
2. cd followed by the name of a nested directory will get you into that directory
3. cd by itself will take you back to your home directory (usually C:\Users\yourusername)
4. cd .. will get you up one level of the directory (cd ..\.. will get you up two levels, cd ../../.. will take you up three and so forth)
{{< /tab >}}
{{< /tabs >}}

# Create a site
As you follow the instructions on the hugo site, a few notes:
- pay particular attention to which directory you are in when you run the hugo new site command. The site will be created as a subdirectory of wherever you are when you execute the command. 
- you can set up a folder to hold your sites or for this class and then build the sites under that folder

# View your site
When you are done with setup, you will preview your site by typing hugo server -D 

Open your browser and type localhost:1313 into the address bar to get to your site.

If you don't see anything, then there's a good chance you haven't added any content yet. Go find the content folder of your site. Also, look at the documentation for the theme and at the example site (usually hosted as a git repository as well) to see where files are kept and how they show up in the example site.

# Modify content
Note that for many blog themes you will find the content under /content/posts

# Markdown
A static site generator takes as input markdown files. These are a form of plaintext file that includes some basic formatting information. For an overview of markdown and cheatsheet, see https://www.markdownguide.org/basic-syntax/

Play around with it and see how formatting is displayed in the rendered site.
