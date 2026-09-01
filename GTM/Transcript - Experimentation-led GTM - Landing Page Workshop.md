  
We're going to take half an hour now and go through at breakneck pace how you create a landing page and use it as the base for some of the testing we're doing here. Now, I'm showing you how to do this in high level. You can build in HubSpot, you can build natively in WordPress, you can build a bunch of different places, the same rules are going to apply here, but where you click the buttons is going to be different.

The first thing I'm going to do for people who are solo marketers or entrepreneurs and have to do this themselves for the first time, is show you how to set up a DNS record for the landing page that we're going to build. If you have a tech team who you have do this, skip on to the next bit.

This part is going to be a little boring, so we need to have control over how when someone types in a destination, they're going to go to a landing page that we create. And usually when I'm building a testing setup, I'm going to build on a subdomain of my main domain. So instead of building on, for example, little landing pages.com, which is where I have a bunch of little test websites and pages I would build on some place like for palladium, we might build on palladium dot little landing pages.com.

And the reason I do this is. So as I make pages now off of that subdomain, I can have plenty about the landing page outcome forward slash page one, and then forward slash page two, page three and have a structure that makes sense that I'm iterating through and testing. I'm going to show you how to set that first bit up.

Then we're going to make a page would add some text into it. I'm going to skip the graphic design bits, because I'm kind of a bad graphic designer. And you can always find someone to take care of the graphics and the images for you and go through that. So we'll start we're here in your high level account, and we're going to say, I want to build something new on a site.

We're not going to go to funnel. We're going to go to websites here. We already have an existing I'll take this business courses one. You could make a new website and choose a template and build it from there. But I'm just going to take one of my pre-built kind of working little websites and say, all right, we need to set up the DNS records for this.

So.

I don't have a domain hooked up here yet. So that's where we actually connect our DNS records. We're going to connect a new domain. And I mentioned palladium dot ality. I used com okay. That's going to be our domain. And that's our URL. Now this is not going to automatically set up terribly well in my case I'm going to have to go into Cloudflare to set this up.

So it's going to ask me in Cloudflare to authorize this domain and connect it. I do recommend Cloudflare. If we're building this kind of thing, you can do it manually or as you see here, high level. I have said I could set this up for you if you do it manually. All you have to do is instead of having this automatically go here.

There's the three things you need to look at here. The first is this is going to be a claim record. You can see here on the left that says type of record is name. Then little landing pages. Dot com is already an existing domain for me and Cloudflare for adding palladium dot little landing pages.com. So the name is palladium, and then the content is what is actually going to go over on the servers I'm setting up.

So this record sets up, I authorize it. That one click is pretty easy. It's going to take a few seconds for Cloudflare to authorize. If you're using and older service like GoDaddy, it might take up to 24 hours. So if you got to wait that long, I don't know, pause the video, go write a really compelling email, get a nap and come back.

Then we're going to link the domain we set up with the website. In this case we have the Business Courses site and there's our home page. That's all we have to do to get this thing set up are the DNS records and services side. I want to show you how to build the actual page. If you skipped ahead.

Welcome back. Now we're building something and we're going to go out of the settings part and into the page we've now put together here. And we're going to we could add a new page. We could add an existing one. We'll start with add a new page. So this is palladium coaching and coaching websites. We tend to show the coach who is the star of the show.

So we're going to call this what's our coach's name. I don't know. Sarah. Sarah. Landing page. And the path is going to be slash I spy and then my SRH slash Sarah create new page. Cool. It's going to ask how do you want to make this page. And we can use an existing page which will be able to use one of the pages we already built for our website or create from blank.

We'll going pretty fast here. So the when to use an existing page from the business courses would use the About Us page. But of course you can build from scratch. You have many, many, many other templates in high level you can work from. There's a lot of ways to go about this, but since we're not a web development course here, let's instead dive into how we take the content we want to create and put it in this page.

So now we're in the page that we made for Sarah as the coach at Palladium Coaching the content here pretty much all lorem ipsum for now. And we got to fix that. Here's Sarah's picture. She's looking great. How do we go from here? I've got another prompt at this prompt will be in the resources at the bottom here.

Grab it when you want for how we're going to build out a landing page. There's a couple pieces a good landing page should have should have a headline that's pretty compelling, that focuses again on your customer problem, not on what you do. It should have some social proof. It should have how what you're doing works. It should have some explainers.

And of course it should have a call to action. So our audience overview, we already know from the previous, chat that we ran where we went, who was our audience is business coaches who were earning more than ten K a month, but less than 70 5KA month. And for social proof, we still have the coaching social proof examples that I made earlier.

So now there's our content for this template. Continue. We're going to use again 3.5 to make this and get this into. It's going to generate a whole landing page for us. And there's going to be bits we're going to use verbatim. And there may will be some bits we tweak of it. But as you can see this just came together with the beginnings of a landing page as better questions make more money isn't a terrible lead, but if you remember in Figma, we ran several different variations of a minimum viable sprint, and it may well be that one of these really worked well it past that winning audience that in which case you probably want

to use the headline for that because you already know it gets people's attention. So we will say in this case, for the purposes of our demonstration, stop creating time for money scale. Your coaching practice was the best headline we have. That's too many words for a headline, but stop trading time for money is pretty good. There is our headline and our subheadline.

It's going to be scale your coaching practice with Palladium coaching. I don't think I need this headline here. So good in that now there are varying opinions on whether to leave your title navigation in place for our landing page. If we're running a minimum viable sprint, this would go to your home page. So you do need title navigation of that.

00;08;20;08 \- 00;08;43;00  
Unbekannt  
But for a specific landing page, you could either have the opinion that you don't want to have title. Now, there could be good people reason to click away and maybe not perform your conversion action and more importantly, not be trackable for having performed your conversion action. But the other school of thought is well, but if they don't want to take the conversion right now, they can find out more about me and then maybe convert later.

Which is right. I don't know. But you know what? I do know? You should test it. Fortunately, we're talking about how to go to landing pages and change them. So this is how you find that out. So okay, stop creating time for money. Scale your coaching practice with Palladium coaching. But we're missing one big thing. I've got this page open.

What do I do here? It would be nice if we added in a button. So we're going to add in button. Which I'll be honest, that green looks pretty bad with all the other colors we've got. That feels a little better. We can change the, call to action now. There are many advanced features I could add here with, you know, changing animation, that advanced stuff.

But we're just going to make this book a chat with Sarah. Cool. And then we would have this go to some destination, might, well, a destination be probably a calendar booking page, something like that. Whatever you want to be, that's your call to action. But we now have a button set up where someone click on it and go somewhere cool.

The next thing we generally see in a landing page set up is going to be some social proof. But what top coaches say okay, I would rephrase that into probably something a little more like what our coaches say.

But now that text is impossible to read, so let's fix that. So the white headline, hey, there we go.

What our coaches say. And this goes up, and then we're going to grab the actual quote.

Oh, we have here's our quote. And here's I believe this person's name was be.

Lovington. And it was for the coaches the CEOs. That these. There we go. There's our quote from our hero. And we may want to add in, a picture. So I'm going to go to this person does not exist.com and grab someone's rendered face. That's probably not a bob. Nor is that eventually we'll get to a Bob.

I may have the filter set to only show, there's a bomb. Okay, so we are.

Saving this image to use as a portrait. There we go. And we will put this in. Oh, I don't know. It says logo here. Let's put bombs face instead.

Hey, there we go. Okay, so now we've got Bob's frankly kind of aggressive looking image here, but whatever. And we will use this as.

Our, source. So we'll replace that with this. That's a bit large. So we will edit the image size down to we'll say.

There we are. And we could apply some design to move it around or make it a circle or other options here, but I'm just showing you how we can make a little bit of social proof go on here. All right. Now we have another picture of our charismatic Sarah. I'm not going to discuss what we're going to have her do now.

So book your strategy session. It's going to be our next section here. We'll add in a.

Headline. That's this.  
And we can add in.

Bullet points laying out the features we've got. We're going to talk about how it works. So what would you actually get out of using this.

And. Make this a, bulleted list instead of a random block of text. I was I ordered list.

And put. This is for.

And then what are the stuff we don't really need except to grab this out? Make another call to action, and we could add a pricing table at the bottom here. Right. The rest of this we're going to remove for now. This is kind of a minimum page.

And we can remove entire sections.  
Social proof. Stripe. Footer. And we could do, you. Pricings that. If you're right, we have core program.

Premium packaging, VIP experience.  
Okay.

Here's the basic elements of building a landing page here. And I click publish. That is SEO and set up you're going to want to do. But you can see, having set up our DNS records, having I set this up to publish, now we have the basics of a landing page here. Like we've got a button, we've got some headlines, we've got some pictures.

There's a lot we can do to make this page better, aside from the design deficiencies of it. And I think that's worth talking about as you send the traffic to a landing page, what are the pieces you have to change to make the performance improve? We'll talk about that in a few moments.  
