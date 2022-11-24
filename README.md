---
page_type: sample
languages:
- cpp
products:
- windows-api-win32
name: V2 Credential Provider Sample
urlFragment: credential-provider
description: Demonstrates how to build a v2 credential provider that makes use of the new capabilities in credential provider framework in Windows 8 and Windows 8.1.
---

# V2 Credential Provider Sample

Demonstrates how to build a v2 credential provider that makes use of the new capabilities introduced to credential provider framework in Windows 8 and Windows 8.1.

To get a copy of Windows, go to [Downloads and tools](http://go.microsoft.com/fwlink/p/?linkid=301696).

To get a copy of Visual Studio, go to [Visual Studio Downloads](http://go.microsoft.com/fwlink/p/?linkid=301697).

## Operating system requirements

Client

Windows 8.1

Server

Windows Server 2012 R2

## Build the sample

1. Start Visual Studio and select **File** \> **Open** \> **Project/Solution**.
2. Go to the directory named for the sample, and double-click the Visual Studio Solution (.sln) file.
3. Press F7 or use **Build** \> **Build Solution** to build the sample.

## Run the sample

To run this sample, build the project in **Release** configuration. Find ```SampleV2CredentialProvider.dll``` in your build folder, and place it under ```C:\Windows\System32```. Then run ```register.reg``` to register the dll. At last press **```Win + L```** and you will be brought to the login page.

To uninstall the Credential Provider, remove ```SampleV2CredentialProvider.dll``` from ```C:\Windows\System32``` and run ```Unregister.reg```.

> It is recommended to test Credential Provider in a virtual machine. Since, it might break something if you're not aware.