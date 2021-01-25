---
title: Problém s poskytnutím SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949947"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="b3cad-102">Problém s poskytnutím SCIM</span><span class="sxs-lookup"><span data-stu-id="b3cad-102">SCIM provisioning issue</span></span>

<span data-ttu-id="b3cad-103">Automatické poskytovanie odkazuje na vytváranie identít používateľov a rolí v cloudových aplikáciách, ku ktorým používatelia potrebujú prístup.</span><span class="sxs-lookup"><span data-stu-id="b3cad-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="b3cad-104">Okrem vytvárania totožností používateľov obsahuje automatické poskytovanie aj údržbu a odstránenie totožností používateľa ako zmeny stavu alebo rolí.</span><span class="sxs-lookup"><span data-stu-id="b3cad-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="b3cad-105">Skôr než začnete s nasadením, môžete si pozrieť, [ako funguje poskytovanie](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) informácií o tom, ako funguje poskytovanie služieb Azure Active Directory (AD), a získať odporúčania na konfiguráciu.</span><span class="sxs-lookup"><span data-stu-id="b3cad-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="b3cad-106">Ako vývojár aplikácie môžete použiť systém pre rozhranie API na správu identít medzi doménami (SCIM) na umožnenie automatického zriaďovania používateľov a skupín medzi aplikáciou a službou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b3cad-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="b3cad-107">[Koncové body na vytvorenie koncového bodu scim a konfigurovanie poskytovania používateľov pomocou článku Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) popisuje, ako vytvoriť koncový bod scim a integrovať ho so službou Azure AD poskytovanie služby.</span><span class="sxs-lookup"><span data-stu-id="b3cad-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



