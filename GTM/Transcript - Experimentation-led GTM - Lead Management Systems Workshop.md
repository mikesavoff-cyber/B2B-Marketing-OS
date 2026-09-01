  
All right. So we're getting leads into the system. And we need to find some way to take them and begin to qualify them further, but also engage them quickly so we can start conversations. There are a number of tools that you can use to start to tackle this problem. I'm going to show you one called thali, which works on both SMS and phone calls to qualify things.

And we're going to build a little script for Sarah at Palladium and show you how this works. And think about the pieces we want to put into qualification at a automated scale. There are other tools you can use that do similar things. You can build directly out of 11 labs with the API and use just the straight AI there, or find a different front end you like.

The end result is going to tend to be the same regardless. So what we need to answer as we tackle lead qualification comes down to if I were to have whether it's an SDR or you, the founder or head of the marketing team, we're able to talk to every single person who was interested in my business. What are the 2 or 3 questions I could ask that would really help me understand if I can help them?

Now, it's important you're making these questions deliberately or something that eliminates bad fits, because we're setting this AI up as a giant filter to go from people who have signed up, are very low intent, and don't seem super engaged to folks who've talked to someone who says, we can help you with your problem, and the problem is narrowly enough to find that.

There you go. Yes, I want your help making this happen. So let's imagine for Sarah here at Palladium Coaching that she needs to know a few things about who her coaches are to understand they're really a good fit for her. One of the questions we were discussing, adding in that Facebook form was, what's your monthly revenue? So supposing we're only working with people who we know are more than ten K a month?

We don't need to ask again, what's your monthly revenue? Because we filtered them out earlier. But it might be worth asking how many clients do you have for them? Maybe you have 110 k a month client as a coach, that would be pretty wild, but if you have a corporate account or something, you might have 5 or 10 exactly who you're helping through that one client.

That's obviously a very risky business. And scaling that up would be challenging because this person isn't used to dealing with multiple clients. So if we asked how many customers do you have, that might be a good one to ask. We also need to figure out if we're going to help this coach scale. Are they ready for it? A common problem, particularly for a small business owner, is if you were to two x or five x their business, it actually wouldn't succeed because the processes they have that work for one or 2 or 3 clients aren't the ones that work for 20\.

So we need to find a way to qualify the people who will succeed. When Sarah gives them the tools they need to make a larger volume business, and not the folks who will end up grinding to a halt. The business fails, and Sarah doesn't have good case studies to discuss as she scales her business. So number of clients you've currently got and we need to ask a process question we need to figure out, we might ask, do you have documented our SOPs for onboarding SOPs and standard operating procedures?

Can we assume that if you've got some documented SOPs, you could say, I need to add a VA or a junior employee in my company? You can tackle some of this so we can add more volume into things. And then if we know that you've actually got a couple clients and you've got some resilience, see there and you're ready to deal with some scale, the last thing we want to figure out is why do you think you aren't scaling?

Yeah, this is a really common sales question. And I know this is a marketing course, not a sales one, but a really common sales question is what is your limiter? Because then I want to be able to say, oh, well we do that. We help you unblock from this limiter. Now the first thing we're going to do is figure out if this person is willing to talk, because I don't know about you, but sometimes I find myself scrolling Facebook one of the morning, and if I filled out a form and you called me right, then I'd be pretty mad.

So we're going to start this year. We're going to have a trigger, and the trigger will be, we'll pick from high level, we'll pick from miss account, and a new contact is created. This is if we're synchronizing from Facebook into high level. As soon as someone filled out the form within like 2 to 5 minutes, there'll be a new contact created so we can say, great, now we have contact creation, we're going to start the conversation.

And this is currently set up for speaking, but I'm not convinced. We want to begin with a call. I think we want to set up some kind of, outbound setup that will begin a conversation over text. What we need to do is send the SMS to our lead that says, hey, is now a good time to chat?

We're going to set up in high level automated message. This will be our for lady. Qualification flow. And after the lead form is submitted, we send them an SMS. And if they say yes, then they end up here and we call. So the called outbound. And we'll start with hey first name. We get that from the on the client field.

Thanks for your interest. Can I ask you a few questions and I'll get a call here. Right. We can get a yes or we can get a no. And you can actually see paths out from here. Now, I'll be honest, at this point, getting a no is pretty weird, given we already got the yes. Let's go ahead and build some resilience at the end of this, because I will just start out if you don't have something right there.

So okay, we're going to say, hey, let me ask you a few questions. And the first question we discussed that we need to ask is, how many clients does your coaching. Business. Have. Now, this outcome is guiding the I know there's definitely some room for some weirdness here, because the AI is attempting to figure out if the answer is what you said.

But if we say fewer than I know for clients and we say more. More than three clients is our two logic. So. Right. So how many clients do you have? I have three, I have two, I have one I, I take you one route. If I have more than that, I'll take you another. And I can just build out from here and say, hey, we're going to add a new node and we will do fewer and add a new node, and we will do more.

And out of this now I can say so if you have fewer than three, three clients or fewer, I can say, oh, I'm sorry. No, sorry, but oh, I think Sarah, and the. Fully the, coaching team are best suited to helping. To work with multiple.

Clients and are ready to scale. Can I check in with you? In. I will say two months. Two months and see if we can help you. Then.

Now, this is important because if you get leads into your system who are not a good fit right now, that doesn't mean they're never a good fit. And setting up some permission, but also automated system where every month, two months, maybe a week, two weeks, depending on what's appropriate for your lead. Based who's going to give you a reason to go back to these leads you've already paid to get, and maybe see if they're a good fit.

Now, in general, if we're asking some of the right questions, but we're doing the lead gen qualification on platform or the lead qualification on your landing page, the people who are signing up may not be ready right now, but they certainly could be ready in some point in the future. The general stat, they say, is something like 90% of buyers aren't ready to buy right now.

So a whole bunch of the leads you are gathering aren't going to be buying right now, but they will definitely be ready to buy at some point in the future. If you hit them when they're ready to buy, you might be able to get that lead for free having already paid and just qualified it earlier. So the outcomes here might be sure we can talk later.

Or. No thanks. If there are no thanks, will basically say, hey, we are, sorry. Oh, thanks. We can add them to a do not disturb list. We got your information. You'd want to be contacted again. Goodbye. Then we would set a reminder out. I can add a new node for an action, and we can set a API call back over to high level.

Set a reminder on that client's record that says, hey, reach out to this person again in two months time. I'll show you how to do that just a second. But before we do that, we are also going to build the no thanks. I don't want to be heard again. Create a, new speech action which will be. Thanks for contacting us.

We'll be sure not to bother you again. And then we can add the only outcome is, another action. So we would drag this to here. We make a new action.

And basically. And the call that's not in the call, we would. Make an end node call was done and wrap this up. Now that's one complete path from start to finish. Right. Somebody fills out a form. We think they're interested. We text them, they say let's talk. We call and say, would you like to talk? And they go, actually, no, never mind.

My bad. I don't want to hear from you again. We're done as the shortest possible path through this tree, but it definitely not the path you want to see your leads take. Now, I'm not going to make you watch me narrate every single step through this, but I'm going to add a few more pieces to this. When we come back, I want to show you what this is like when somebody actually gets to call what we've done off camera.

Now, if we put together a workflow, what you can see is, I'd say modestly complex, but not insanely so. The goal here is to go through the three questions we've just discussed. Like, do you have a business that has a couple of clients? So you've got some processes that mean you were ready to scale? Do you have a SOPs in place so that if you saw more volume coming in, you'd be ready to tackle it?

And then finally, why do you think it is? You're not growing right now. The AI is going to ask all these questions. And as it asks them, we're going to see how it handles the qualification. And then it will be routed different places based off of what we say.

Hi there. Thanks for your interest. Can I ask you a few questions? Sure. Great. Let me ask you a few questions. How many clients does your coaching course have? We have seven clients right now. Oh. That's great. Seven clients means you're on the right track. Do you have a sop's you can use to help you onboard new customers and scale up your business with new clients?

No. We don't have any SOPs. Why? Oh, I get it. Not having your SOPs can make it tough to onboard new clients smoothly. It can be frustrating if you're not growing and you don't know why. Can I get you on a call with Sarah to see if she can help you identify your problem with a free 30 minute consult?

Well, sure. Yeah. Okay, great. I'll set that up for you. When would be a good time for Sarah to reach out for that consult? Can I do Thursday afternoon? Thursday afternoon works. Well, I'll make sure Sarah reaches out then. Looking forward to it. Is there anything else you'd like to discuss before we wrap up? No thank you.

I think I'm okay. Thanks for your time today. I'll have Sarah reach out on Thursday afternoon. Have a great day. So a couple things have happened here in the background. One of these is you can see down in the kind of final action where these calls are going, we have a Calendly integration. What's going to happen right now is this will look at Sarah's calendar and the timezone where this person connected from and find it opening it automatically send the booking and automatically sent booking will have all the information attached for the call to actually happen.

Now I could do another call where I instantly just qualify myself and we'll see what happens. Instead, you'll see that the, end is going to be quite different.

Hi there. Thanks for your interest. Can I ask you a few questions? No. That's fine. When would be a good time for me to reach out again? I don't want to hear from you again. Who are you? Thanks for calling. Have a great day. And there we go. So that's the lead. Who? Immediately. Which happens. Sometimes they fill out a form and you text them.

You say, can I call? They say yes and you call. They're like, no. Who are you? You spammer? Go away forever, right? Anywhere you do this, you can see this is effectively the same as having an SDR. I chose the Scottish voice pack for this one. I don't know why it's amused me to write. In any case, these are 11 labs voices.

They have like 200 of them. They can also do many languages. So what you get out of this is, I mean, choose a voice pack you want. I see this is Daisy, the young Scottish female. You choose whatever voice pack you want, choose the workflow you want to work through. And of course, in the messages, the Scottish accent won't come through and you are able to qualify somebody any hour of the day or night and begin to build lead in Richmond.

I would note if you say, I don't want to talk to you now, but instead you come back and you say, maybe touch base with me later. What you get here is an API call where we are basically posting to an end point in our CRM, and that's going to vary by, whatever your CRM is an API call to put a reminder on a task, basically on a contact record that 60 days from today they're going to be reached out to again.

So you can see how very quickly we're able to assemble workflows where as leads come in, we begin to qualify them. And the ones that are good fit get passed off to a human. And the ones that aren't a good fit get put aside to come back to again later. Doing this. Whether this lead came from your website, it came from LinkedIn or Facebook or whatever, we could create the triggers that work at the beginning of this for basically any instance you want, particularly because I can set here a trigger for, you know, when a contact is updated in some way and high level, then do a new thing over here.

This kind of workflow automation across several tools is what's going to make you be able to punch above your weight. As a marketer, working at a small team, or as a solo entrepreneur building your own thing. Something else we can do as we're building a system to take leads from a website or wherever and begin to understand more about them and work them at scale, is in basically any CRM you work with, you're going to have the capacity to start to do lead scoring.

Now, we kind of did a very rough version of lead scoring with the AI, SMS and calling, lead filtering we showed because basically our lead score was purely pass or fail. Either you've answered all the questions correctly and we want to talk to you or you don't, and we don't. But as you begin to build more complex workflows and begin to scale up what you're doing, there's going to be this area in between a good lead and a badly that says we should do something with you, other than just kind of automatically send stuff your way every week with our newsletter.

But we're not ready to have a human try and talk to you. Just yet. Lead scoring lets you begin to figure out what all those pieces look like. And as you have, whether it's sales agents or AI, sales agents, begin to give you something that indicates people are tipping over when you already have their contact info, but you haven't really talked to them yet.

Some examples of ways to build lead scoring include looking at what's happening on your site, and how often this prospect has come back to your website. If they're showing up several times and reading some of your content on your website frequently, this is a highly engaged person, even if they've never talked to you, and you're able to say based off of maybe the pages they've been to, if they're a particular interest of theirs, if your content has tagging or, topics applied to it, you can say, oh, this person looked at all of my life coaching, of course, information, and you can go, okay, let me reach out to you about, hey, it seems you're

interested in being a better life coach. Could you have a chat with Sarah and see how we can help you learn to improve your life? Coaching, outreach programs? Whatever it is, we have a hook in there. We can see based off of what you are doing, leads going on within a change per company, even sometimes per campaign. So the basics of how to set up lead scoring are going to largely be in the beginning based off of what you think is going to work.

But it's going to be hard to say for sure if you've got all the right lead scoring mechanisms in place and if you put the right weight on the right things. If you do set up triggers for an AI call based off of hitting a few different elements of your lead scoring, you start to get better information out.

Because the AI call is so consistent, it's always doing the same thing. Unlike a human who maybe one day they're a little higher energy and the other day they're a little lower energy and not quite feeling it. And so you get different results out based off of just how good the salesperson is that week. With an AI, the consistency of what you're delivering gives you a fixed point of data to say, hey, we thought this was the lead score, and if you visit the website this many times, we're going to do this action now and reach out to you.

But the conversion rate through for this set of lead scores is worse than this one. So we need to alter things. You have harder data on what's working and what's not. There are a few caveats here. As you're building your lead scoring and as you're building your automations, it is really easy when you build automations that are multi-touch, right?

I've got an email, I've got an SMS that maybe I've got a call set up and I've got onboarding. Oh no, there's another call set up for onboarding. And then, oh, someone at the end of their trial, I want to I want to make sure we send them the smells that, hey, you're transiting in two days. And if you got into this workflow and then you didn't finish it, we think maybe you have a problem.

We'll set up an email or two to help you get out of it. And quickly, before you realize it, you're sending someone seven messages, two emails, and two phone calls in one day. Stop. Well, you were building particularly multi-touch workflows. You have to really look at the high level. What are all of the pieces you are sending? And make sure that you don't have overlapping multiple touch instances.

One of the good ways to do that any CRM is going to have a conversation view. Now, this is a, a template kind of set up environment. So we're not going to have a lot of conversations going on here. But you'll see, for example, SMS, WhatsApp and email conversations in high level or in HubSpot. And you'll be able to see the volume of what's being sent as you're building multi-stage workflows throughout many different parts of the buyer journey.

Do take some time. Every week, pick 3 to 5 random contacts and just see what their message flow has looked like. You might be just surprised to discover you're touching people two, three, five times a day when you didn't really mean to because edge cases start to crop up. The other part is, I know some people see, wow, I can set up AI qualification that's really low cost to have somebody talk to somebody.

Maybe I should do this outbound. I can just robo dial people right? No, that's against the law in most parts of the world. And if you do this and you get caught, you'll pay a pretty high. Fine. I find this tool is really, really powerful to take people who have come to you and begin to understand more about them in a way that wasn't possible even two years ago.

If you do set these tools up and don't pay attention to them or set them up and don't use them the right way, you're going to get yourself in trouble. And that's not what we want to do at the high level. The pieces you want to pay attention to as you are building out your campaigns and automating them, is we have our three things.

We have our four numbers. And those four numbers we're looking at are going to be our North Star. We want to understand, are we at that 1% crossing the interest gap, the 5% on sign up. And now here we are nurturing our 20% of people who begin a discussion with our AI through SMS or through Facebook chat or through call are they indicate they want to talk to a human?

Are they indicate they want to go to the next step? If they are indicating that, they are saying, yeah, you know what, I'm ready to go. Then we're in a good place to say this part of the engine is nurturing people, moving on. The individual will sub pieces of data in here, right? How long is the call? What number of people go from stage one to stage three?

When you're first building this out, it's really easy to get lost in all the little tiny bits of data and really geek out about what you've got to see here and how do I optimize things. But a big part of this iteration process we're going through with go to market engines and minimum Viable, some of these Legion campaigns, and we want to go for big swings.

First. We want to make big changes first. If you find yourself adjusting step two or step three of ten different campaigns and you're really not yet at that 20% activation and 4,050% close rate, you're focusing on the wrong thing. And we want to optimize is what's the smallest change we can make earliest in the system to have the biggest outcome later on we get leads and interested prospects in.

So although you've got with tools like high level and tools like me and up lead and all these other ways to outreach and connect to people, you've got a lot of numbers you can pay attention to. I really recommend a dashboard like this. Set it up and you want to focus on what's my people crossing the interest gap, the attention gap, the consideration gap, and finally the decision gap.

If you pay attention to those numbers and don't get distracted by everything else you could look at, you want to focus on what moves the needle for your business. You want to end up growing faster when you build these lead qualification systems that you're bringing all this information into your business, you're going to quickly discover that you're starting to reach the maximum of what you can accomplish on meta ads or LinkedIn ads, and you're starting to find that spending more money doesn't make more results.

That's when you're ready to take the next step in building and scaling your marketing efforts, and go from just inbound marketing gear to something that's a bit bigger, contains more elements of it. I like to call that all about marketing. Let's talk about that next.  
