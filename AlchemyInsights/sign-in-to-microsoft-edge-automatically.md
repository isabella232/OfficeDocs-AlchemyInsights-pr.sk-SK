---
title: Automaticky sa prihláste do prehliadača Microsoft Edge
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
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678815"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="3d528-102">Automaticky sa prihláste do prehliadača Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="3d528-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="3d528-103">Microsoft Edge používa predvolené konto operačného systému na automatické prihlásenie používateľa podľa toho, ako je zariadenie používateľa nakonfigurované.</span><span class="sxs-lookup"><span data-stu-id="3d528-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="3d528-104">Scenáre jednotlivých typov konfigurácie zariadenia a jeho prihlasovacieho procesu závislého používateľa sú popísané nižšie:</span><span class="sxs-lookup"><span data-stu-id="3d528-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="3d528-105">**Zariadenie je hybridné/AAD-J**: Táto možnosť je k dispozícii vo Windowse 10, Windowse nadol a v zodpovedajúcich verziách servera.</span><span class="sxs-lookup"><span data-stu-id="3d528-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="3d528-106">Používatelia sú automaticky prihlásení pomocou svojich kont služby Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="3d528-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="3d528-107">**Zariadenie je pripojené k doméne**: Táto možnosť je k dispozícii vo Windowse 10, systéme Windowse na úrovni nižšie a v zodpovedajúcich verziách servera.</span><span class="sxs-lookup"><span data-stu-id="3d528-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="3d528-108">Používatelia s kontom domény sa predvolene nepodpisujú automaticky. Ak chcete povoliť automatické prihlasovanie, použite politiku **ConfigureOnPremisesAccountAutoSignIn** .</span><span class="sxs-lookup"><span data-stu-id="3d528-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="3d528-109">Ak chcete povoliť automatické prihlasovanie pre používateľov s kontom Azure AD, zvážte hybridné pripojenie k svojim zariadeniam.</span><span class="sxs-lookup"><span data-stu-id="3d528-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="3d528-110">**Predvoleným kontom operačného systému je konto Microsoft**: Táto možnosť je k dispozícii vo Windowse 10 RS3 (verzia 1709, Zostava 10.0.16299) a v novších verziách.</span><span class="sxs-lookup"><span data-stu-id="3d528-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="3d528-111">V podnikových zariadeniach nie je pravdepodobné, že sa vyskytne scenár.</span><span class="sxs-lookup"><span data-stu-id="3d528-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="3d528-112">Ak je však predvoleným kontom operačného systému konto Microsoft, Microsoft Edge sa automaticky prihlási používateľovi s kontom Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3d528-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
