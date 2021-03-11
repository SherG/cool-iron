---
title: How to Add SMS to Your Marketing Mix
path: /sms-marketing
date: 2019-03-17
summary: Adding SMS (text messaging) to your marketing mix doesn't need to be time or labor intensive. Here's how to add it to the Autopilot marketing automation platform. 
tags: ['mobile marketing']
---

<a href="https://learn.g2.com/sms-marketing-statistics" target="blank">Ninety-eight percent</a> of text messages are read and most (90%) are read within 3 minutes.

Adding SMS (text messaging) to your marketing mix doesn't need to be time or labor intensive.

You'll appreciate this approach, especially if you're concerned about adding another layer to your marketing stack and keeping all your channel activity tied to an integrated plan and aligned with your top objectives.

First, some basics.

![background](../static/sms-marketing.svg)
 

## When to Use SMS

Use SMS as infrequently as possible while still achieving your goal. Think of it as a garnish: too much and you'll ruin the dish. 

Text messages go to an individual's cellphone — their most personal device. You want to delight, not annoy. 

Content sent via SMS needs to be well-timed, and highly relevant and valuable to that user, even more so than content sent via other channels.

For starters, use macro conversions for inspiration. Some scenarios where a previous conversion by a customer might be a good opportunity for SMS include:

* They registered for an in-person event
* Appointment reminders 
* They signed up for your SaaS
* Automated surveys (following macro-conversion)
* ETA notifications (e.g. They purchased a high-ticket item and you text to thank them and/or to alert them on the day before and day of delivery.)

What if you don't have a database of qualified mobile numbers? Email your current contacts (<a href="https://neilpatel.com/blog/email-marketing-segmentation-strategies/" target="blank">segment first</a>!) and offer them something of value in exchange for a mobile opt-in. 

> Think of SMS as a garnish: too much and you'll ruin the dish. 

Some brands have successfully created a "VIP messaging club" or "Mobile Insider Club" to generate subscribers via special deals and offers. Consider updating all of your online sign-up forms with an optional mobile number field. Associate an opt-in message with that field. 


## Caution: Regulations Ahead

Regulations surrounding use of SMS are strict. Inform yourself. Adhere to the requirements. 

The <a href="http://www.kleinmoynihan.com/new-tcpa-rules-effective-october-16-2013/" target="blank">Telephone Consumer Protection Act of 2013</a> requires that there be an explicit, written consent in your database for every consumer you send a text message to. Failure to obtain explicit consent can result in fines of up to $1,500 per individual text message. 

You cannot text anyone who has not opted in to receive SMS messages from you. If they opted in for email, you cannot consider this as an opt-in for SMS. You need a distinct SMS opt-in option listed when they sign up for your service or product. 

When a user <em>does</em> opt in to receive SMS from you, it must be for a designated campaign, e.g. a giveaway, an event, etc. When you launch a new campaign, you must obtain a new opt-in. 

Twilio has a convenient <a href="https://www.twilio.com/guidelines/sms" target="blank">online resource</a> listing SMS regulations. You can search by country a view compliance recommendations.


## Adding SMS in Autopilot

I recommend adding SMS via <a href="https://autopilothq.com/" target="blank">Autopilot</a>, a powerful and easy-to-use multi-channel marketing automation platform with drag-and-drop functionality. 

This also offers the benefit of keeping your messaging channels integrated via one platform and your contacts residing in a single marketing database. It supports designing for a seamless cross-channel, cross-device customer journey.

Autopilot offers 4 communication types to create interactive drip campaigns (customer journeys) with: 

* In-app messaging (no log in required) (This is a personalized, unobtrusive pop-up that appears on your website. it's about the size of a live chat feature.)
* Personalized email (The subject can be personalized too.)
* SMS
* On-demand print (postcards)

By "interactive" I mean that you can design your user journeys so that each successive automated message (online or offline) received by a prospect/customer depends on how they interacted with the preceding message. This is smart behavior-based marketing.

 All of these communication types can be personalized, in multiple ways, with fallback variable options included.
 
 ![background](https://res.cloudinary.com/icecloud7/image/upload/f_auto,q_auto,w_auto,e_sharpen/v1563064073/autopilot-canvas_gcmqzi.jpg)

<em>A view of the drag-and-drop canvas you'll use to create multi-channel, interactive drip nurture campaigns.</em>
<hr>


Out of the box, Autopilot comes with a default integration with <a href="https://www.twilio.com/" target="blank">Twilio</a> for SMS. 

You'll get an assigned number from which the texts originate from, and the area code is (415)―San Francisco, where Autopilot's headquarters are. Your SMS messages will be sent from Autopilot's Twilio account. 

This is convenient but the downside is the recipient can't reply to or call the originating number, and you don't have control over the area code. 

Let's go further and set up a custom Twilio integration.

1. Create an account with Twilio.
2. Log in and <a href="https://www.twilio.com/console/phone-numbers/search" target="blank">purchase a number</a>, with an area code of your choice. You can choose whether your number is Voice, Fax, SMS, and/or MMS enabled. (<a href="https://support.twilio.com/hc/en-us/articles/223179348-Porting-a-Phone-Number-to-Twilio" target="blank">Porting over a number</a> you already own is also possible in Twilio.)
 
### Add Your Custom SMS Number to Autopilot
 
To associate your new custom Twilio number with the SMS messages you'll be sending from Autopilot, just log in to Autopilot and go to:

<strong> Settings > App Connections > Twilio > Connect Custom account</strong>

You’ll be prompted to add your Twilio account SID and AuthToken. Don’t know where to find these? Just click on the hyperlink “Where do I find these?” 

![background](https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1563065881/autopilot-accountsid_bec1se.jpg)


That link will take you back to your Twilio account where (logged in) you’ll wind up on the General Settings page you’ll find the two required numbers. 

Once you've connected your custom Twilio account with your Autopilot account, whenever you drag an SMS message block onto your user journey canvas, you'll be able to click the drop-down on it, and select either your custom number or the out-of-the-box 415 number to send SMS messages from.

![background](https://res.cloudinary.com/icecloud7/image/upload/q_auto,f_auto/v1563065991/autopilot-sms_ft6vh8.gif)
 
### Personalization 

All of your communications in Autopilot, including SMS, can be personalized with 23 default personalization variables. Simply click on the Message block (see red "Send SMS" block in image below), then click on the head icon. 

A scrollable drop-down will open with the list of personalization variables. Simply click on the variable of your choice to insert it into the SMS message. 

* Variables use the formulation <mark class="highlight">--Variable Here--</mark>. 
* Fallback variables use the formulation <mark class="highlight">=fallback variable</mark>. 
* Combined: <mark class="highlight">--Variable Here=fallback variable--</mark>. 

![background](https://res.cloudinary.com/icecloud7/image/upload/f_auto/v1563066086/sms-marketing_oewqsk.jpg)

<em>Above image: I've highlighted personalization variables in yellow. The fallback variable is highlighted in green.</em><hr>


### Handling Replies: Send in the Twimlets


Via the Twilio control panel you can connect your SMS number to a staff member's cellphone number, so that any replies to texts that you send out get <a href="https://support.twilio.com/hc/en-us/articles/223134287-Forwarding-SMS-messages-to-another-phone-number" target="blank">forwarded to your cell</a> for speedy reply. 

This is especially helpful for event operations. Say you sent an automated, pre-scheduled text offering help with hotel booking. By having replies sent to the staff member responsible for assisting registrants, they can receive personalized, fast feedback, adding to a positive customer experience. 

Another event example where this is helpful: you can send out an on-location announcement, maybe of a schedule change or surprise guest speaker. Attendees will get the message wherever they are, regardless of whether they have access to a computer. 

You can also program a text message to be delivered when a recipient replies to you. For example: "Thanks for texting the JavaScript Conference Team. We'll get back to you shortly." This is useful if you think you may not be able to respond immediately, but want to give the texter assurance that their message was received. 

You also have multiple options in Twilio re: how to handle inbound voice calls to your SMS number. For example, you can record a greeting and transcribe the caller's voice mail and have it forwarded to your email. 

Get some ideas from <a href="https://www.twilio.com/labs/twimlets" target="blank">browsing Twilio's "twimlets"</a>―micro apps (or widgets) that offer voice functionality. For example, the "Simulring" twimlet will dial 2 or more (5 max) phone numbers simultaneously, and the first person to answer is connected to the caller.


### Integrating With Slack

Want to have all replies forwarded to a Slack channel so the entire team can see them? 

Simply created a dedicated channel in Slack then return to Autopilot Settings:

<mark class="highlight">Settings > App Connections > Slack > Connect to Slack</mark>

You can have any prospect/customer responses―whether to email, in-app messaging, or SMS, spill into a Slack channel. 


## Remarkable Marketing

Done right, with flair and a light touch, SMS can contribute to a remarkable brand experience for your prospects and customers. 

Well-crafted user journeys in Autopilot, across the 4 channels, can yield <A href="https://sherrieg5.myportfolio.com/autopilot" target="blank">mind-blowing engagement rates</a>. Check out the <a href="https://www.getapp.com/marketing-software/a/autopilot/" target="blank">user testimonials</a> on the review platform GetApp.


### Resources on SMS Marketing and Automation

#### <a href="https://learn.g2.com/sms-marketing-statistics" target="blank">30+ Noteworthy SMS Marketing Statistics to Known in 2019</a>

Tricia Dempsey shares some recent stats and shares some interesting info on Metallica's use of SMS marketing.

#### <a href="https://www.thinkwithgoogle.com/advertising-channels/mobile/mobile-marketing-strategy-integrated-experiences/" target="blank">Why You Can No Longer Define Your Strategy By Channels</a>

Consumers expect a consistent and seamless experience across your online + offline channels. Google’s VP of U.S. retail and telecom sales talks about the shifts he's seeing as brands work to deliver truly integrated experiences. Think With Google.


#### <a href="https://autopilothq.com/" target="blank">Autopilot</a>

Map visual user journeys to acquire, nurture, and grow customers. Show new users/web visitors how to get started with your product/service, turn stagnant contacts into repeat buyers, nurture leads, and create successful customers using personalized journeys.

<a href="https://www.thinkwithgoogle.com/marketing-resources/micro-moments/purchase-decision-mobile-growth/" target="blank">I-Want-To-Buy-It Moments: Mobile's Growing Role in a Shopper's Purchase Decision</a>

76% of people who conduct a local search on their smartphone visit a business within 24 hours and 28% of those searches result in a purchase. Source: Think With Google.

#### <a href="https://teamtreehouse.com/library/http-basics" target="blank">HTTP Basics</a>

For those with geeky inclinations: Did you explore the <a href="https://www.twilio.com/labs/twimlets" target="blank">Twilio twimlets</a>? Curious how information is passed via the GET and POST requests in urls? Then check out Team Treehouse's 67-minute course on HTTP Basics. (Also comes in handy if you plan on learning PHP.) 


