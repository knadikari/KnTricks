---
layout: post
title: "Install Ruby in Windows"
description: 
headline: 
modified: 2015-02-17
category: webdevelopment
tags: [jekyll]
imagefeature: Ruby.jpg
mathjax: 
chart: 
comments: true
featured: true
---



Ruby is an object oriented language

Main different installing Ruby on Windows than Linux and Mac os is that Windows need "Ruby installer" to install ruby Linux and Mac need rbevn or RVM to install ruby.
<h3>
Method 1
</h3>
First download and install Ruby installer for windows from "http://railsinstaller.org/en".
With this installer you get the chance to install git and this will automatically add  necessary  environment variable to the system. 

![Startmenu]({{ site.url }}/images/post5/1.png) 

After the installation you can config and use git. 

![Startmenu]({{ site.url }}/images/post5/2.png) 

From this installation the Ruby dev kit is also installed so you do not have to download and install it manually. 
To see whether that Ruby is installed correctly type "ruby -v" in the command line and see whether it gives the version of ruby. 

![Startmenu]({{ site.url }}/images/post5/3.png) 

If you did not get that add Ruby to your environment  variable. My path is "C:\RailsInstaller\Ruby2.2.0\bin". How to add environment variable

To see whether the devkit also installed correctly you can type 
"gem install json --platform=ruby" in the terminal this will install a gem called "json"  to ruby

![Startmenu]({{ site.url }}/images/post5/4.png) 
<h3>
Method 2
</h3>
Go to "https://www.ruby-lang.org/en/downloads/" page and download the latest stable Ruby installer.


RubyGems
Gems in ruby are some ruby code (actually these are like libraries) that has been packaged for easy distribution. RubyGems is the package manager that manages those gems.
To make sure we have RubyGems type "gem -v" on the command prompt.

![Startmenu]({{ site.url }}/images/post5/5.png)  

You can get the gems list you have by typing "gem list"

![Startmenu]({{ site.url }}/images/post5/6.png) 

To update the gems you can type "gem update --system". This will check and update your gems to their latest version.

if you want to install a gem "gem install nameofthegem [--version versionnumber] --no-ri --no-rdoc".
if you do not give a version number this will automatically install the latest version. "--no-ri --no-rdoc" mean that not to download the document for the gem. Those document take lot of space and lot of time to generate. They are available online. 


