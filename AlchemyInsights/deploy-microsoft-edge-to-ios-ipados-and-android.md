---
title: Nasadenie prehliadača Microsoft Edge do systému iOS, iPadOS a Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194588"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="5a80f-102">Nasadenie prehliadača Microsoft Edge do systému iOS, iPadOS a Android</span><span class="sxs-lookup"><span data-stu-id="5a80f-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="5a80f-103">Scenár so sprievodcom, ktorý je zhrnutý nižšie, vám pomôže priradiť Microsoft Edge používateľom zariadení so systémom iOS, iPadOS a Android.</span><span class="sxs-lookup"><span data-stu-id="5a80f-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="5a80f-104">Ak ste zablokovaní používateľov zaregistrovaným v mobilných zariadeniach, tento interaktívny scenár nebude fungovať a používatelia budú musieť nainštalovať Microsoft Edge sami.</span><span class="sxs-lookup"><span data-stu-id="5a80f-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="5a80f-105">Scenár so sprievodcom zahŕňa tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="5a80f-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="5a80f-106">Predpoklady</span><span class="sxs-lookup"><span data-stu-id="5a80f-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="5a80f-107">Zavedenie</span><span class="sxs-lookup"><span data-stu-id="5a80f-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="5a80f-108">Základy</span><span class="sxs-lookup"><span data-stu-id="5a80f-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="5a80f-109">Konfigurácie</span><span class="sxs-lookup"><span data-stu-id="5a80f-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="5a80f-110">Úlohy</span><span class="sxs-lookup"><span data-stu-id="5a80f-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="5a80f-111">Revízia a vytvorenie</span><span class="sxs-lookup"><span data-stu-id="5a80f-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="5a80f-112">Po dokončení krokov v scenári so sprievodcom vám politiky služby Microsoft Intune umožnia tieto funkcie Microsoft Edge for Business:</span><span class="sxs-lookup"><span data-stu-id="5a80f-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="5a80f-113">Dvojitá identita</span><span class="sxs-lookup"><span data-stu-id="5a80f-113">Dual identity</span></span>
- <span data-ttu-id="5a80f-114">Integrácia s politikou ochrany aplikácie Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5a80f-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="5a80f-115">Integrácia so serverom proxy aplikácie služby Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5a80f-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="5a80f-116">Prepojenia spravovaných obľúbených položiek a domovských stránok</span><span class="sxs-lookup"><span data-stu-id="5a80f-116">Managed favorites and home page shortcuts</span></span>
