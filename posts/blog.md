---
title: "How I made this blog"
date: "2020-11-03"
draft: false
path: "/posts/blog"
tags: "Engineering", "Product Management"
---

This is the obligatory “how I made this blog” post. This is not the prettiest or most user- (or maker-, for that matter lol) friendly blog, but I had some specific goals, and this was a fun way to meet those goals. I’ll expound below on my goals, in order of priority: 

1. FREE. Full stop.
2. I want to own the content I create.
3. I don’t want to worry too much about the visual design or building backend services.
4. It would be nice to avoid having another CMS to manage.

As you can probably guess, these criteria remove a lot of awesome potential tools from the running. But lets go through each if you’re curious why. 

# Decision Factors

## Price
Stingy-ness here is all about my expectations. If I were expecting millions of visitors, thousands of blog posts, detailed tagging needs, or the like, this criteria might not be here. But this for me is a hobby project, where I can practice my thinking, writing, maybe have some people follow along.

Along with the low expectations, this is a fairly saturated space. A quick Google search reveals tons of products to help build a blog, many with free tiers. For my expectations, one of these ought to be sufficient. Although I’d love to not have a completely lame domain name, which could be tricky at this price tier of NOPE. 

Lastly, if I wanted a more capable platform that would required some features that were only available on a paid tier, I would skip these alternatives altogether and just build my own. I’ve made many websites that are much more complex and detailed, and I’m far too cheap to pay a few bucks a month when I could do it myself. Cue Seinfeld referenced: [“Why pay for it when you can apply yourself, and then maybe you can get it for free?”](https://youtu.be/AcqEcYVmiPU)

## Ownership
I’ve heard too many horror stories of people using a platform to host their content (be it a blog, photos, music, etc) and have the platform change (shut down, change restrictions, require logins, paywall, etc) and they are disappointed. Perhaps this is a superstition or I’m being overly cautious and making readers and myself suffer for it, but oh well. Again, this is a hobby project more than a real monetization platform. Also, I sometimes have this weird thing about liking to *own* things and feel like they are *mine*, like a small corner of my room being “mine”. Maybe its a just result of growing up the youngest of seven kids, or maybe I just have some deeper stuff to work through there, but I’ll leave that for another day 🙃.

## Design
I am a recovering perfectionist, and very strongly believe the “great is the enemy of the good” mantra. I know myself, and while I have some strong design opinions, I suffer from some decision-paralysis when presented with too many options. Also, something I just like looking at pretty/interesting/cool things. I could ~spend~ waste HOURS looking through different Wordpress designs and swing violently between emotions of pleasantly enjoying myself and stressing la horribly with 50 tabs open stuck between which was is really *me*. If I were to venture into designing it myself, a similar thing could happen. I’d be at risk of getting lost tinkering with some button placement and distract from the real goal, which is to work on my writing and thinking, and communicate some of the thoughts along the way.

Backend services here is a similar thing. I’d feel very comfortable designing and building a database, infrastructure, API, and connectors all-around- its something I’ve done on much larger scales and for much higher stakes situations. But I just didn’t feel like doing it here. I didn’t want to worry about that stuff because I felt it would distract from what my real goal was here.

## CMS-less
This is another thing about goals and kinda some (likely mis-directed) laziness. This wasn’t a full NO WAY thing, but mostly like, it’d be nice to not learn another tool, have another account, get locked to some propriety platform (See “ownership”), or whatever. CMSs are LIFE, but this hobby project probably doesn’t necessitate one right now. Maybe when I get to like 100 untagged posts that are totally unreadable, I’ll have to move over and resolve the tech debt then, but that won’t be a terrible mountain to climb if I get to that point, so I’ll live light-weight now.

All that, some research and recommendations from friends, and this is where I ended up:

# Finalists

## First place: [Gatsby](https://www.gatsbyjs.com)

- Price: Free!
- Ownership: Yes!
- Design: Lots of great themes available, lots of customization potential if I want it. Backend and infrastructure is a few easy clicks. 
- CMS-less: Mostly 

Lots of recommendations from friends pointed me here. Gastby is SO COOL. There are a lot of cool tools on the internet, but this one stood out to me because of the paradigm it has about how to build really made sense to me. I’ll let them to the explaining, so navigate over there if you want to learn more.This is probably the best balance between me using an existing product, but being able to customize a bit to get exactly what I wanted.  The integration with netlify is great, and it really seems like Gatsby just thought through everything right. Can’t recommend it enough.

## Second place: [Wordpress](https://wordpress.com/create-blog/)

- Price: Free!
- Ownership: Yeah basically
- Design: Great themes available, easy to manage
- CMS-less: Not really

This is the “get over yourself” part. If my goal is really just to write and think, and I don’t want to worry about code/infrastructure/cms, shouldn’t I just grab a free tool off the shelf? And its industry standard, and I have some experience with it. I could get going in minutes. Seems obvious.

## Third place: [Github Pages](https://pages.github.com) + Jekyll with md files

- Price: Free!
- Ownership: Yes!
- Design: Only like 8 themes available, they’re pretty good. No worry at all about backend for better or worse
- CMS-less: Yes!

I didn’t know this option was a thing until late in the game. This is a really cool thing Github Pages has built, targeting mostly at devs who want to add MD file-based documentation to their projects. You can build a whole website as a sub-project on your Github Pages domain, served with Jekyll. Right in your repository settings, you can add it to your Github Pages site, choose a theme, and just add your .md files. Zero code, not hadly customizable, and clunky as a blog. But pretty cool.

# Decisions

I started building a Gatsby project since it was the winner in my eval. In an hour of tinkering and having some fun, I had a great site running just like I’d like on my local machine, and all indications were that deployment was going to be a breeze. But I got cold feet for no good reason. Maybe it was avoiding setting up a netlify account, or maybe it was some indecision on a few design points, but I just kinda sat on it for a weekend or so while I thought it over. I considered Wordpress during this time, and I was met with the same cold feet. Maybe the domain and CMS slowed me down? 

Anyhow, that’s when option 3 popped up. I really like the idea of using MD files as my blog content, and I really like the idea of hosting it out of Github. And I really like Github Pages. Where has this been my whole life? 

Turns out my little throw in about not having a weird domain (and not paying for one lol) probably played a bigger factor than I’d care to admit, but between everything, I decided I’d roll up my sleeves a bit and use (Github Pages)[https://pages.github.com] to host something I had some hand in building myself. Partially because I could, but mostly because Github Pages is just so cool.
 
So for no great reason, but a lot of probably lame ones, I decided this was the way to go. I chose a theme (easy, cause there were only 8), decided I could live with the lack of customization and tech debt I might be building up, but more than anything, I just liked the solution. And after all, this is a hobby project! Liking it is the whole point! So I made it happen. 

Go check out the repository and you can see the structure. A single one-line config file (that was auto-generated haha), and some md files. All I do now is add a new file, and a link on the homepage to the new blog post (tech debt is why we all have jobs, right??). Another fun thing is I can do all this through the browser (either with Github’s normal UI or Codespaces). I don’t even have the repo stored on my machine right now. And all my posts a change-managed with Git which is completely unnecessary but kinda neat!

Later, I’ll likely see what simple customizations I can add to Jekyll with, which Github has some docs on (and what they support, Jekyll is MUCH more than what I/they are using for here). But until that day, I’m pretty happy! It’s not great, its not even perfect by any means, but its effective, it was fun and easy to setup, and I learned some new stuff! 
