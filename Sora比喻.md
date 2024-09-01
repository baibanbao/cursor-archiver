---
tags:
  - sora
---
# Sora比喻



[How Sora Works (And What It Means)](https://every.to/chain-of-thought/sora-and-the-future-of-filmmaking)



# How Sora Works (And What It Means)

OpenAI's new text-to-video model heralds a new form of filmmaking

BY [DAN SHIPPER](https://every.to/@danshipper)

FEBRUARY 16, 2024

[50](https://every.to/sora-and-the-future-of-filmmaking/sora-and-the-future-of-filmmaking/feedback?rating=amazing)

**Listen**

![Pasted 2024-02-17-13-36-18.png](./Sora比喻-assets/Pasted%202024-02-17-13-36-18.png)

DALL-E/Every illustration.

Look, here’s what we’re *not* going to do. We’re not going to freak out. We’re not going to prognosticate about utopia or predict doom. We’re going to keep our heads on straight and…

DID YOU FREAKING SEE SORA????

OpenAI’s new text-to-video model can generate a 60-second photorealistic video of a pair of adorable [golden retrievers podcasting on a mountain top](https://twitter.com/sama/status/1758218820542763012). It can generate a video of [Bling Zoo](https://twitter.com/billpeeb/status/1758223674832728242), where a tiger lazes in an enclosure littered with emeralds and a capuchin monkey wears a king’s crown behind a gilded cage. It can generate a video of an [AI Italian grandmother](https://twitter.com/sama/status/1758219575882301608) wearing a pink floral apron and making gnocchi in a rustic kitchen. (Her hands look a little like the hot dog fingers from *Everything Everywhere All at Once,* but still—that’s a movie, too!) 

It’s wild. It’s incredible. It caused Mr. Beast [to tweet at Sam Altman](https://twitter.com/MrBeast/status/1758194696034365674): “Please don’t make me homeless.”

There’s a line from a Chekhov story that reads, “I understood it as I understand lightning.” He might as well have been talking about Sora. The demos struck me bodily, like electricity. 

*Phew*. I’m glad I got that out of my system. It was important to say that because writing about a buzzy new drop from OpenAI is a little bit like sailing between a [Scylla and Charybdis](https://en.wikipedia.org/wiki/Between_Scylla_and_Charybdis) of the mind:



![Pasted 2024-02-17-13-36-18.jpeg](./Sora比喻-assets/Pasted%202024-02-17-13-36-18.jpeg)

*Meme format inspired by [Visakan Veerasamy](https://twitter.com/visakanv).*



In one part of my brain are the multi-headed dragons of doom telling me to strafe the freaking data centers before the movie industry combusts like Mel Gibson’s career. In another part is the techno-optimistic quantum whirlpool of excitement already planning the Pixar-style movie I will create as soon as I get my hands on this model. The world will finally see me as the undiscovered heir to George Lucas that I secretly always knew that I was—lack of ever having made a film be damned.

The problem is, I know both parts of my brain are wrong. *Ayyy lmao*. 

My brain is mistaking *newness* for something that it’s not. The feeling I’m getting from watching these demos is not the one I get from watching a great movie, YouTube video, or TikTok. Why? I know, in time, the newness of these demos will fade, and they’ll become normal—mundane, even. I’ll no longer get excited by them. But a well-crafted movie will continue to be compelling.

The best way to keep a level head about advances like these is to think of them in terms of long-term trends. Sora in particular, and AI filmmaking in general, is an extension of two important ones:

1. Tremendous amounts of data and compute being used to generate mind-blowing AI breakthroughs

2. Technology driving down the cost of filmmaking 

Let’s talk about both of them.

## **How Sora uses massive amounts of data to make mind-blowing video clips**

AI runs on scale: More data and more compute means better results. Sora is impressive because OpenAI figured out how to throw more data and more compute at text-to-video than anyone else has before. Here’s a simplified version of how the company did it based on what I can glean from [its whitepaper](https://openai.com/research/video-generation-models-as-world-simulators). 

Imagine a film print of *The Dark Knight*. You know what I’m talking about: the reel of cellophane wound around a metal disk that a young man in a red blazer hooks up to a projector in an old-style movie theater.

You unroll the film from its scroll and chop off the first 100 frames of cellophane. You take each frame—here the Joker laughing maniacally, there the Batman grimacing —and perform the following strange ritual: 

You use an X-acto knife to cut a gash in the shape of an amoeba in the first frame. You excise this cellophane amoeba with tweezers as carefully as a watchmaker and put it in a safe place. Then you move on to the next frame: You cut the same amoeba-shaped hole from the same part of the next cellophane frame. You remove this new amoeba—shaped precisely the same as the last one—with tweezers and stack it carefully on top of the first one. You keep going, until you’ve done this to all 100 frames. 

You now have a multicolored amoeba extruded along its Y-axis. A tower of cellophane that could be run through a projector to show a small area of *The Dark Knight*, as if someone stuck their hand in a loose fist in front of the projector, letting only a little bit of the movie through.

This tower is then compressed and turn into what’s called a “patch”—a smear of color changing through time. The patch is the basic unit of Sora in the same way the “token” is the basic unit of GPT-4. Tokens are bits of words, while patches are bits of movies. 

GPT-4 has been trained to take in a sequence of tokens and output the next token in the sequence. Sora has been trained to do the same thing: It takes in a sequence of patches and outputs the next “patch” in the sequence. 

Patches are innovative—and Sora appears to be so powerful—because they allowed OpenAI to train Sora on an immense amount of image and video data. Imagine patches cut out of every video in existence—infinite towers of cellophane—stacked and fed into the model.

Previous text-to-video approaches required images and videos used in training to all be the same size, which required significant pre-processing to cut videos down to size. But because Sora trains on “patches” instead of the full frame of the video, it can gobble up any video or image without requiring it to be cut down. 

As a result, more data can be used for training, for a higher quality output. For example, pre-processing videos into new aspect ratios often means that they’re cut in such a way that the original framing of the video is lost. A video showing a person at the center of the frame in widescreen, when cropped, might show that human only partially in view. Because Sora can take any video as training input, its output doesn’t suffer from the effects of poorly framed training input.

Another big advance with Sora is the architecture it uses. Traditionally, text-to-video models like [Runway](https://runwayml.com/) are diffusion models, while text models like GPT-4 are transformers. Sora is a diffusion transformer: a mashup of the two. Instead of predicting the next piece of text in a sequence, Sora predicts the next “patch” in a sequence of patches. By using this architecture, OpenAI can throw much more data and compute at training Sora, and the results are stunning.

When Sora videos first dropped, [people were amazed](https://twitter.com/drjimfan/status/1758210245799920123?s=46) that it could simulate things like the fluid dynamics of coffee splashing around in a coffee cup. They assumed that OpenAI had connected Sora to a game engine (the algorithms that power video games and can simulate physics) in order to generate results like that. But that’s not what happened. Sora can create graphics like that on its own.

GPT-4 seems to learn the rules of grammar in order to predict the next word in a sequence. 

Diffusion transformer models like Sora seem to learn physics—the grammar of the universe—in order to predict the next segment of video. OpenAI sees Sora as the first step in a “world simulator” that can model any slice of reality with a text prompt.

It’s mind-blowing. And it will have important implications for filmmaking.

## **How technology has shaped filmmaking**

What will be different in a world where videos like this are normal? Probably everything about how videos are made—and that’s a good thing. 

Movie-making has historically been insanely expensive. Cameras, lights, emotionally unstable actors—these things all cost *moolah*. That’s why the movie industry is an industry instead of an artist’s colony.

For most of the history of movies, only a few people got to make them. They were risky! You needed money to make them. And only certain people were able to get enough money to take the risk of making an expensive flop. Making movies was akin to starting a company.

Over the past two decades, that started to change. The internet and the iPhone, for example, are step-changes that put movie-making and distribution equipment into millions more hands than was possible before. It spawned an entirely new form of filmmaking: YouTube videos, TikToks, Reels, and Quibbis. (Okay, maybe not Quibbis.) 

This generation’s genre of filmmaking has its own style, distinct from Hollywood, that is constrained and shaped by the technology and resources available to make it. YouTubers, for example, are known for direct-to-camera monologues, quick cuts, and vlogs showing the day-to-day minutiae of life—the kind of videos you can make alone in your room with an iPhone.

AI video makes it even easier to make many more kinds of videos alone in your room. Runway, which is already publicly available, allows you to turn an image—whether real or AI-generated—into a four-second video clip. You can make different elements of the image move in different ways and control the motion of the camera. It’s as if you have the ability to make your images move like the wizard photos in *Harry Potter*.

These tools, too, have spawned a new style of filmmaking constrained and shaped by their unique powers and limitations. For example, they make it easy to create AI videos that use familiar characters in new settings and styles. A common trope is to take two shared pieces of pop culture and mash them up, like in a clip that renders *[Star Wars](https://www.youtube.com/watch?v=d-8DT5Q8kzI)*[ characters in the style of Wes Anderson](https://www.youtube.com/watch?v=d-8DT5Q8kzI). 

Another example: The architecture of today’s video models like Runway make it tricky to consistently generate the same character in different clips. You can get them to look similar—there’s a family resemblance—but the controls are not fine-grained enough to make the characters look exactly alike.  So AI films tend to be more like visual montages: clips of a few seconds with quick cuts and a narrator monologuing a story, rather than one where a consistent set of actors do dialogue in front of a camera.

Sora is a step-change in the capabilities of these tools, making it possible for AI filmmakers to do more with less. Clips can be 60 seconds long, which will enable a greater variety of editing styles. The motion and physics simulation that Sora can perform is *far* better than any publicly available model. This will allow for more complex scenes, character movements, and interactions between characters and the world around them than is currently possible. 

What effect will this have on filmmaking?

## **AI filmmaking today**

Sometimes it feels like the universe has your back, like hitting a straight on the river card when you’re holding a two-three off-suit. As it happens, I know a little bit about AI filmmaking because I interviewed someone at the forefront of it for [my podcas](https://www.youtube.com/@everyinc)t this week, two days before Sora launched. That interview will be live in two weeks, but I want to tell you a bit about what I learned.

[Dave Clark](https://twitter.com/Diesol) is a traditional filmmaker who has started to make AI-generated videos. He recently produced a sci-fi short called *[Borrowing Time](https://twitter.com/Diesol/status/1747351624329355474)* that was inspired by his father’s experiences as a Black man in the 1960s. He produced it entirely using Midjourney and Runway to generate images and videos. He narrated the movie himself and used [Eleven Labs](https://elevenlabs.io/) to turn his voice acting into the voices of different characters. 

*Borrowing Time* went viral, and Dave told me he wouldn’t have been able to make it without AI. It would’ve been impossible to get a sci-fi short like his funded by a traditional Hollywood studio. But now that it’s out, and popular, he says that he’s fielding interest from top-tier Hollywood studios who would like to make it into a full-length movie. 

This anecdote speaks volumes about the way that AI models like Sora will change filmmaking in the future.

#### **Movie concepts will be cheap to test**

If you want to make a sci-fi movie in a world with Sora, all you need is a laptop and some OpenAI credits. More people will be able to make videos reflecting their imagination without needing to go through traditional gatekeepers for approval or get funding. And it won’t be just podcasting or monologuing YouTubers who get this opportunity; it will be anyone.

Video producers whose ideas get traction will be more likely to get funded to make them into movies—much like the way writers today use tweets and newsletters to land book deals. 

#### **Big-budget movies will cost less to make**

In a vacuum, AI tools will make traditional Hollywood movies cost less to produce. *Everything Everywhere All at Once*, which used Runway for its special effects, was able to portray mind-bending feats (like hot dog hands!) with a [team of just eight people](https://variety.com/2023/artisans/news/artificial-intelligence-runway-everything-everywhere-all-at-once-1235532322/). For context, about 300 people worked on *Shrek*.

Theoretically, Sora *should* make productions like *EEAAO* more common. But pre-existing business structures and union agreements might make it difficult for Hollywood to take maximum advantage of these tools. Instead, a new form of filmmaking will flower somewhere else.

#### **AI filmmaking will become its own form, and Hollywood will become less relevant**

In the same way that the iPhone and the internet led to the flourishing of vlogs and makeup tutorials, AI filmmaking will create its own genre of film, with its own style and form. I’d expect the kinds of videos we’ve already seen to proliferate: The use of existing IP to make mashups and clips with quicker cuts and voiceover monologue should be staples of the genre until the technology changes again. (As far as we can tell, actors in videos generated by Sora can’t deliver facial movements that map to a specific line of dialogue.)

These AI videos won’t replace traditional Hollywood movie-making—just like YouTube videos haven’t—but they’ll likely eat into mind- and market-share, especially among young people. 

## **The future of creativity**

Earlier in this article we talked about the long-term trends that Sora is extending:

1. More data and more compute generating more impressive AI results

2. Technology driving down the cost of filmmaking, thereby changing what kinds of movies get made and by whom

Hopefully that has put some of Sora’s capabilities into a broader perspective. But there’s one more important trend that I want to end with. 

I’ve been writing for the last couple months about our transition from a knowledge economy to [an allocation economy](https://every.to/chain-of-thought/the-knowledge-economy-is-over-welcome-to-the-allocation-economy): We’re moving from a world where you’re compensated based on what you know to one where you’re compensated for how well you can allocate intelligence. In this world, even individual contributors or solopreneurs become managers—but instead of managing humans, we manage models.

It’s clear that Sora fits into this paradigm: The better you know how to manage it as a tool to create incredible things, the better you’ll be positioned in the new economy. But the most exciting part is that it broadens the sphere of people who are allowed to make things in the world.

Just like GPT-4 made it possible for anyone to ship a web app with enough persistence, Sora makes it possible for anyone to make a video. And when I say anyone, that includes you.

Sora doesn’t allow anyone to make a great video at the touch of a button. Storytelling will require much more skill, taste, and dedication than that. But anyone can get started, learn those skills, and have a shot to be great—all they need is a laptop.

If you are a creative person, this is without a doubt the best time to be alive.



---



*Editor's note:* The explanation of Sora is deliberately simplified. The pixels of video that make up a "patch" are compressed into a smaller latent space before being used. For full details, read the [white paper](https://openai.com/research/video-generation-models-as-world-simulators) (also linked to in the article).