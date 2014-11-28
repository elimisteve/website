---
layout: no-sidebar
title:  "The Start Page"
date:   2014-11-27 19:00:00
categories: [communication, interface]
image: posts/notwritingsoftware.png
---

## Not writing software

Since we started a lot of people are asking us how exactly IndieHosters is different from:

- SandtStorm.io
- classic CMS hosting
- Cpanel
- ..

First of all, I want to state out loud, we are not writing software. Pieces of code you can find on [github/indiehosters](https://github.com/indiehosters/) are mostly configuration and documentation.

IndieHosters is a network of Hosters that share an ideology and a migration format. We have now a "reference implementation" on how to run the migration format. But this implementation is just configuration of industry standard tools - namely CoreOS. (But tomorrow, we'll also have ubuntu, and probably yours)

(Later we'll publish more on the [migration format](http://indiewebcamp.com/one_click_migration)..)

## Oh wait!

### How the user can "control" his software?

This is indeed a good question. Some people did the choice to write software to solve this problem. We call it meta-software, software to manage software. There is already a bunch on the free software market:

- [YunoHost](https://yunohost.org/)
- [Sandstorm](https://sandstorm.io/)
- [arkos](https://arkos.io/)
- [Freedom Box](https://freedomboxfoundation.org/)
- [Cozy](http://cozy.io/)
- [ownCloud](http://owncloud.org/)
- [webmin](http://www.webmin.com/)

And actually, we plan to offer hosting also for these in the future. One of the problem of these software is they are aimed at technical people. And they all have some kind of technical restrictions:
- one VM/hardware per user
- one language for all the applications
- strong opinion on how to run the software

We plan to offer hosting at scale, on shared ressources, and on an easy way.

## Introducing the StartPage

### Socket activation

One of the idea we have in mind is to use Socket Activation. For the non technical people, it means that for a user, all the applications we offer, they will be available from the first registration. And just during the first connection to the application, the software will be started.

So at the end, the start page is basically a static html page with links to the different applications.

We are still at the planning phase, and we have to benchmark this technique, but we are really enthusiastic about this idea.

### Migration button

Then for every application, there will be a migration button that will allow you to switch from one Hoster to another. We believe that this is really our value added for the customer to be able to switch. It's getting closer and closer to the feeling of freedom you could have in the time your data were on your computer.

### IndieWeb use case

If we take the IndieWeb application that we are currently hosting for alpha users and [offering as a pre-sale](https://www.indiegogo.com/projects/indiehosters/x/9169969). To be part of the IndieWeb, is basically having your domain name with a blogging platform.

The plan for registration is:

- get an IndieHoster based on your language
- connect with email/google/facebook/twitter
- choose your domaine name (guessed on your connection)
- access your start page
- access your blogging application (we choose [known](https://withknown.com/) as default)

And on the start page, on the blog section, in "advanced area", you could access other blogging plateforme from wordpress.mydomain.com, ghost.mydomain.com, static.mydomain.com and so on. And you'll also have the possibility to switch your main domain to another one with a click.

## Conclusion

As you can see, it's still on going discussion :) We'd love to hear your feedback on that! But we believe that there is room to develop a good and simple user experience, and not another store/meta-software.

And then the idea is to start with this simple html page, and accept email tickets. And slowly, we'll see the needs appearing. We can't predict the future, but for IndieWeb hosting this is the experience we plan.
