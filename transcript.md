# Introduction to voice Technology

## Introduction and welcome

Thanks everyone for your time and for coming tonight, I know many of you have competing demands on your time. I'm Kathy Reid, Director of Developer Relations for Mycroft AI, an open source voice recognition startup based in States, and I'm also President of Linux Australia, the voice of Australia's open source community. I work at the intersection of technical communities, emerging technology, helping to bring structure, frameworks and order to the chaos that can be emerging tech.

### Partners
I'd like to give my sincere thanks too to Creative Geelong, and Jennifer Cromarty for hosting ushere at the Creative Geelong Makers Hub. This event is also part of the Victorian Digital Innovation Festival, which you can follow on social media with the handles on screen there.

### Acknowledgement of Country
I'd like to acknowledge that our event tonight is held on the land of the Wadawarrung people of the Kulin nations, the traditional custodians of the land, and we pay our respects to elders past and present.

## Overview

>  "Be a voice not an echo"

This is one of my favourite quotes from Albert Einstein - a man who continually innovated, who picked apart problems, who was a deep thinker and held unconventional views. My hope is that after tonight's session you'll be able to form your own informed opinions about voice technology - what it is, where it's going, and how it should form a part of your organisation's technical strategy and roadmap.

So, what are we going to cover tonight?

* A brief history of computer interaction

We'll take a look at how voice is a natural evolution in many ways for human computer interaction

* Voice in fiction and voice in real life

We'll look at how voice technology is represented in fiction, and talk a little bit about how it's set our expectations for how voice should work in real life - and how there's still a bit of a difference between fiction and reality.

* Different voice technologies

We'll look at the different voice technologies that are available currently in the market, and where they sit on a continuum of complexity from simple to advanced.

* Anatomy of a voice stack

Digging a bit deeper into the technology itself, we'll take apart the voice technology stack, and take a deep dive into how different layers in the stack work.

* Challenges and opportunities of Voice

We'll take a look at some of the use cases for voice - and why it works in some situations much better than typing or touch. We'll also look at some of the challenges in voice, and how the technical community is overcoming them.

* Your action plan

We'll finish off the session by chatting about what you can be doing in your organisation to prepare for voice, and what you need to be thinking about for your technical roadmaps and strategies.

## A brief history of computer interaction

Some of you in the room might be old enought to remember these - punch cards - and older computers in the 1960s and 1970s were programmed this way - by punching cards with a program or routine and then loading the cards into the computer - which was usually the size of a house.

We moved on to keyboard input - and then in the mid 1980s the mouse came along and the graphical user interface was born, popularised by the Apple Mac. We started to move into touch interfaces with graphical tablets - shown here with this Wacom Bamboo pen, and then both mobile phones and even computers themselves adopted touch based displays.

SLIDE: Keyboard
SLIDE: mouse
SLIDE: Bamboo tablet
SLIDE: Wiimote

We've also seen a rise in what we call gesture control - for instance the Wiimote uses gestures in the Wiimote controllers to figure out how fast you moved, and where you moved.  We're seeing gesture control being used a lot more extensively in interactive displays such as this one.

SLIDE: Interactive display

So, you can see a natural evolution here.

SLIDE: Voice technology

Voice technology is another natural evolution for human computer interaction - instead of using a pointer or gestures, it uses the power of speech to control what a computer does.

## Voice technology in fiction and in real life

And of course this power of speech has been used significantly in fiction - predominatly sci-fi. Shall we take alook?

https://youtu.be/fJfkYjrbPS4?t=1m32s
Data talking to computers

https://youtu.be/OtPnZXfjKf0?t=6s
Knight rider - KITT

https://www.youtube.com/watch?v=sAz_UvnUeuU
Scottish elevator

Scotty talking to computer
https://youtu.be/xaVgRj2e5_s

Swedish man locked out of House
https://www.youtube.com/watch?v=sgJLpuprQp8

### Themes coming out of voice technology

So you can see that although some of these are quite funny - the Scottish elevator gets me every time - they raise really interesting questions about the challenges of voice technology.

What were some of the issues that you heard in the videos?

* Robotic sounding voices
* Difficulties understanding accents
* Difficulties understanding changes in a person's physical state - dentist
* Poorly recognised intents, the system didn't understand
* No manual override or easy way to achieve something without voice

## Voice stack

So let's have a closer look at the technologies in a voice stack so we can pull apart what's happening in some of these videos.

* Wake Word
  - siri!, alexa, hey mycroft, cortana
* Utterance
* Speech to text
  - different languages
  - phonemes
  - being able to differentiate sounds
  - training datasets for speech to Text
  - commercial imperatives - some languages have a lot more speakers than others
* Intent
  - understanding what the user is trying to do
  - context can often be an issue here
* Processing / Skill / gathering data
 - the need to go out to the internet to get data then come back
* Text to Speech
  - robotic sounding voices

### Accents and racial diversity

Another key issue for voice technology is the recognition of accents in people who may speak the language of the device as a second or other language. Because Speech to Text datasets are trained on samples, often those samples come from a very narrow cohort of people - for instance, white, middle aged men - and you'll probably find that your voice assistant recognises you better if you're a white, middle aged man than if you're say a woman, or a child, or have an accent.

So, if you're using voice technology in your organisation, it's something that you need to be really mindful of, particularly if your organisation serves cohorts that may not be covered well in voice recognition.

SLIDE: Common voice

One of the initiatives in this space is the Common Voice project from Mozilla - the people who make the Firefox browser,

### What does your voice assistant know about you?

SLIDE: Privacy

In order to gather the data that is used to train speech to text and text to speech engines, many voice assistant providers require that you send your data - your _utterances_ to them - as part of their Terms of Service. This way, they're able to accumulate huge amounts of data for training purposes.

But understandably, some people feel quite uneasy about this.

These devices, by their nature are "always on" - they're always listening, and this means that they can sometimes "leak" information about you or your household unintentionally.

SLIDE: Alexa privacy

And that's exactly what happened in Portland, Oregon in May - Alexa was listening in in a room where people were talking, and misinterpreted an intent to "record" a conversation, then sent that recording to someone on a contacts list - accidentally - there was no evidence of hacking, or foul play here - Alexa simply got the Intents wrong.

And this is one of the downsides of this technology at the moment - it raises all sort of questions about not only **what** is being collected but what the companies that collect that data are able to **do** with it.

Does anyone want to hear what's able to be heard when a voice assistant is listening? In this demonstration, we will only hear snippets from Wake Word recordings, and I want to assure people that the people you will hear have explicitly opted in to have their voice recordings stored as part of an open data set. For further privacy assurance, I can't identify any of the people in these recordings - the data has been de-identified so that I can't tie any of the recordings to an individual.

DEMONSTRATION OF PRECISE Wake Word listener

### Sexism in voice technology

Did you notice that in all of the video examples I showed, the voice that was portrayed was female? There's a reason for that. 

One of the other challenges we have around voice technology is sexism. Have you ever wondered why so many of the voices for voice assistants are female? Well it turns out that all of us - women included - are more comfortable giving orders to a female sounding voice than a male sounding voice. So that's definitely something to ponder.

### Haber's classification of contexts

One of the considerations for voice is that we might not be in a private office or personal space when we're using voice technology.

How many people have been on a crowded train when someone decides to start having a very loud phone call? Well the same effect is present for voice assistants - imagine if the 600 people on the Geelong to Melbourne train all started to use their voice assistant at once?

So Haber came up with this classification system to think about as we explore voice technology - for understanding the **contexts** in which it can be used

* Intimate space
* Personal space
* Social space
* Public space

It's only appropriate to use voice technology in some of those contexts.

## Positive use cases for voice

* **We're becoming increasingly distracted** - work and family life is blending, and we're often trying to do many things at once. It's more natural for example to speak while you're driving than to look down at your mobile phone and to try and type something in -

* so voice has a place in environments where the user would otherwise be very distracted, such as **driving, or operating machinery**, or plant equipment - where they need to "keep they're eyes on what they're doing".

* Information at our fingertips - we don't plan anything anymore - which route we'll be travelling in a car, what we'll have for dinner or how we will get there, what to buy - a lot of these decisions have been moved to what we call **just in time** - because technology has all those answers for us at our fingertips. So voice has a very strong role to play there

* **Always on, ubiquitous** - we've come to expect that technology will "just work" - wherever we are, anytime and anywhere. Voice technology helps to fulfil on that promise. For instance, we saw in the smart home video, that the whole house is automated, and voice has a place in ubuitous environments like that.

## Action plan for your voice stack

* Understand who your audiences are - do they have any special voice characteristics? Accents?
* What are the repeated interactions in your organisation? Where are there examples in your organisation where voice would be of assistance?
* Keep in mind Haber's contexts!
* How would voice help? Would it be a hindrance?
* Small steps - plan out specific uses cases
* Small scale testing - is it valuable - if so scale, iterate
* Be aware of the challenges and biases of voice - sexism.

## Questions and comments
