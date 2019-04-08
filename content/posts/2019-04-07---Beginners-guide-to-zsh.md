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

Just this morning while trying to make my command prompt look a bit more like linux using <a href="https://cmder.net" target="_blank">cmder</a>, I quickly switched to <a href="https://twitter.com/wesbos" target="_blank">Wesbos</a> course on <a href="http://commandlinepoweruser.com" target="_blank">Command Line Power User</a>

What struck me was the bash terminal he was using. It looked really pretty and I told me self, "I what something like this". So in his course, he taught about Zsh & Z. I did a little study and research and soon got hooked up with [Zsh](https://ohmyz.sh) terminal  which is an extended Bourne Shell with a large number of improvements. I had to get it running on my system. But the problem was, I was using WINDOWS 10, **OUCH!**

But I determine to get it running, so I had two choices, Install Windows Linux Subsystem like or Cygwin. I went for both. (Laughing seriously here) 

This is the final look of what I am trying to achieve:
![Zsh Prompt](/media/zshprompt.png)

To get started these are the steps I took

1. Go to programs and features in your Control Panel

2. __Enable__ **Windows Subsystem for Linux** by clicking on Turn windows features on or off 

![Cpanel](/media/cpanel.png)
3. Visit <a href="https://www.microsoft.com/en-lr/search?q=linux" target="_blank">Windows Store</a> and install any Debain Flavor Distro you wish. I installed Ubuntu.
   ![Windows Store](/media/windows_store.png)
4. After installation, set a username and password and you are good to go
5. Install Zsh  
   
   ```sudo apt-get install zsh```

6. Visit <a href="https://ohmyz.sh/" target="_blank">Oh-my-Zsh</a> home page and copy the installer links provider
7. After installation, you will have a .zshrc file created in your home directory:

	```ls -la``` 
![ZSHRC](/media/cmd-prompt.jpg)

8. Open with ```nano ~/.zshrc```
9. Change the ZSH_THEME from its default to 

Check if the command prompt understands "agonster" fonts and its characters that were used by running this code in your command promt:

```echo "\ue0b0 \u00b1 \ue0a0 \u27a6 \u2718 \u26a1 \u2699"```

Visit <a href="https://github.com/agnoster/agnoster-zsh-theme " target="_blank">Agonster</a> for more understanding.
 
<pre style="color:#DC143C">Note: To use Agonster Theme, you'll have to install <a href=" https://github.com/powerline/fonts" target="_blank">Powerline Fonts</a></pre>


After all these, you are good to go.

If in doubt with all these steps, I will suggest you take a look at <a href="http://commandlinepoweruser.com" target="_blank">Wesbos CommandLine Course</a>

There is just one error in the command prompt I'm trying to resolve and that's the unicode ```\ue0a0``` and hope to update this blog soon.

Till then, **#KeepLearning**

O! lest I forget, you can get a quick understanding on how to use ZSH by visiting this video on <a href="https://www.youtube.com/watch?v=Ojdk1lNXB0E" target="_blank">YouTube</a>

**update**:
I had to replace ```\ue0a0``` to ```u0e0a``` inside the agonster theme by replacing ```PL_BRANCH_CHAR=$'\ue0a0'```  