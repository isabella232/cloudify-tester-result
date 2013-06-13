---
layout: default
title: .Net SetUp Instructions
---

      For running the .Net SGTest please follow these instructions:
		1. Make sure you have the following installed on your machine:
			a. .Net framework version 2 and 4
			b. Visual studio 2005
			c. [testdriven.net](http://www.testdriven.net/)
		2. Check out the following projects:
			a. svn://svn-srv/SVN/xap/trunk/gigaspaces-dotnet
			b. svn://svn-srv/SVN/xap/trunk/quality/frameworks/DotNetSGTest
		3. Download the a XAP Premium java zip (from tarzan)
		4. Run gigaspaces-dotnet\Build\BuildDev-x86-v20.bat with the path of the zip as an argument
		5. A GS .Net build is created under gigaspaces-dotnet\NET v2.0.50727 update its license in gigaspaces-dotnet\Runtime
		6. Open the DotNetSGTest.sln in visual studio 2005
		7. Either set an environment variable XapNet_<version>_SettingsPath=<Settings.xml file path> (e.g. XapNet_9.5.0.8491-319_SettingsPath=D:\head\NET v2.0.50727\Config\Settings.xml) or set it up in the code
		8. Run gigaspaces-dotnet\"NET v2.0.50727"\bin\Gs-agent.exe gsa.global.lus 1 gsa.global.gsm 0 gsa.gsc 0
		9. In the test class with the mouse in the [test] method right click and select Run test (or Test with -> Debugger)
		