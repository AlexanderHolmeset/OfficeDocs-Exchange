---
ms.localizationpriority: medium
description: "Unified Messaging (UM) mailbox policies are required when you enable users for Unified Messaging. You create UM mailbox policies to apply a common set of policies or security settings to a collection of voice mail users' mailboxes. UM mailbox policies are used to specify UM settings like the following:"
ms.topic: article
author: msdmaguire
ms.author: jhendr
ms.assetid: dfae629e-ee89-4494-a3ed-9655b67eb87e
ms.reviewer: 
f1.keywords:
- NOCSH
title: UM mailbox policies in Exchange Online
ms.collection: exchange-online
audience: ITPro
ms.service: exchange-online
manager: serdars

---

# UM mailbox policies in Exchange Online

> [!NOTE]
> Cloud Voicemail takes the place of Exchange Unified Messaging (UM) in providing voice messaging functionality for Skype for Business 2019 voice users who have mailboxes on Exchange Server 2019 or Exchange Online, and for Microsoft Teams or Skype for Business Online voice users. For more information, see [Plan Cloud Voicemail service](/skypeforbusiness/hybrid/plan-cloud-voicemail) and [Retiring Unified Messaging in Exchange Online](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/Retiring-Unified-Messaging-in-Exchange-Online/ba-p/608991).

Unified Messaging (UM) mailbox policies are required when you enable users for Unified Messaging. You create UM mailbox policies to apply a common set of policies or security settings to a collection of voice mail users' mailboxes. UM mailbox policies are used to specify UM settings like the following:

- PIN policies

- Dialing restrictions

- Other general UM mailbox policy properties

For example, you can create a UM mailbox policy to increase the level of PIN security by reducing the maximum number of sign-in failures for a specific group of UM-enabled users, such as executives.

## UM mailbox policies

At least one UM mailbox policy must have been created before you can enable users for Unified Messaging. You can create additional UM mailbox policies to apply a common set of settings for groups of users.

You create UM mailbox policies by using Exchange Online PowerShell or the Exchange admin center (EAC). By default, a single UM mailbox policy is created every time you create a UM dial plan. The new UM mailbox policy is automatically associated with the UM dial plan, and part of the dial plan name is included in the display name of the UM mailbox policy. You can edit this default UM mailbox policy.

Multiple UM-enabled users can be linked to a single UM mailbox policy. However, the mailbox for each UM-enabled user must be linked to a single UM mailbox policy. This lets you control PIN security settings such as the minimum number of digits in a PIN or the maximum number of sign-in attempts for the UM-enabled users who are associated with the UM mailbox policy. You can also control message text settings or dialing restrictions for the same UM-enabled mailboxes.
