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

Specifically, JAMstack uses (or "stacks") 3 core technologies: JavaScript, APIs, and Markup, i.e., "JAM." This approach uses sleek tools and leverages recent advances in browsers.

This approach began as an organic movement among developers to build websites better aligned with the way the modern web works. They questioned current dogmas, and  jettisoned the use of web apps like WordPress and Drupal, which they viewed as "monolithic." Here, monolithic means inefficient, complicated, and outdated. WordPress and Joomla were the past. They were creating the future web.

This questioning spirit seems to have also impacted the visual design of JAMstack sites: the best inspire you to avoid redundancies and engage in structured thinking about what problems you want your website to solve. 

## Speed and Security

To understand the difference between the Jamstack approach and the monolithic approach, we can look at how a website is "served" (or "delivered") to a reader. 

"Monolithic" apps like WordPress, use as set of technologies called the LAMP stack: Linux, Apache Web Server, MySQL databases, and PHP.  Critically, when a reader using a browser enters the URL of a LAMP stack site, a lot transpires just to get a single page to that viewer.

Each individual page is built on the fly by making "calls" to locations where the various pieces of a page are stored. For example a sidebar might visually appear to be on that page, but is actually being "called" from another location in the database. "Calls" might also be made to fetch third-party content, like images or fonts or marketing tools. It's not uncommon for dozens -- or even 100 or more -- "calls" to have to be made, to generate a single web page, which is then sent to the browser. 

Here's a typical process:

* The reader, using a browser (client), makes a request for a web page. 
* That request passes through multiple stages to get to the database, then makes a round trip back to the browser. 
* Those stages may include a load balancer, a web server, an application server, and one or more databases.
* If a CDN (content delivery network) is being used, then it will cache a version of the page. But any personalization or database requests (triggered, by things like filling out a form, signing up for something, or posting user content) will still need to percolate down the layers and back up again to the browser.

This is what Biilmann rightly terms the Legacy web:

<img src="https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1614574590/SignalFox/evolution-of-web_ynrwep.png">

Furthermore, 'monolithic' apps are made up of a "front-end" and "back-end." The front-end includes all the code that creates the visual look and feel of the site. The back-end includes the CMS (content management system) which users log in to, to post, edit articles, upload photos, embed videos, add SEO tags like meta descriptions, and so on. Back-end code and all your site's articles and visual assets are stored in a database.

By contrast, a Jamstack site decouples the visual presentation (the front end) from the back end, which it does away with entirely. 
Content pages are coded in Markdown. These pages are "prebuilt" and live on global CDN nodes, close to users. The pages are ready to be viewed and nothing needs to be built on the fly. Biilmann recalls that Aaron Swartz referred to this general concept as "<a href="http://www.aaronsw.com/weblog/000404" target="blank">Bake, don't fry</a>." Pushing that analogy, we might ask, "Do you want to cook an entire meal from scratch once your visitors arrive or do you want to have it ready to serve?"

Note that all the pages have been pushed out close to end-users: the CDNs are the first "ping" the browser will make, and the content will be immediately delivered to the browser.

Now you may be thinking: that's a static website. Yes, but only part of the site is static. Dynamic elements are simply dealt with differently. Modern browsers now process JavaScript right in the client and make API calls as well. Any dynamic page elements will be processed in the browser, which call also make calls to third-party APIs like Stripe for payments. 


## How do you scale up a monolithic app? 

So-called monolithic apps often need to add hosting infrastructure in order to scale. This must be handled by a professional which can become time-intensive. There are also "managed hosting" services you can purchase, but what that actually includes varies widely between providers. 

Choosing the right hosting approach requires a bit of knowledge. Choose poorly and your site may crash during a big traffic surge. 

## Developer experience 
