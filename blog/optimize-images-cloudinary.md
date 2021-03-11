---
title: How to Use Cloudinary to Optimize Images
path: /optimize-images-cloudinary
date: 2019-04-05
summary: Optimizing your website images can give you quick speed gains. Learn how to use Cloudinary to set up automatic image optimization.
tags: ['website optimization', 'images']
---

![optimize images](../static/optimize-images.svg)

When it comes to slow website loading speeds, images are usually the biggest culprit. Optimizing your images is an important first step to improving your site's speed and performance. 

Cloudinary automatically optimizes your images for you, serving the best image format and right quality to each individual user based on their browser, device type, and screen size. 

In this article, you'll learn how to set up Cloudinary and use it for your own website. 
<hr>
<strong>Skills required</strong>: Basic computer literacy. Basic knowledge of HTML. Basic knowledge of working with files and folders. 
<hr>

## Why Is Website Loading Speed Important?  

Research by Google and other firms has shown that website page load times directly impact revenue, engagement, conversions, and time spent on sites. Sluggish pages or delayed interaction may be interpreted by the user as a poor experience. 

Here's a snapshot of relevant data: 

* A 1-second delay in page load time can decrease conversions by 7% or more. (Source: Akamai)
* As a page's site loading speed goes from 1 second to 6 seconds the likelihood that the visitor trying to access the page will abandon it, goes up by 106%. (Source: Google / SOASTA research)

> Speed, performance, and SEO is where key competitive gains can be had.

## Optimizing Images: Choosing an Approach

In addition to boosting your web page load times, optimizing your images can reduce your bandwidth costs. 

There are many ways to optimize online images. Some approaches require advanced coding or image knowledge. All strive to achieve a balance between maximum image quality and miminal file size. 

In this article, I'll be <a href="#start">sharing a technique</a> for optimizing your images that presents the highest opportunity to most users: it requires low effort, little technical knowledge, and typically results in high impact on load times. 

### Get Started Now

<a href="#start">Click here</a> to skip the background information and jump right into optimizing your images.


### Optimizing for Format and Quality

The two tactics we'll be using relate to <u>image format</u> and <u>image quality</u>. 

#### Next-Gen Formats

Image formats like JPEG and PNG are common but their file sizes are often not economical.

When testing a website using <a href="https://developers.google.com/speed/pagespeed/insights/" target="blank">Google Page Speed Insights</a>, the results will often warn "Serve images in next-gen formats." (For example, see this  <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.wired.com%2F&tab=mobile" target="blank">Google Page Speed test for Wired.com</a>. The test flags images that don't use next-gen formats.)

Next-gen formats compress images down to a smaller file size while preserving visual quality. The display size of the image doesn't change. 

WebP, JPEG 2000, and JPEG XR are examples of next-gen formats. 

#### The Browser Compatability Problem — Solved
<a href="https://developers.google.com/speed/webp/" target="blank">WebP</a> was developed by Google. It loads extremely fast, but is <a href="https://caniuse.com/#search=webp" target="blank">not supported by all browsers</a>. 

For example, it's not compatible with Safari, iOS Safari, BlackBerry Browser, or IE Mobile. <em>If all of your website images were WebP images, visitors coming to your website using one of these other browsers would see blank spaces where the images were supposed to be.</em>

In addition, formats like <a href="https://caniuse.com/#feat=jpegxr" target="blank">JPEG XR</a> are only supported by Microsoft's Internet Explorer and Edge browsers. 

You can see how browser compatibility issues complicate our goal to serve images that load fast.

<strong>The Solution</strong>: Cloudinary can automatically detect what browser a site visitor is using, and then serve the images on that web page in a format that's optimal for that browser — all in real-time.

#### Image Quality

Cloudinary can also use its algorithms to calculate and deliver image quality based on the image content and the end-user's browser and device. The algorithm achieves the best balance between low file size and visual quality. 


![cloudinary homepage] (https://res.cloudinary.com/icecloud7/image/upload/f_auto/v1565472385/SignalFox/cloudinary-image-optimization_imj3ym.png)

## <a href id="start">Getting Started With Cloudinary</a>


1. Sign up for a <a href="https://cloudinary.com/" target="blank">Cloudinary account</a>. (There's a free developer tier that allows for 25 GB of storage or "net viewing bandwidth.")
2. Log in to your new account and click on "Media Library." 
3. Upload an image. (Tip: If you're going to use Cloudinary for multiple websites, create a folder in Media Library for each website.)
4. Hover your cursor over the image and a paper clip icon will appear in the upper left corner. Click on the paperclip icon. This causes the image URL to be copied. 
5. Paste the URL into an new browser window. 


As an example, I'm going to use the URL for the Cloudinary website image that appears above this section. 

After uploading the image to Cloudinary, I click on the paperclip icon to copy this URL:

```html
https://res.cloudinary.com/icecloud7/image/upload/v1565472385/SignalFox/cloudinary-image-optimization_imj3ym.png
```

Then I place the URL in a browser window. You'll see the image appear.

### Adding f_auto and q_auto

Now we're going to add the <mark class="highlight">f_auto</mark> and <mark class="highlight">q_auto</mark> parameters to this URL. 

* f_auto tells Cloudinary to automatically transform this image into a file format that's optimal for the user's browser.
* q_auto tells Cloudinary to automatically deliver the image at a quality level suitable for the device accessing the web page. 

Insert <mark class="highlight">f_auto</mark> and <mark class="highlight">q_auto</mark> after the `/upload/` trailing slash, like so:

``` html
https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1565472385/SignalFox/cloudinary-image-optimization_imj3ym.png
```

* The order of the parameters doesn't matter
* Place a comma between the parameters
* Don't add any spaces

#### Insert the New Image URL Into Your Web Page

Next, in the HTML of your web page, you're going to swap out your old image URL and replace it with your new image URL from Cloudinary.

For this example, let's assume that I originally uploaded a PNG version of this image on my web page. The HTML for my page might look like this: 

``` html
<p>Cloudinary can also use its algorithms to calculate and deliver image 
quality based on the image content and the end-user's browser and device. 
The algorithm achieves the best balance between low file size and visual 
quality.</p>

<img src="/assets/cloudinary-image-optimization.png" />

<h2> Getting Started With Cloudinary </h2>

```

Next, replace the old image URL with your new image URL from Cloudinary. 

``` html
<p>Cloudinary can also use its algorithms to calculate and deliver image 
quality based on the image content and the end-user's browser and device. 
The algorithm achieves the best balance between low file size and visual 
quality.</p>

<img src="https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1565472385/SignalFox/cloudinary-image-optimization_imj3ym.png" />

<h2> Getting Started With Cloudinary </h2>

```

### Additional Tips

You can't go wrong with f_auto. It's really all you need to do to dramatically improve your image delivery. That results in a better user experience. 

Cloudinary offers dozens of image transfomations, but for optimization and speed f_auto is the most important one. 

If you're curious about other parameters, here are two more to explore:

* <mark class="highlight">w_auto</mark> - This parameter instructs Cloudinary to make copies of your image to match the breakpoints of your website. It stores those other images and serves them up as necessary. 
* <mark class="highlight">e_sharpen</mark> - If your image lacks crispness, you can add this parameter to sharpen it. (Note: Check to see the visual result before adding this permanently to your image URL. On occassion, the sharpening looks a bit exaggerated.)

<details>
  <summary>What's a breakpoint?</summary><br/>
  <p>A breakpoint is a browser width setting, coded into a website, that triggers a re-arrangement of responsive design elements. In everyday language, breakpoints are used to allow your site to "re-arrange" itself so that it looks good on different screen sizes. Breakpoints are commonly set (at minimum) for tablets and mobile phones. The purpose of breakpoints is to offer 3 (or more) design options for a website, one that's optimal for common device screen sizes. </p>
</details>

### What Next? 

You should optimize (at minimum) the images on your main landing pages any pages designed for conversion. 

If you have multiple people posting to your blog, then you'll need to train them on using Cloudinary, or assign one individual to handle images. 

A decent workaround for a multi-author blog is to have authors create screen grabs of images they want to use. As they take the screen grab, have them size it by eye (roughly) to fit the width of your blog's text column. By using screen grabs and avoiding huge image sizes, you'll saving on image loading time. 

You won't get the same results as using Cloudinary, but the results should be much better than letting users upload any image file size they want.


## Summary

You've learned that images are typically the biggest problem creating a poor user experience for your website's visitors. That experience directly impacts your engagement, conversions, and ROI.

Optimizing your images with Cloudinary can significantly improve end user experience.

As you're working on your image optimization, feel free to contact me with any questions you might have. 

