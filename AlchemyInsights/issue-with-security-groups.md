---
title: Problém so skupinami zabezpečenia
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177632"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="47fc7-102">Problém so skupinami zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="47fc7-102">Issue with security groups</span></span>

<span data-ttu-id="47fc7-103">**Ak dostávate AADDS104 chyby siete**</span><span class="sxs-lookup"><span data-stu-id="47fc7-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="47fc7-104">Neplatné pravidlá skupiny zabezpečenia siete sú najčastejšou príčinou chýb siete pre doménové služby Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="47fc7-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="47fc7-105">Skupina zabezpečenia siete pre virtuálnu sieť musí umožniť prístup k konkrétnym portom a protokolom.</span><span class="sxs-lookup"><span data-stu-id="47fc7-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="47fc7-106">Ak sú tieto porty blokované, platforma Azure nedokáže monitorovať alebo aktualizovať spravovanú doménu.</span><span class="sxs-lookup"><span data-stu-id="47fc7-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="47fc7-107">Synchronizácia medzi službou Azure AD a službou Azure AD DS je tiež ovplyvnená.</span><span class="sxs-lookup"><span data-stu-id="47fc7-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="47fc7-108">Zabezpečte, aby boli predvolené porty otvorené, aby sa zabránilo prerušeniu prevádzky.</span><span class="sxs-lookup"><span data-stu-id="47fc7-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="47fc7-109">Ak chcete porozumieť a vyriešiť bežné upozornenia na problémy s konfiguráciou skupiny zabezpečenia siete, pozrite si tému [Pridanie a overenie skupín zabezpečenia](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="47fc7-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
