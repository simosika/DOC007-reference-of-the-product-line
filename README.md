# How to establish your own Corolla production line

We start by creating necessary services to help us manage passwords and other project information. In this case I use gigapossu@gmail.com as example account to help you get through various phases of service creation.

**Table of Contents**
- [Password management](#password-management)
- [Communication channel](#communication-channel)
- [Work organization](#work-organization)
- [Diagrams](#diagrams)
- [Tool integrations](#tool-integrations)
- [Managing the code](#managing-the-code)
- [Continuous Integration and Deployment](#continuous-integration-and-deployment)
- [Feedback](#feedback)
- [Mockups](#mockups)
- [Platform for App Deployment](#platform-for-app-deployment)

## Password management

First useful service we should establish is a password management service. In our case CommonKey has proven itself a good option, but you may also use something else if you want. Just keep in mind that proper password management saves you from a lot of trouble in managing your project passwords.

![CommonKey account creation](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A18%3A39.png)

![CommonKey account confirmation](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A19%3A56.png)

When you have created an account and logged in you may install browser extension to make password management easier, but it is not mandatory. At the time of writing this guide the said browser extension was not available, so don't worry too much if you aren't able to install the browser extension.

![CommonKey company creation](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A30%3A27.png)

![CommonKey teams](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A33%3A39.png)

![Invite users to CommonKey company](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A35%3A15.png)

As you can see from the screenshots, it is possible to manage your password sharing with all kinds of options, for example creating teams inside your main account or just simply creating one company account without teams, whatever floats your boat. The most simplified option would be of course to just use one account without company option and share the password with all the users that have access to your projects' passwords, but feel free to compare pros and cons between various approaches. To avoid using too much time into tinkering with password management, it would be wise to go with somewhat simple approach, though.

To create an example scenario here we've created our password account in CommonKey with two methods, Auto-login and Custom app. The rule of thumb is that if your application of choice is listed in Auto-login, it should be used, otherwise use Custom app.

![CommonKey password account with auto-login](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A43%3A51.png)

![CommonKey password account with custom app](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A44%3A56.png)

After creating a password account you can open its details by clicking it on the list, in this example we are using personal Gmail account. When you have opened the account details, you can edit your password details, show the password in plain text for a few seconds, or copy it to your clipboard to paste it to your login of choice.

![CommonKey copy password to clipboard](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2014%3A50%3A10.png)

## Communication channel

One of the most important cornerstones in every teams' ability to work together is communication. Our project has tried a couple of different platforms for communication, and we are currently using Slack. Slack is versatile, configurable, can be integrated with several other tools and most importantly, it is free. So let's go ahead and establish our own communication project for our project in our next step.

![Slack create a new team](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2015%3A09%3A41.png)

Let's navigate to https://slack.com/ and create a new team. To create a new team sign up with your email address. It is completely up to you if you want to receive email notifications about Slack service.

After you've named your Slack channel, you have to create an url to be able to access it. You might want to use a bit more imagination to create something a bit more practical and compact than what's used in this example, but please keep in mind that URL has to be unique so in cases of very short URLs you might be limited by addresses already reserved by other users.

In the last step of creating our slack channel you'll choose your username. It is tough to give recommendations on this one, although you might want to steer away from too complicated or offensive usernames, just in case. In this example I decided to stay on my very imagination-limited path.

![Slack confirm account details](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2015%3A23%3A35.png)

In case everything went well so far, you'll have a chance to see your choices so far and confirm that this is indeed what you'll want to do. If you are confident on your choices, by pressing the button below you are able to establish your own Slack channel, and start inviting people to it.

Now you can start customizing your fresh communication channel. Enabling desktop notifications is optional, but helps quite a lot in being able to notice urgent messages that are being sent to you over Slack. Slack also has mobile applications if you get a feeling that you'd like to be available better or there's one tab too many open in your web browser. Either way setting your Slack channel up is pretty simple. With “invite people” you'll be able to add members to your communication channel. At the time of writing, “full member” is the only available account type for free Slack accounts.

![Invite people to Slack team](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2015%3A30%3A22.png)

 ![Creating a new channel](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-06%2015%3A34%3A47.png)

It is possible that you can manage with the channels that have already been provided to you by default, but at least in case your team has several teams with different purposes within it (teamception?) it is possible to create new public/private channels for controlling the conversation. Or you can just create different channels for different topics if you want. Creating a private channel allows you to strictly decide who gets to participate in conversation, and the rest of users will not be able to see this private channel without invitation.

Once you've created your Slack channel, you'll receive an email that asks you to set a password for your account. You should do that to avoid being confused by the fact that when you try to log back in to your channel it will prompt you for a password, which you have not even set, thus making it impossible for you to login before the password has been set.

After you've added a password for your Slack account, it is recommended to add this password to your password management of choice. You might want to write your domain name and other information about your Slack channel somewhere to avoid confusion for example in case you want to log in to your channel from other device.

## Work organization

![Trello front page](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2011%3A03%3A16.png)

The next tool we should establish in our quest for viable production environment is Trello. Trello can be effectively used for tracking progress of your project and it can also be integrated with Slack. With a little imagination you can find creative ways to benefit from Trello, such as sharing materials and images related to your project phases and dividing your project into smaller, easily manageable parts.

![Trello boards](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2011%3A13%3A28.png)

![Creating a new Trello board](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2012%3A54%3A17.png)

Confirm your account via email message and start getting to know Trello. Let's have a short tutorial on how to use Trello. The default board called “Welcome Board” can be used to familiarize yourself with Trello and get some useful tips on how to use it along the way. After that you might want to create a new board for your project. When creating a new board you'll be able to assign new teams or change your board type between setting private, team and public. Of course you won't be able to use team setting unless you have already created some teams. In the most simple scenario where you have a small team working on a single project you can just create a public  board that you can name with its purpose. Here's a simple example of tasking board with Kanban-influenced workflow.

![Trello example board](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2013%3A13%3A54.png)

![Adding new users to Trello](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2013%3A47%3A22.png)

Adding new users to your board can be done via the menu in right corner of your board. Public boards can be seen by everyone but edited only by members of the board. Private boards are only seen and edited by members.

## Diagrams

Lucidchart can be used for making diagrams and you can think of it as a free replacement to Microsoft Visio. There are lots of free alternatives to programs like this, but compared to Dia, for example, Lucidchart has a benefit that it's online-based and this makes sharing your diagrams with your team and other parties a lot easier.

![Lucidchart front page bar](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2015%3A02%3A08.png)

![Lucidchart free account](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2015%3A02%3A49.png)

![Lucidchart account creation](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-09%2015%3A21%3A14.png)

From the front page click “sign up free” and in the next screen below the paid subscriptions you can find option to start free account. Free accounts have some complexity restrictions in diagrams and other hindrances, but it should be fine for most small project cases. Lucidchart includes a lot of templates you can use for making your diagrams easier, and tips and tutorials can be useful if you don't know how to start. In the main screen you can create new diagrams or edit existing ones. 

As you can probably see pretty soon, the default forms and shapes won't get you very far. Therefore it is good that you can add more shape libraries by clicking “more shapes” in the lower left corner and choosing the libraries you believe are useful to your use case. Then save and you are free to start creating diagrams. In the upper left corner you can name your flowchart and just below it, next to “file” menu you can see Lucidchart icon. By clicking it you can activate “Go to documents” option, which returns you back to the main screen. 

Hint: When you create a new shape that has been equipped with a default name, you can double click this name to modify it. Same actually applies to lines you can draw between items; you can double click somewhere along the line to make a text box on the point of click.
Hint 2: When using a background for your other icons, for example the cloud in this topology image, it is recommended to first create, name and arrange icons and then add the background and send it to background with mouse button 2 menu. Otherwise Lucidchart might get confused with the object user wants to interact with.

Here's a quickly made example wannabe-topology that is ugly and crude and has no deeper meaning. It's here just as an example of typical scenario when you would need Lucidchart: drawing topology images.

![Topology made with Lucidchart](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-10%2011%3A43%3A45.png)

## Tool integrations

Zapier is a tool that can be used for many purposes. Most commonly, it is used to create integrations between services that do not have native support in themselves to be integrated. Of course, integrations done with Zapier are not as well-executed as official implementations, but in some cases if you simply want some of your tools to transmit data into another the Zapier is the way to go. In our use case we have at some point of our project used Zapier for transferring our UserVoice tickets to our GitHub issues.

## Managing the code

![Join GitHub](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2013%3A37%3A16.png)

![Choose GitHub plan](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2013%3A38%3A20.png)

GitHub is a very important tool for managing your code and making it easily accessible to use in various environments. Create your account by clicking “sign up” and provide the account with your user information. In this case I'm using N4S project repositories that have been created earlier, but in your case you'll probably want to know how to create private repositories provided by JAMK. After adding some of your account information confirm your email via link that you've received to your accounts' address and feel free to explore how GitHub works. In this case I've created a private repository called gigacorolla-toolchain for N4S project and used my main account to invite our Gigapossu user to that private repository. After our GitHub account has been set up and has a repository to work on, we are set to initiate our CircleCI account. In your case your organization will probably be JAMK-IT but otherwise the process should be somewhat similar.

## Continuous Integration and Deployment

![CircleCI GitHub integration](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2013%3A57%3A23.png)

![CircleCI GitHub authorization](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2013%3A58%3A22.png)

![CircleCI testing and deployment](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2014%3A27%3A55.png)

CircleCI is a tool used for Continuous Integration and Deployment. From the front page, click “Sign up free” and create an account. After that, “Add code from GitHub” and you should be provided with login screen or in case you're already logged in, you'll be asked to authorize CircleCI to use your GitHub account with listed permissions. At this point it's good to know that you'll have to have admin permissions to repository you're about to add to CircleCI. The next part depends on whether you've created a private repository for your account or your organization. In this case the repository has been created for our organization, N4SJAMK, so we choose that as an organization and because we only have privileges to gigacorolla-toolchain repository under this organization we select it for our repository. After that click on “Build project” next to your chosen repository. Because in this case our repository was just about empty with no code to build, we received some warnings in the process. That issue will be fixed when we've got our code underway in GitHub, and this phase is not really relevant in case your GitHub repository doesn't have anything meaningful in it.

## Feedback

Choosing a user feedback system is a bit more complicated issue. We used UserVoice for quite a while to collect feedback from our Contriboard, and as integration with our issue listing was not possible from the start, we used Zapier to export our feedback tickets from UserVoice into GitHub issues. We were satisfied with UserVoice and it served us well. However, since then things have become a bit more complicated. UserVoice has changed its payment model drastically. When we used it they had free account option that was limited in some functionalities but didn't have any kind of trial period or something that was severely limiting our basic usage. Since then they have moved to radically different pricing methods. Now they have 14 day free trial and first pricing option starts from 499$ a month. So now we're in a situation where we'll have to find another free alternative that has the necessary integrations or implement those integrations manually with Zapier.

## Mockups

![NinjaMock front page](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2011%3A09%3A28.png)

![NinjaMock project selection](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2011%3A10%3A07.png)

![NinjaMock user interface](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2011%3A10%3A48.png)

![NinjaMock create account](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2011%3A13%3A44.png)

For designing our first piece of software we can use a wide variety of tools. First up, in this guide we introduce NinjaMock. We start up by clicking “start designing now” on the front page, choosing our platform, in this case preferrably www, and then we are already on the design interface. At this point we'd probably want to create and account from the top right corner to maintain our progress. After creating an account you create a new project and again, choose your platform of choice and you're back in program user interface, this time logged in with your account. 

![Big red button original](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2012%3A29%3A08.png)

![Big red button well done](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2012%3A48%3A08.png)

![NinjaMock page linking](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-13%2012%3A53%3A15.png)

In this example we created a very simple point of interaction, a big red button you can press. First we take two circles from shapes, one larger than the other, the same height and width per circle. Then we set them on top of each other, set colours from fill brush via menu. You can add labels via basic menu on the left, and make your object clickable by adding a click spot. After that create a new page from the bottom of the page by pressing “add portrait page” button. The easiest way to do what we're about to do here is to select the button and its texts in their entirety and copy them to page 2, but you might want to remove clickable area from your button before copying. Try to set the button on page 2 into same place where it is on your page 1 by following height and vertical movement indicators. After you've done this you can add the clickable area again to page 1 and link it to page 2. Change the texts on page 2 so you can clearly see that the page changes when you click on the link you have created. Now you can preview your page from preview button on upper right corner and see if your mockup works as it should.

## Platform for App Deployment

![Heroku account creation](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2014%3A36%3A48.png)

![Heroku account creation finished](https://dl.dropboxusercontent.com/u/27852594/Screenshot%20from%202015-11-27%2014%3A55%3A09.png)

Heroku is our site of choice for building our app in working condition. This is basically where our application is deployed after being tested and compiled in CircleCI. To create your account click “Sign up for free” and once again, fill in the necessary information to get your account initiated. If you already have in mind what programming language you're about to use for your project then go ahead and select it from the menu, but Heroku also has couple of options in case you're not so sure. After filling out the account information you'll be asked to confirm your email account. After confirming your account you'll be prompted to set password to your account. Do so and log in.
