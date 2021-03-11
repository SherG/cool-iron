---
title: What's So Great About the Jamstack?
path: /jamstack
date: 2021-03-10
summary: The impressive performance and simple workflow of Jamstack websites is leaving monolithic apps and practices behind.
tags: ['jamstack''websites']
---

Over a decade ago I managed a website project that transitioned an old legacy ASP.NET site to Drupal. With Drupal, good architecture, and ongoing attention to SEO we achieved a 10,000% traffic boost (one million visitors). More importantly, our key segments were doubling and even tripling their time spent online and viewing more pages. 

I became a Drupal loyalist and evangelist for fastidious SEO. (Ranking is hard-won, easily lost.) After this project I would sometimes be asked in passing, "Which is better: Drupal, WordPress, or Joomla?" While I was a staunch advocate for Drupal (and my favorite Drupal host, Acquia), I learned to avoid entertaining this question. It's overly simplified. And besides, people seem to have already made their mind up anyway.

It's been a long time since I've thought about Drupal. All of the sites I own are now <a href="https://jamstack.org/" target="blank">Jamstack</a> sites that run on Netlify Edge. 

## What is the Jamstack? 

Jamstack is a term coined by Mathias Biilmann to describe a modern approach to web architecture that delivers impressive speed, performance, scalability, security, and ultra-simplified workflows -- all in a cost-efficent way. 

Specifically, JAMstack uses ("stacks") 3 core technologies: JavaScript, APIs, and Markup, i.e., "JAM." This approach began as an organic movement among developers to build websites better aligned with the way the modern web works. They questioned current dogmas, and  jettisoned the use of web apps like WordPress and Drupal, which they viewed as "monolithic." Here, monolithic means inefficient, complicated, and outdated. WordPress and Joomla were the past. They were creating the future web.

JAMstack uses sleek build tools and more importantly, leverages recent advances in browsers.


## How your site gets served to visitors

To understand the difference between the Jamstack approach and the monolithic approach, we can look at how a website is "served" (or "delivered") to a reader. 

When a reader using a browser enters the URL of a 'monolithic app', a lot transpires just to get a single page to that viewer.

Each individual page is built on the fly by making a series of "calls." 

* The reader, using a browser (client), makes a request for a web page. 
* That request passes through multiple stages to get to the database, then makes a round trip back to the browser. 
* Those stages may include a load balancer, a web server, an application server, and one or more databases.
* While the requested web page is being assembled, "calls" may be made to third-party sites that store the fonts, images, videos, or marketing tools used on the site. It's not uncommon for dozens of such third-party calls to be made -- or even 100 or more.
* If a CDN (content delivery network) is being used, then it will cache a version of the page. But any personalization or database requests (triggered, by things like filling out a form, signing up for something, or posting user content) will still need to percolate down the layers and back up again to the browser.

This is what Biilmann rightly terms the Legacy web:

<img src="https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1614574590/SignalFox/evolution-of-web_ynrwep.png">

## A brief comparison

Monolithic apps like WordPress are made up of a "front-end" and "back-end." The front-end includes all the code that creates the visual look and feel of the site. The back-end includes the CMS (content management system) which users log in to, to post, edit articles, upload photos, embed videos, add SEO tags like meta descriptions, and so on. Back-end code and all your site's articles and visual assets are stored in a database.

By contrast, a Jamstack site decouples the visual presentation (the front end) from the back end. Content pages are coded in Markdown. These pages are "prebuilt" and live on global CDN nodes, close to users. Your website's pages are ready to be viewed instantly. Nothing needs to be built on the fly. 

Biilmann recalls that Aaron Swartz referred to this general concept as "<a href="http://www.aaronsw.com/weblog/000404" target="blank">Bake, don't fry</a>."

Note that all the pages have been pushed out close to end-users: the CDNs are the first "ping" the browser will make, and the content will be immediately delivered to the browser.

Dynamic elements are simply dealt with differently than with Drupal or WordPress. Modern browsers now process JavaScript right in the client and make API calls as well. Any dynamic page elements will be processed in the browser itself, which can make calls to third-party APIs like Stripe for payments. 


## Decoupling your WordPress or Drupal site

I'm sold on the JAMstack and on Netlify's leadership in this arena. <a href="https://www.netlify.com/products/edge/">Netlify's interface</a> for deploying your site online beats anything I've ever seen in terms of easy of use, simplicity, performance, and low cost.

But if you have a Drupal or WordPress site you can gain some advantage by decoupling your front-end from your back-end. For example, see <a href="https://www.netlify.com/with/drupal/?">this guidance from Netlify</a> and <a href="https://www.acquia.com/resources/decoupled-drupal">this from Acquia</a>.

## When you have to stick with your CMS

For cost reasons, a business with a complicated site that's running many marketing tools and custom code and has already been build in WordPress or Drupal, may need to stick with what they've got. 

But don't let that deter you from improving your speed and performance. After a redesign, <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fdigital.com%2F&tab=mobile">this massive WordPress site</a> is loading in under a second on desktop and under 3 seconds on mobile. 

If you're serious about Drupal performance, <a href="https://www.acquia.com/">go with Acquia</a>. If you need to do some preliminary research, browse <a href="https://www.whoishostingthis.com/hosting-reviews/">review sites</a> to learn more about hosting. Then talk to developers or agencies who manage WordPress sites that are scoring at 97-100/100 on <a href="https://developers.google.com/speed/pagespeed/insights/">Google Page Speed Insights</a>. Skip the agencies producing anything below exceptional Google Page Insight scores. 

Tip: If you're new to Google Page Speed Insights, realize that there is some natural fluctuation in scores: you may click their "Analyze" button 3 times in a row and get slightly different scores. Also realize that you should click it several times if you see a low score, because ocassionally there's a "hiccup" in their stats and an ultra-fast site will temporarily display a mediocre score.
