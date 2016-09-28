<img src="https://cdn-images-1.medium.com/max/497/1*uqOOpzC6f0Bl1QxVG70IBw.jpeg?raw=true">

# Tutorial on building a slack bot with Botkit

This is a tutorial for building a slack chatbot using botkit. (Based on some steps in the [Kazuar](http://kazuar.github.io/building-slack-game-part1/) tutorial)

I love [Slack](https://slack.com/). I's my favorite meeting chat room. My interest in bots leaded me to write this tutorial where you'll see how simple it is to build your own chatbot in slack.

A bot is a piece of software designed to execute scripts to automate tasks that you would normally do on your own, such as make a dinner reservation, or update calendar appointment information. 
Often deployed inside messaging apps, chatbots are a popular way of handling customer service requests. 

<img src="https://wolfpaulus.com/wp-content/uploads/2016/05/slackbot-660x400.jpg?raw=true" width="300">

[Slack](https://slack.com/) has been interested in chatbots a while now. Here are the most popular bots in [Slack](https://slack.com/)  

<img src="https://s3-us-west-2.amazonaws.com/slack-files2/avatars/2016-05-09/41532123248_86c89d7c608b75bbd782_512.png?raw=true" width="48">  Polly by Subcurrent : Smart polls and automated feedback.

<img src="https://s3-us-west-2.amazonaws.com/slack-files2/avatars/2016-05-09/41383466498_0b42b10e4722adcb3653_512.png?raw=true" width="48">  Statsbot : Analytics Companion for your slack team.

<img src="https://s3-us-west-2.amazonaws.com/slack-files2/avatars/2015-12-15/16747060519_b4cbfae7661cabea36fc_512.png?raw=true" width="48">  Howdy : your new digital coworker. Our bot will automate repetitive tasks so you can do the real work.

<img src="https://s3-us-west-2.amazonaws.com/slack-files2/avatars/2015-12-19/17065321733_953d8b35467f5bd029c3_512.png" width="48">  Meekan Scheduling Assistant : matches everyone’s calendars, and quickly finds common free times. 

You will be building a chatbot that lives in slack messaging application with a well known framework : [Botkit](https://github.com/howdyai/botkit) that was made by [Howdyai](https://howdy.ai/) and sold to Slack a few months ago. 

##Building steps: 

**1. Create a slack account**
If you don’t have one already, create one at [Slack](https://slack.com/) and start using it. … or work on something else :)

**2. Regsiter a slack bot**
Go to https://slack.com/apps/build and click on “Make a Custom Integration” under “Something just for my team” 
<img src="http://kazuar.github.io/images/slack_bot/screen1.png">

**3. In the new page, click on “Bots”**
<img src="http://kazuar.github.io/images/slack_bot/screen2.png">

**4. Choose your new slack bot name (i.e. slack_bot) and press “Add bot integration”**
<img src="http://kazuar.github.io/images/slack_bot/screen3.png">

**5. In the new page, copy the API token of the new slack bot as we will need it in our script**
<img src="http://kazuar.github.io/images/slack_bot/screen4.png">

##Prepare the environnement

As indicated, we will use the Botkit 

###Installation

Install Node from here https://nodejs.org, this will be the server environment. Then open up Terminal or Command Line Prompt and make sure you've got the very most recent version of npm by installing it again:
  ```
    sudo npm install npm -g
  ```

Create a new folder somewhere and let's create a new Node project. Hit Enter to accept the defaults.

    ```
    npm init
    ```
Botkit is available via NPM.

```
npm install --save botkit
```

You can also check out Botkit directly from Git.
If you want to use the example code and included bots, it may be preferable to use Github over NPM.

```
git clone git@github.com:howdyai/botkit.git
```

After cloning the Git repository, you have to install the node dependencies. Navigate to the root of your cloned repository and use npm to install all necessary dependencies.
```
npm install
```

You should indicate your slack bot token you copied while creating the bot on Slack a few minutes ago. 

to run the slack bot : 

```
node slack_bot.js
```

See how easy it is to build your bot ? 
Now, the sky is your limit. You can create how many amazing bots as you can. 
**advice:** Check out the facebook messenger bots too, they're cool. 

## Contribute

Contributions are always welcome!
Please read the [contribution guidelines](contributing.md) first.


## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](http://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Rania ZYANE](https://twitter.com/raniazy) has waived all copyright and related or neighboring rights to this work.


