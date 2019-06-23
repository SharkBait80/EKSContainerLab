# Module 3: Configure your Windows Server 2019 Dev Environment

**Time to complete:** 20 minutes

**Services used:**
* [AWS EC2](https://aws.amazon.com/ec2/)
* [AWS CloudFormation](https://aws.amazon.com/cloudformation/)
* [AWS Identity and Access Management (IAM)](https://aws.amazon.com/iam/)

## Overview

In this module, we will use AWS EC2 to launch and configure our Windows Server 2019 Dev Environment.

<a id='dev-env'></a>
### Your Windows Development Environment
Your Windows workstation environment needs to have the following tools configuration.

**A Dev-Environment with the following development tools.** 
1. Visual Studio 2019 Community Edition (https://visualstudio.microsoft.com/vs/community)
2. .NET Core SDK (https://dotnet.microsoft.com/download/visual-studio-sdks)
3. AWS Tools for Visual Studio (https://aws.amazon.com/developer/language/net/tools/)
4. AWS Command Line Tools (aws)  (https://aws.amazon.com/cli/)
5. .NET Portability Analyzer (https://marketplace.visualstudio.com/items?itemName=ConnieYau.NETPortabilityAnalyzer)
6. Cmder (https://cmder.net)



**Your Windows Workstation - A Remote AWS Windows Server 2019 AMI Instance**

1. For this lab, we utilize an EC2 hosted **Microsoft Windows Server 2019 Base with Containers** instance.  This Amazon Machine Image (AMI) is preconfigured to support Docker Containers.
2. Don't know how to create an EC2 instance?  Please refer to step-wise documentation at (https://aws.amazon.com/getting-started/tutorials/launch-a-virtual-machine/). 
3. When creating your AMI instance, be sure to select the **Microsoft Windows Server 2019 Base with Containers** AMI-type.  We recommend utilizing a **t2.xlarge** or better host-machine type. 
4. Refer to  <a href="#appendix-a">**Appendix A**</a> herein for instructions on accessing your AMI instance via Remote Desktop Protocol (RDP). 

**Proceed with installation of the following tools only after completion of the above workstation guidance.  Lab instructions are to be executed from a RDP client application.**

**Update and configure your Windows Workstation**







That concludes Module 3.

[Proceed to Module 4](/module-4)



<a id='appendix-a'></a>
## Appendix B : Connect to your Windows Server 2019 Development Environment

### Connect to Your EC2 Development Instance

You should have already created an EC2 instance.  You will use an RDP client (such as Remote Desktop Connection, mstc.exe, included with most versions of Windows) to connect to your server. 

1. Open the *Instances* view within the *AWS EC2 Console*.  Select your Windows Server instance and press *Connect* as illustrated.

![AWS EC2 Console](/images/WindowsAMI-Connect-1)

2. From the *Connect to your Instance* dialog window, press *Download Remote Desktop File* and subsequently press the *Get Password* button.  Save this password to a text file for subsequent copy/paste usage.

![Downlaod RDP File](/images/WindowsAMI-Connect-2)

If you are running Mac OS X, <a href="#rdp-MACLinux">skip to the MAC specific section below</a>.

### Windows Users - Connect to Your Windows Instance

1. Using Windows Explorer, locate the RDP file previously downloaded. 
2. Click the file to open the Remote Desktop Protocol application.  
3. Provide the previously saved Administrator account password to logon to the remote Windows instance.

<a id='rdp-MACLinux'></a>
### MAC/Linux Users - Connect to Your Windows Server 2019 Development Environment 

you can install the **Jump Desktop** application from the AppStore, or, download the CoRD RDP client: [*http://cord.sourceforge.net/*](http://cord.sourceforge.net/).

1. Open your RDP client, then configure:

* **Server:** Paste the value of **Public DNS** address of your remote Windows instance.
* **Username:** `\Administrator`
* **Password:** Paste the value of **WindowsPassword** located to the left of these instructions

1. Click **Connect**.

<a href="#dev-env">Return to the top of this file</a>



## [AWS Developer Center](https://developer.aws)

