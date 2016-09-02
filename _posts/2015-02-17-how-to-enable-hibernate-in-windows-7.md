---
layout: post
title: "How to enable hibernate in windows 7"
description: 
headline: 
modified: 2015-02-17
category: webdevelopment
tags: [jekyll]
imagefeature: winows7.jpg 
mathjax: 
chart: 
comments: true
featured: true
---

How to enable hibernate in windows 7

<h3>
Method 1
</h3>
1. Type “cmd” in search bar of the start menu and right click on the command prompt and select “Run as administrator” .

![Startmenu]({{ site.url }}/images/post1/trick-1-1.png)

2. Type “powercfg -h on” or “powercfg.exe /hibernate on” to enable hibernate.
3. If still you do not see the hibernate button in shutdown menu go to ” Control Panel\Hardware and Sound\Power Options “.
4. click on the “Change plan settings ” on the selected plan.

![]({{ site.url }}/images/post1/trick-1-2.png)

5. Then click “Change advance power settings”.
6. From the dialog box that popped up expand “sleep” by clicking the “+” sign.
7. Now expand “Allow hybrid sleep” and change the setting to “off”.

![]({{ site.url }}/images/post1/trick-1-3.png)

<h3>
Method 2
</h3>
1. Type ” regedit ” in search bar of the start menu and enter. You can also use “Ctrl + R” and open the run window and type ” regedit ” and enter.
2. When register editting window came up navigate thorough
” HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\Power” in the left side menu. Do not expand the “power” folder.

 ![]({{ site.url }}/images/post1/trick-1-4.png)


3. Then Double on ” HibernateEnabled” on the right side.
4. Change the “value data” to 1 and click ok.

![]({{ site.url }}/images/post1/trick-1-5.png)