---
title: Beginners guide to using ZSH in Windows 10
date: "2019-04-07"
template: "post"
draft: false
slug: "/posts/using-zsh-in-windows/"
category: "Poweruser"
tags:
  - "web"
  - "Technology"
description: "To become very efficient and productive is very important in the tech world. Having the right tools to get the job done faster is essential. No tool comes to the heart of developers than a good terminal. Thus, I decided to explore the Z-Shell for Windows environment. Nut right?"
---

Just this morning while trying to make my command prompt look a bit more like linux using [cmder](https://cmder.net), I quickly switched to [Wesbos](https://twitter.com/wesbos) course on [Command Line Power User]()  

What struck me was the bash terminal he was using. It looked really pretty and I told me self, "I what something like this". So in his course, he taught about Zsh & Z. I did a little study and research and soon got hooked up with [Zsh](https://ohmyz.sh) terminal  which is an extended Bourne Shell with a large number of improvements. I had to get it running on my system. But the problem was, I was using WINDOWS 10, OUCH!

But I determine to get it running, so I had two choice, Install Windows Linxu Subsystem like or Cygwin. I went for both. (Laughing seriously here)

This is the final look of what I am trying to achieve:
![Zsh Prompt](/media/zshprompt.png)

To get started these are the steps I took

1. Go to programs and features in your Control Panel
2. __Enable__ **Windows Subsystem for Linux** by clicking on Turn windows features on or off 
3. Visit [Windows Store](https://www.microsoft.com/en-lr/search?q=linux) and install any Debain Flavor Distro you wish. I installed Ubuntu.
4. After installation, set a username and password and you are good to go
5. Install Zsh <pre>sudo apt-get install zsh</pre>
6. Visit [Oh-my-Zsh](https://ohmyz.sh/) home page and copy the installer links provider
7. After installation, you will have a .zshrc file created in your home directory: 
	<pre>ls -la</a>
8. Open with <pre>nano ~/.zshrc</pre>
9. Change the ZSH_THEME from its default to 

Check if the command prompt understands "agonster" fonts and its characters that were used by running this code in your command promt:
	<pre>echo "\ue0b0 \u00b1 \ue0a0 \u27a6 \u2718 \u26a1 \u2699"</pre>

Visit [Agonster](https://github.com/agnoster/agnoster-zsh-theme) for more understanding.
 
<pre style="color:#DC143C">Note: To use Agonster Theme, you'll have to install <a href=" https://github.com/powerline/fonts" target="_blank">[Powerline Fonts]</a></pre>


After all these, you are good to go.

If in doubt with all these steps, I will suggest you take a look at [Wesbos CommandLine Course](http://commandlinepoweruser.com/)

There is just one error in the command prompt I'm trying to resolve and that's the unicode \ue0a0 and hope to update this blog soon.

Till then, **#KeepLearning**