---
title: Konfigurácia a riešenie problémov s tvrdeniami SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901289"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="01a65-102">Konfigurácia a riešenie problémov s tvrdeniami SAML</span><span class="sxs-lookup"><span data-stu-id="01a65-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="01a65-103">Konfigurácia a riešenie problémov s tvrdeniami SAML:</span><span class="sxs-lookup"><span data-stu-id="01a65-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="01a65-104">Postupujte podľa krokov uvedených v [tomto článku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) a nakonfigurujte nárok na rolu vydaný v tokene SAML pre podnikové aplikácie.</span><span class="sxs-lookup"><span data-stu-id="01a65-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="01a65-105">Postupujte podľa krokov v [tomto článku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) na prispôsobenie pohľadávok vydaných v tokene SAML pre podnikové aplikácie.</span><span class="sxs-lookup"><span data-stu-id="01a65-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="01a65-106">Postupujte podľa krokov v [tomto článku](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) na prispôsobenie pohľadávok emitovaných v tokenoch pre konkrétnu aplikáciu v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="01a65-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="01a65-107">V [tomto článku](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) sa dozviete, ako pracovať s aplikáciami s vedomím pohľadávok v aplikačnom serveri proxy.</span><span class="sxs-lookup"><span data-stu-id="01a65-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>