---
layout: post
title: "Sonarqube"
description: 
headline: 
modified: 2015-02-17
category: webdevelopment
tags: [jekyll]
imagefeature: technology.jpg
mathjax: 
chart: 
comments: true
featured: true
---

What is Sonarqube
Sonarqube is a open source Quality management tool. SonarQube is a web based application. SonarQube can be extended by plugins and can be integrated into IDEs.  This tools support 20+ languages.

How to install Sonarqube in Windows
First go to the Sonarqube website http://www.sonarqube.org/. Current  latest version is SonarQube 5.5 . download it.  Then download the analyzer from  http://docs.sonarqube.org/display/SCAN/Analyzing+with+SonarQube+Scanner unzip both files to
c:\sonarqube\ . 
Then you have to add your jdk path to the wrapper.conf file in  C:\sonarqube\sonarqube-5.5\conf\
Mine was at "#wrapper.java.command=C:\Program Files/Java/jdk1.7.0_79/bin/java". 
After that you should add Sonarqube scanner to your environment variable so that we can run it from any where we want. You should add "C:\sonarqube\sonar-scanner-2.6.1\bin\" according to our example. Go here to see how to add environment variables.
After that go to your project main folder and add a "sonar-project.properties" file with below content.

<code>
# must be unique in a given SonarQube instance
sonar.projectKey=my:project
# this is the name displayed in the SonarQube UI
sonar.projectName=My project
sonar.projectVersion=1.0
</code>
<code>
# Path is relative to the sonar-project.properties file. Replace "\" by "/" on Windows.
# Since SonarQube 4.2, this property is optional if sonar.modules is set. 
# If not set, SonarQube starts looking for source code from the directory containing 
# the sonar-project.properties file.
sonar.sources=.
#Path to test derectories(comment if no tests)
#sonar.tests = Testdir
</code>
<code>
# Encoding of the source code. Default is default system encoding
</code>
<code>
#sonar.sourceEncoding=UTF-8
</code>

After that we can start the server and analyze the source code. To start the server go to
"C:\sonarqube\sonarqube-5.5\bin\windows-x86-64" and run "StartSonar.bat".  by right clicking and "Run as Administrator". Then server will start. Then got to your projects main folder by command prompt and type "sonar-scanner". It will analyze your project. To see the results  you can open a browser and go to "http://localhost:9000". 