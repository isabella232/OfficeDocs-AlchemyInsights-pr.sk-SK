---
title: Riešenie bežných problémov s formátovaním záznamov DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525646"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="d7293-102">Riešenie bežných problémov s formátovaním záznamov DKIM</span><span class="sxs-lookup"><span data-stu-id="d7293-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="d7293-103">Väčšinu problémov s nastavením DKIM súvisia s nesprávnymi záznamami DNS.</span><span class="sxs-lookup"><span data-stu-id="d7293-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="d7293-104">Ak chcete vyriešiť problémy s nastavením DKIM, overte, či je záznam CNAME CNAME (**nie** txt záznam) naformátovaný správne.</span><span class="sxs-lookup"><span data-stu-id="d7293-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="d7293-105">Ďalšie informácie nájdete v téme [čo je potrebné urobiť na manuálne nastavenie funkcie dkim v Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="d7293-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="d7293-106">Ak potrebujete pomoc so záznamami DNS všeobecne, pozrite si tému [Vytvorenie záznamov DNS u ktoréhokoľvek poskytovateľa hostiteľských služieb DNS pre Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="d7293-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="d7293-107">Po vytvorení alebo aktualizácii DNS záznamov v hostiteľskej službe DNS pre svoju doménu budete musieť počkať na propagáciu DNS záznamov.</span><span class="sxs-lookup"><span data-stu-id="d7293-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
