---
title: What's So Great About the JAMstack?
path: /jamstack
date: 2021-03-10
summary: The impressive performance and simple workflow of JAMstack websites is leaving monolithic apps and practices behind.
tags: ['jamstack','websites']
---

Over a decade ago I managed a website project that transitioned an old legacy ASP.NET site to Drupal. With Drupal, good architecture, and ongoing attention to SEO we achieved a 10,000% traffic boost (one million visitors). More importantly, our key segments were doubling and even tripling their time spent online and viewing more pages. 

I became a Drupal loyalist. After this project I would sometimes be asked in passing, "Which is better: Drupal, WordPress, or Joomla?" While I enjoyed these discussions, I learned to avoid entertaining the question. It's overly simplified. 

It's been a long time since I've thought about Drupal. From 2019, all of the sites I own are now <a href="https://jamstack.org/" target="blank">Jamstack</a> sites that run on <a href="https://www.netlify.com/">Netlify Edge</a>. 

## What is the Jamstack? 

Jamstack is a term coined by Mathias Biilmann to describe a modern approach to web architecture that delivers impressive speed, performance, scalability, security, and ultra-simplified workflows --- at low cost.

Specifically, JAMstack uses ("stacks") 3 core technologies: JavaScript, APIs, and Markup, i.e., "JAM." It also uses sleek build tools that developers love. More importantly, it leverages recent advances in browsers.

This approach began as an organic movement among developers to build websites that were better aligned with the way the modern web works and that delivered optimal user experience. They questioned current dogmas, and jettisoned the use of web apps like WordPress and Drupal, which they viewed as "monolithic." Here, monolithic means inefficient, complicated, and outdated. WordPress and Joomla were the past. They were creating the future web.

## How your site gets served to visitors

To understand the difference between the Jamstack approach and the monolithic approach, we can look at how a website is "served" (or "delivered") to a reader. This requires a basic understanding of how web hosts work. (<a href="https://www.whoishostingthis.com/hosting-reviews/" target="blank">Explore this site</a> to learn  about web hosts and how hosting works.)

When a reader using a browser enters the URL of a 'monolithic app', a lot transpires just to get a single page to that viewer.

Each individual page is built on the fly by making a series of "calls." 

* The reader, using a browser (client), makes a request for a web page. 
* That request passes through multiple stages to get to the database, then makes a round trip back to the browser. 
* Those stages may include a load balancer, a web server, an application server, and one or more databases. A CDN may also be used.
* While the requested web page is being assembled, "calls" may be made to third-party sites that store the fonts, images, videos, or marketing tools used on the site. It's not uncommon for dozens of such third-party calls to be made -- or even 100 or more.
* If a CDN (content delivery network) is being used, then it will cache a version of the page. But any personalization or database requests (triggered, by things like filling out a form, signing up for something, or posting user content) will still need to percolate down the layers and back up again to the browser.

This is what Biilmann rightly terms the Legacy web.

<img src="https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1614574590/SignalFox/evolution-of-web_ynrwep.png">

## A brief comparison

Monolithic apps like WordPress are made up of a "front-end" and "back-end." The front-end includes all the code that creates the visual look and feel of the site. The back-end includes the CMS (content management system) which users log in to, to post, edit articles, upload photos, embed videos, add SEO tags like meta descriptions, and so on. Back-end code and all your site's articles and visual assets are stored in a database.

By contrast, a Jamstack site decouples the visual presentation (the front end) from the back end. Content pages are coded in Markdown. These pages are "prebuilt" and live on global CDN nodes, close to users around the world. Your website's pages are ready to be viewed instantly. Nothing needs to be built on the fly. 

![website design](../static/web-design.svg)

### Bake, don't fry 

Biilmann recalls that Aaron Swartz referred to the underlying concept as "<a href="http://www.aaronsw.com/weblog/000404" target="blank">Bake, don't fry</a>."

Note that all the pages have been pushed out close to end-users: the CDNs are the first "ping" the browser will make, and the content will be immediately delivered to the browser.

Dynamic elements are simply dealt with differently than with Drupal or WordPress. Modern browsers now process JavaScript right in the client and make API calls as well. Any dynamic page elements will be processed in the browser itself, which can make calls to third-party APIs like Stripe for payments. 

What about CMSs for JAMstack? There are many now to choose from: Forestry, Contentful, Strapi, and even Netlify has one --- made up of a single page of React code.

I'm sold on the JAMstack and on Netlify's leadership in this arena. <a href="https://www.netlify.com/products/edge/">Netlify's interface</a> for deploying your site online beats anything I've ever seen in terms of easy of use, simplicity, performance, and low cost.

## Decoupling your WordPress or Drupal site

But if you have a Drupal or WordPress site you can still obtain some benefits of JAMstack by decoupling your front-end from your back-end. This will give you what's called a "headless CMS." Biilman considers this to be an "adaptation" to trends fostered by JAMstack.

For more information, see <a href="https://www.netlify.com/with/drupal/?">this guidance from Netlify</a> and <a href="https://www.acquia.com/resources/decoupled-drupal">this from Acquia</a>.

## When you want to stick with your CMS

For cost or functionality reasons, a business with a complicated site that's running many marketing tools and custom code and has already been build in WordPress or Drupal, may need to stick with what they've got. 

But don't let that deter you from improving your speed and performance. After a redesign, <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fdigital.com%2F&tab=mobile">this massive WordPress site</a> made significant speed gains.

If you're serious about Drupal performance, <a href="https://www.acquia.com/">go with Acquia</a>. More importantly, consult with them on the best way to get optimal speed with your Drupal site. They're experts. I tapped their expertise back when I was managing the Drupal site I mentioned earlier. And I was amazed by the speed and performance results. 

Talk to developers or agencies who manage WordPress sites that are scoring at 97-100/100 on <a href="https://developers.google.com/speed/pagespeed/insights/">Google Page Speed Insights</a>. Skip the agencies producing anything below exceptional Google Page Insight scores. 

<em>Note: If you're new to Google Page Speed Insights, realize that there is some natural fluctuation in scores: you may click their "Analyze" button 3 times in a row and get slightly different scores. Also realize that you should click it several times if you see a low score, because ocassionally there's a "hiccup" in their stats and an ultra-fast site will temporarily display a mediocre score.</em>

## What is JAMstack's maturity?

In my next article, I'll drill down on the JAMstack-WordPress-Drupal comparisons, discuss where I think JAMstack needs to head to obtain significant market share from non-developers, and float some ideas for decision-making. 

I'll also share what small business scenarios the JAMstack might be ideal for. 

One more note: my hosting bill for 2 years of blazingly fast JAMstack sites is ... $0.00. Priceless. 




