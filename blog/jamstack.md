---
title: What's So Great About the JAMstack?
path: /jamstack/
date: 2021-03-10
summary: The impressive performance and simple workflow of JAMstack websites is leaving monolithic apps and practices behind.
tags: ['jamstack','websites']
---

Over a decade ago I managed a website project that transitioned an old legacy ASP.NET site to Drupal. With Drupal, good architecture, and <a href="/seo-set-forget">ongoing attention to SEO</a> we achieved a 10,000% traffic boost (one million visitors). More importantly, month-over-month our key segment metrics were increasing by double-digit precentages. We also saw, over quarters, a doubling or even tripling of key segment time spent online and and in page depth. 

I became a Drupal loyalist. After this project I would sometimes be asked in passing, "Which is better: Drupal, WordPress, or Joomla?" While I enjoyed these discussions, I learned to avoid entertaining the question. It's overly simplified. 

It's been a long time since I've thought about Drupal. From 2019, all of the sites I own are now <a href="https://jamstack.org/" target="blank">Jamstack</a> sites that run on <a href="https://www.netlify.com/" target="blank">Netlify Edge</a>. 

## What is the Jamstack? 

JAMstack is a term coined by Mathias Biilmann, co-founder and CEO of Netlify, to describe a modern approach to web architecture that delivers impressive speed, performance, scalability, security, and ultra-simplified workflows — at low cost.

Specifically, JAMstack uses ("stacks") 3 core technologies: JavaScript, APIs, and Markup, i.e., "JAM." It also uses sleek build tools that developers love. More importantly, it leverages recent advances in browsers.

This approach began as an organic movement among developers to build websites that delivered optimal user experience and were better aligned with the way the modern web works. They questioned current dogmas, and jettisoned the use of apps like WordPress and Drupal, which they viewed as "monolithic." Here, monolithic means inefficient, complicated, and outdated. WordPress and Joomla were the past. They were creating the future web.

## How your site gets served to visitors

To understand the difference between the Jamstack approach and the monolithic approach, we can look at how a website is "served" (or "delivered") to a reader. This requires a basic understanding of how web hosts work. (<a href="https://www.whoishostingthis.com/hosting-reviews/" target="blank">Explore this site</a> to learn  about web hosts and how hosting works.)

When a reader using a browser enters the URL of a 'monolithic app', a lot transpires just to get a single page to that viewer.

Each individual page is built on the fly by making a series of "calls." 

* The reader, using a browser (client), makes a request for a web page. 
* That request passes through multiple stages to get to the database, then makes a round trip back to the browser. 
* Those stages may include a load balancer, a web server, an application server, and one or more databases. A CDN may also be used.
* While the requested web page is being assembled, "calls" may be made to third-party sites that store the fonts, images, videos, or marketing tools used on the site. It's not uncommon for dozens of such third-party calls to be made — or even 100 or more.
* If a CDN (content delivery network) is being used, then it will cache a version of the page. But any personalization or database requests (triggered, by things like filling out a form, signing up for something, or posting user content) will still need to percolate down the layers and back up again to the browser.

This is what Biilmann rightly terms the Legacy web. 

<img src="https://res.cloudinary.com/icecloud7/image/upload/f_auto/v1614574590/SignalFox/evolution-of-web_ynrwep.png">

## A brief comparison

Apps like WordPress are made up of a "front-end" and "back-end." The front-end includes all the code that creates the visual look and feel of the site. The back-end includes the CMS (content management system) which users log in to, to post, edit articles, upload photos, embed videos, add SEO tags like meta descriptions, and so on. Back-end code and all your site's articles and visual assets are stored in a database.

By contrast, a Jamstack site decouples the visual presentation (the front end) from the back end. Content pages are coded in Markdown. These pages are "prebuilt" and live on global CDN nodes, close to users around the world. Your website's pages are ready to be viewed instantly. Nothing needs to be built on the fly. 

![website design](../static/web-design.svg)

### Bake, don't fry 

JAMstack repects the efficient design inherent in the early web, and it has roots in static site development. Biilmann recalls that Aaron Swartz referred to the underlying concept as "<a href="http://www.aaronsw.com/weblog/000404" target="blank">Bake, don't fry</a>." 

Static sites have existed for decades. But it would be incorrect to perceive JAMstack as a throwback. While JAMstack uses the term "static" (as in "static site generators" or "static sites") not every static site is a JAMstack site.

Dynamic elements exist in JAMstack sites - they're just dealt with differently than in Drupal or WordPress. Modern browsers now process JavaScript right in the client and make API calls as well. Any dynamic page elements will be processed in the browser itself, which can make calls to third-party APIs like Stripe for payments. 

What about CMSs for JAMstack? There are many now to choose from, including Forestry and Contentful. Even Netlify has one — made up of a single page of React code.

<details>
  <summary>What is React?</summary><br/>
   <ul class="highlight2">
     <li>React is an <a href="https://reactjs.org/docs/how-to-contribute.html" target="blank">open source JavaScript library, created by Facebook engineers</a>. It's used to create fast, interactive user-interfaces.</li>
 </ul>

</details>
<br/>
<details>
  <summary>What is a JavaScript library?</summary><br/>
   <ul class="highlight2">
     <li>A JavaScript library is a collection of pre-built JavaScript functions. Using pre-built functions speeds the development process: the programmer doesn't need to build everything from scratch .</li>
 </ul>

</details>

I'm sold on the JAMstack and on Netlify's leadership in this arena. <a href="https://www.netlify.com/products/edge/">Netlify's interface</a> for deploying your site online beats anything I've ever seen in terms of ease of use, simplicity, performance, and low cost.
<br/>
> "Within 5 years, you'll build your next large scale, fully featured web app with JAMstack and deploy on Netlify." <br/>
<small>—  GitHub founder and CEO Tom Preston-Werner, in 2018</small>

<br/>
<br/>
In sum, JAMstack could've been designed by Steve Jobs: it seeks to remove everything inefficient, unnecessary, and unsupportive of a beautiful and performant experience. In doing so, it cuts across the grain of the status quo.


## When you want to stick with your CMS

For cost or functionality reasons, some businesses may want to stick with their current CMS. For example, a business with a complicated site that's running multiple marketing tools and custom code and has already been built in WordPress or Drupal, may want to continue with their investment in their CMS.

But don't let that deter you from improving your speed and performance. After a redesign, <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fdigital.com%2F&tab=mobile" target="blank">this massive WordPress site</a> made impressive speed gains.

And if you have a Drupal site, consider Acquia for hosting. Tap their staff expertise. I did so for the 2010 site I mentioned, and after following their recommendations at the time (Varnish and Pressflow for a Drupal 6 site) was amazed by the results.


### Decoupling your WordPress or Drupal site

If you have a <a href="https://www.drupal.org/" target="blank">Drupal</a> or WordPress site you can also obtain some benefits of JAMstack by decoupling your front-end from your back-end. This will give you what's called a headless CMS. 

(Biilman considers decoupling a monolithic app to be an <em>adaptation</em> to the JAMstack that is less-than-ideal.)

For more information on decoupling, see:
* <a href="https://www.netlify.com/with/drupal/?" target="blank">This guidance from Netlify</a>
* <a href="https://www.acquia.com/resources/decoupled-drupal" target="blank">This from Acquia</a>
* <a href="https://pantheon.io/features/decoupled-cms" target="blank">This from Pantheon</a>.

## What is JAMstack's maturity?

In my next article, I'll drill down on the JAMstack-WordPress-Drupal comparisons, discuss where I think JAMstack needs to head to obtain significant market share from non-developers, and float some ideas for decision-making. 

I'll also share what small business scenarios the JAMstack might be ideal for. 

One more note: What's my Netlify bill for 2 years of blazingly fast JAMstack sites? $0.00. Priceless. 


