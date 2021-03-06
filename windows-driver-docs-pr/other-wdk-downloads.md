---
title: Previous WDK versions and other downloads
description: Install versions of the Windows Driver Kit (WDK), the Windows Debugger (WinDBG), and more.
ms.assetid: e07d9f05-f8d0-46e5-82e6-c23baa614bb1
keywords:
- Windows Driver Kit
- previous versions
- WDK
ms.date: 05/07/2018
ms.localizationpriority: medium
---

# Other WDK downloads

This topic contains information about earlier versions of the Windows Driver Kit (WDK),
Enterprise WDK (EWDK), and additional downloads for support purposes. To develop drivers,
use the latest public versions of the Windows Driver Kit (WDK) and tools, available for
download on [Download the Windows Driver Kit (WDK)](download-the-wdk.md).


The Windows Driver Kit (WDK) is used to develop, test, and deploy
Windows drivers. To develop drivers, use the latest public versions of
the Windows Driver Kit (WDK) and tools, available for download on
[Download the Windows Driver Kit (WDK)](download-the-wdk.md).

This topic contains information about earlier versions of the WDK, the
Enterprise WDK (EWDK), and additional downloads for support purposes. To
use these earlier versions, you must *first* install the version of
Visual Studio that is appropriate for your targeted platform.


## Step 1: Install Visual Studio

Development of drivers is supported for specific versions of Visual
Studio. To develop a driver for a specific version of Windows, you must
use one of the versions of Visual Studio that are identified (and linked
for download) in the following table.

| Versions of Windows      | Edition(s) of Visual Studio            |
|--------------------------|----------------------------------------|
| Windows 10, version 1803 <br/>Windows 10, version 1709 | [Visual Studio Community 2017](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Community&rel=15) <br/>[Visual Studio Professional 2017](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Professional&rel=15) <br/>[Visual Studio Enterprise 2017](https://www.visualstudio.com/thank-you-downloading-visual-studio/?sku=Enterprise&rel=15) |
| Windows 10, version 1703 <br/>Windows 10, version 1607 | [Visual Studio Express 2015 for Desktop](https://go.microsoft.com/fwlink/?linkid=875331) <br/>[Visual Studio Community 2015](https://go.microsoft.com/fwlink/p/?LinkId=534599) <br/>[Visual Studio Professional 2015](https://go.microsoft.com/fwlink/p/?LinkId=619628) <br/>[Visual Studio Enterprise 2015](https://go.microsoft.com/fwlink/p/?LinkId=619629) |
| Windows 8.1 Update <br/>Windows 8.1 | [Visual Studio 2013](https://go.microsoft.com/fwlink/?linkid=875331) |
| Windows 8                | [Visual Studio Professional 2012](https://go.microsoft.com/fwlink/p/?LinkID=255976) <br/>[Visual Studio Ultimate 2012](https://go.microsoft.com/fwlink/p/?LinkID=255982) |


### Configure Visual Studio for Windows 10, versions 1709 and 1803

When you install Visual Studio, select the **Desktop development with
C++** workload. The Windows 10 Software Development Kit (SDK) is
automatically included and is displayed in the right-hand **Summary**
pane.

To develop drivers for ARM/ARM64, choose **Individual components** and
under **Compilers, build tools, and runtimes** select **Visual C++
compilers and libraries for ARM/ARM64**.

### Install Windows SDK for Windows 10, versions 1607 and 1703

For systems that run Windows 10, version 1607 or Windows 10, version 1703, also download and install the Windows SDK:
[Windows SDK for Windows 10.0.15063.468](https://go.microsoft.com/fwlink/p/?LinkID=845298).

The Windows SDK was not included in Visual Studio 2015, so you must install the SDK separately. Later versions of Visual Studio include the Windows SDK.


## Step 2: Install the WDK

The WDK is integrated with Visual Studio and Debugging Tools for Windows
(WinDbg). This integrated environment gives you the tools you need to
develop, build, package, deploy, test, and debug drivers.

> [!Note]
> Starting with Windows 10, version 1709, installing the WDK
> will by default install the WDK extensions for Visual Studio. These
> extensions are required for integration of the WDK with Visual Studio.

| Versions of Windows      | WDK and related downloads                       |
|--------------------------|-------------------------------------------------|
| Windows 10, version 1803 | [WDK for Windows 10, version 1803](https://go.microsoft.com/fwlink/?linkid=873060) |
| Windows 10, version 1709 | [WDK for Windows 10, version 1709](https://go.microsoft.com/fwlink/p/?linkid=859232) |
| Windows 10, version 1703 | [WDK for Windows 10, version 1703](https://go.microsoft.com/fwlink/p/?LinkID=845980) |
| Windows 10, version 1607 | [WDK for Windows 10, version 1607](https://go.microsoft.com/fwlink/p/?LinkId=526733)                |
| Windows 8.1 Update       | [WDK 8.1 Update](https://go.microsoft.com/fwlink/p/?LinkId=393659) (English only) <br/>[WDK 8.1 Update Test Pack](https://go.microsoft.com/fwlink/p/?LinkID=393660) (English only) <br/>[WDK 8.1 Samples](https://code.msdn.microsoft.com/windowshardware/Windows-Driver-Kit-WDK-81-cf35e953) |
| Windows 8                | [WDK 8](https://go.microsoft.com/fwlink/p/?LinkID=324284) (English only) <br/>[WDK 8 redistributable components](https://go.microsoft.com/fwlink/p/?LinkID=253170) (English only) <br/>[WDK 8 Samples](https://code.msdn.microsoft.com/windowshardware/Windows-Driver-Kit-WDK-80-e3161626) |
| Windows XP <br/>Windows Server 2003 | [WDK 7.1.0](https://www.microsoft.com/download/confirmation.aspx?id=11800) |

<!-- On 02/21/2019, Andy luhrs suggested cutting all of this stuff for Windows 8.1.  I'm leaving this note here for now. [v-gmoor, 2019-03-07]

### Notes for Windows 8.1 Update

#### WinDbg for Windows 8.1

Debugging Tools for Windows (WinDbg) are included in the WDK 8.1 Update,
but you can also install them as a standalone component from the Windows
8.1 SDK. First, download the installer: [sdksetup.exe](https://go.microsoft.com/fwlink/p/?LinkId=323507).
Start the installer, and then in the installation wizard, select **Debugging Tools for Windows**,
and clear all other components.
-->
<!-- On 02/21/2019, Don Marshall suggested cutting this section: "As the former 'Remote Debugging Client for Windows 8.1' in no longer available for remote across the internet partner debugging, I would probably just remove this entire block of text." I'm leaving this note here for now. [v-gmoor, 2019-03-07]

#### Remote Debugging client for Windows 8.1

With the Windows Remote Debugging client, you can work remotely with
developers from Microsoft, over the internet, to debug kernel-mode
failures by using the kernel debugger. For more information about remote debugging,
see [Remote Debugging](https://docs.microsoft.com/windows-hardware/drivers/debugger/remote-debugging).

-   [Download the Remote Debugging client](https://go.microsoft.com/fwlink/p/?LinkId=316921) (English only) -->
<!--edit: Preceding link for the Remote Debugging client for Windows 8.1 is dead, and I haven't yet found a working replacement, unless one of these applies: https://docs.microsoft.com/en-us/visualstudio/debugger/remote-debugging?view=vs-2017#download-and-install-the-remote-tools -->


## Optional: Install the EWDK

The EWDK is a standalone, self-contained, command-line environment for
building drivers and basic Win32 test applications. It includes the
Visual Studio Build Tools, the SDK, and the WDK. This environment
doesn't include all the features available in Visual Studio, such as
the integrated development environment (IDE).

For more information about the EWDK, see
[Using the Enterprise WDK 10](https://docs.microsoft.com/en-us/windows-hardware/drivers/develop/using-the-enterprise-wdk).

| Versions of Windows               | EWDK                              |
|-----------------------------------|-----------------------------------|
| Windows 10, version 1803          | [EWDK for Windows 10, version 1803](https://developer.microsoft.com/windows/hardware/license-terms-EWDK) |
| Windows 10, version 1709          | [EWDK for Visual Studio with Build Tools 15.6](https://developer.microsoft.com/windows/hardware/license-terms-enterprise-wdk-1709-VS15-6) (Recommended) <br/>[EWDK for Visual Studio with Build Tools 15.4](https://developer.microsoft.com/windows/hardware/license-terms-enterprise-wdk-1709-VS15-4) <br/>[EWDK for Visual Studio with Build Tools 15.2](https://developer.microsoft.com/windows/hardware/license-terms-enterprise-wdk-1709) |
| Windows 10, version 1703          | [EWDK for Windows 10, version 1703](https://developer.microsoft.com/windows/hardware/license-terms-enterprise-wdk-1703) |

> [!Note]
> Starting in Windows 10 version 1709, the EWDK is ISO-based. To get started, download and mount the ISO, and then run **LaunchBuildEnv**.


## Optional: Install WinDbg Preview

WinDbg Preview is a new version of WinDbg with more modern visuals, faster windows, a full-fledged scripting experience, built with the extensible debugger data model front and center. WinDbg Preview supports debugging every version of Windows 10.

For download links and more information about WinDbg Preview, see [Download WinDbg Preview](/debugger/debugger-download-tools#small-windbg-preview-logo-download-windbg-preview).


## Standalone tools for debugging Windows XP and Windows Vista

If you're debugging Windows XP, Windows Server 2003, Windows Vista, or
Windows Server 2008 (or using one of these operating systems to run
Debugging Tools for Windows), you need to use the Windows 7 release of
the debugging tools. It's included in the SDK for Windows 7 and .NET
Framework 4.0.

> [!IMPORTANT]
> Newer versions of the Visual C++ 2010 Redistributable can cause
> issues when you install the SDK for Windows 7. For more information, see
> [Windows SDK Fails to Install with Return Code 5100](https://support.microsoft.com/en-us/help/2717426/windows-sdk-fails-to-install-with-return-code-5100) on Microsoft Support.

Get the standalone debugging tools for Windows XP by first downloading
the Windows 7 SDK:
[Microsoft Windows SDK for Windows 7 and .NET Framework 4](https://www.microsoft.com/download/confirmation.aspx?id=8279).

To install the Debugging Tools for Windows as a standalone component,
start the SDK installer, and in the installation wizard, select
**Debugging Tools for Windows**, and clear all other components.


### Related downloads
* [Download the Windows Assessment and Deployment Kit (Windows ADK)](https://developer.microsoft.com/windows/hardware/windows-assessment-deployment-kit)
* [Download the Windows HLK, HCK, or Logo Kit](https://developer.microsoft.com/windows/hardware/windows-hardware-lab-kit)
* [Download the debugging Tools for Windows (WinDbg)](https://developer.microsoft.com/windows/hardware/download-windbg)
* [Download Windows Symbol Packages](https://developer.microsoft.com/windows/hardware/download-symbols)
* [Download the WDK Insider Preview](https://www.microsoft.com/software-download/windowsinsiderpreviewWDK)
