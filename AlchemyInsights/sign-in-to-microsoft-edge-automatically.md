---
title: Automatické prihlásenie do Microsoft Edgeu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398744"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="933c9-102">Automatické prihlásenie do Microsoft Edgeu</span><span class="sxs-lookup"><span data-stu-id="933c9-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="933c9-103">Microsoft Edge používa predvolené konto operačného systému na automatické prihlásenie používateľa v závislosti od konfigurácie zariadenia používateľa.</span><span class="sxs-lookup"><span data-stu-id="933c9-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="933c9-104">Scenáre každého typu konfigurácie zariadenia a jeho závislého procesu prihlasovania používateľom sú popísané nižšie:</span><span class="sxs-lookup"><span data-stu-id="933c9-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="933c9-105">**Zariadenie je hybridné a AAD-J:** Táto možnosť je k dispozícii vo Windowse 10, systému Windows na úrovni nadol a v príslušných serverových verziách.</span><span class="sxs-lookup"><span data-stu-id="933c9-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="933c9-106">Používatelia sú automaticky prihlásení pomocou svojich kont v službe Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="933c9-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="933c9-107">**Zariadenie je pripojené k doméne:** Táto možnosť je k dispozícii vo Windowse 10, v down-level Windowse a v príslušných serverových verziách.</span><span class="sxs-lookup"><span data-stu-id="933c9-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="933c9-108">V predvolenom nastavení nie sú používatelia s kontami domény prihlásení automaticky. ak chcete zapnúť automatické prihlásenie pre nich, použite **politiku ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="933c9-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="933c9-109">Ak chcete povoliť automatické prihlásenie pre používateľov s kontami Azure AD, zvážte hybridné pripojenie k zariadeniam.</span><span class="sxs-lookup"><span data-stu-id="933c9-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="933c9-110">Predvolené konto operačného systému je **konto Microsoft:** Táto možnosť je k dispozícii vo Windowse 10 RS3 (verzia 1709, zostava 10.0.16299) a novších verziách.</span><span class="sxs-lookup"><span data-stu-id="933c9-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="933c9-111">Scenár sa pravdepodobne vyskytuje v podnikových zariadeniach.</span><span class="sxs-lookup"><span data-stu-id="933c9-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="933c9-112">Ak je však predvoleným kontom operačného systému konto Microsoft, Microsoft Edge sa automaticky prihlási používateľa s kontom Microsoft.</span><span class="sxs-lookup"><span data-stu-id="933c9-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
