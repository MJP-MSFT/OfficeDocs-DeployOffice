---
title: "Overview of licensing and activation in Office 365 ProPlus"
ms.author: jwhit
author: jwhit-MSFT
manager: laurawi
audience: ITPro
ms.topic: get-started-article
ms.service: o365-proplus-itpro
localization_priority: Normal
ms.collection: Ent_O365
ms.custom: Ent_Office_ProPlus
description: "Explains how to assign Office 365 ProPlus licenses to users, and how individual installations are activated."
---

# Overview of licensing and activation in Office 365 ProPlus

 **Summary:** Explains how to assign Office 365 ProPlus licenses to users, and how individual installations are activated.
  
To deploy Office 365 ProPlus to users in your organization, you start by assigning licenses to your users. Then, each user can install Office 365 ProPlus on up to five computers. Each installation is activated and kept activated automatically by cloud-based services associated with Office 365. This means you don't have to keep track of product keys. It also means you don't have to figure out how to use other activation methods such as Key Management Service (KMS) or Multiple Activation Key (MAK). All you have to do is make sure you purchase enough licenses, keep your Office 365 subscription current, and make sure your users can connect to Office Licensing Service via the Internet at least once every 30 days.
  
> [!NOTE]
> The information in this article also applies to Project Online Desktop Client and Visio Online Plan 2 (previously named Visio Pro for Office 365), which are licensed separately from Office 365 ProPlus. 
  
<a name="BKMK_LicensingO365PP"> </a>
## Licensing Office 365 ProPlus

The number of available licenses available for Office 365 ProPlus depends on your organization's Office 365 subscription level. To assign a license to a user, you select a check box on the licenses page for the user's account. 
  
![Office 365 licenses](images/15b018fe-c12e-4d78-9287-bc95d5e14cac.png)
  
After that's done, the user can install Office directly from the Office 365 portal or you can deploy Office to your users from your local network. If the user hasn't been assigned a license, the user can't install Office from the Office 365 portal. 
  
You can remove a user's license (for example, if the user leaves your organization). After you do this, any installations of Office 365 ProPlus that the user had go into [reduced functionality mode](overview-of-licensing-and-activation-in-office-365-proplus.md#BKMK_ReducedFunctionalityMode). The Office Licensing Service, a part of Office 365, keeps track of which users are licensed and how many computers they've installed Office on.
  
<a name="BKMK_ActivatingO365PP"> </a>
## Activating Office 365 ProPlus

As part of the installation process, Office 365 ProPlus communicates with the Office Licensing Service and the Activation and Validation Service to obtain and activate a product key. Each day, or each time the user logs on to their computer, the computer connects to the Activation and Validation Service to verify the license status and extend the product key. As long as the computer can connect to the Internet at least once every 30 days, Office remains fully functional. If the computer goes offline for more than 30 days, Office enters [reduced functionality mode](overview-of-licensing-and-activation-in-office-365-proplus.md#BKMK_ReducedFunctionalityMode) until the next time a connection can be made. To get Office fully functional again, usually a user can simply connect to the Internet and let the Activation and Validation Service reactivate the installation.
  
> [!IMPORTANT]
> Because of its online activation features, Office 365 ProPlus won't work on computers that are completely cut off from the Internet. For those computers, we recommend installing Office Professional Plus 2019 and using a [traditional activation method](https://docs.microsoft.com/DeployOffice/vlactivation/plan-volume-activation-of-office) such as Key Management Service (KMS) or Active Directory Domain Services.
  
### Managing activated installations

Each Office 365 ProPlus license allows a user to install Office on up to five computers. The user manages installations in the Office 365 portal:
  
![Managing Office 365 active installations](images/c830ebad-a255-4e32-8d7a-af5a687dc107.png)
  
If the user decides to install Office 365 ProPlus on a sixth computer, she will need to deactivate one of the first five. Office 365 ProPlus goes into [reduced functionality mode](overview-of-licensing-and-activation-in-office-365-proplus.md#BKMK_ReducedFunctionalityMode) on the deactivated computer.
  
<a name="BKMK_ReducedFunctionalityMode"> </a>
## What is reduced functionality mode?

In reduced functionality mode, Office 365 ProPlus remains installed on the computer, but users can only view and print their documents. All features for editing or creating new documents are disabled, and the user sees a message like the following:
  
![Product deactivated](images/78aa59b0-8772-4ba2-8094-bfeb65602ab7.png)
  
The user can then choose one of the available options to reactivate Office 365 ProPlus on that computer.

If the user hasn't been assigned a license, and they try to use Office 365 ProPlus on a computer where it's installed, Office will be in reduced functionality mode. Also, the user will be prompted to sign in and activate every time they open an Office app, such as Word or Excel.
  
 ## Improvements in Office 365 ProPlus versions >1910.

We have made great improvements to how licensing and user administration is handled with Office 365 ProPlus.

For your users, here’s what stays the same:

- Sign in to activate Office: Users will continue to sign in to activate Office on their devices. When single sign-on is enabled, Office detects the user’s credentials and activates Office automatically.

- Sign-in limits: Users can sign in to activate Office on five desktops, five tablets, and five mobile devices.


Here are the changes that your users may notice:

- No more prompts to deactivate: Users can install Office on a new device without being prompted to deactivate Office on another device.

- Automatic sign out: When a user reaches the sign-in limit, instead of being prompted to deactivate, the user will be automatically signed out of Office on the device where Office has been least recently used. The next time the user starts Office on that device, the user will be prompted to sign in to activate Office.


Here are the changes that you as an admin may notice when managing devices where Office is installed:

- Improved device reallocation: Previously, users who received reallocated devices could receive an error if the previous user deactivated the device from the portal or if you removed the Office 365 license from the previous user. Going forward, users will not receive the error because the activation and deactivation is user specific.

- Improved activation reporting: Previously, when one user activated Office on a device and a second user later signed on to that device, the second activation was not displayed in the Admin Center’s Activation Reports. Going forward, both activations will be identified and displayed in the Activation Report.



## Related topics

[Licensing and activation data sent to Office 365 by Office 365 ProPlus](licensing-and-activation-data-sent-to-office-365-by-office-365-proplus.md)
  
[About Office 365 ProPlus in the enterprise](about-office-365-proplus-in-the-enterprise.md)
  
[Choose how to deploy Office 365 ProPlus](choose-how-to-deploy-office-365-proplus.md)

