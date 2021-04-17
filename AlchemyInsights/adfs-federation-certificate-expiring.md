---
title: Uplynutie platnosti certifikátu federácie ADFS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821966"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="be9af-102">Uplynutie platnosti certifikátu federácie ADFS</span><span class="sxs-lookup"><span data-stu-id="be9af-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="be9af-103">Ak chcete tento problém vyriešiť, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="be9af-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="be9af-104">Do počítača nainštalujte modul Microsoft Azure Active Directory pre Windows PowerShell (ak modul ešte nie je nainštalovaný).</span><span class="sxs-lookup"><span data-stu-id="be9af-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="be9af-105">Ak to chcete urobiť, prejdite do [časti Spravovanie služby Azure AD pomocou prostredia Windows PowerShell.](https://aka.ms/aadposh)</span><span class="sxs-lookup"><span data-stu-id="be9af-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="be9af-106">Postupujte podľa krokov v časti Scenár 1: Platnosť podpisového certifikátu tokenu služby ADFS uplynula v časti Vyskytol sa problém s prístupom na lokalitu zo služby ADFS, keď sa externý používateľ prihlási do služieb [Microsoft 365, Azure alebo Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="be9af-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="be9af-107">Postupujte podľa krokov v [článku Aktualizácia alebo oprava nastavení federnej domény v službe Microsoft, Azure alebo Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)</span><span class="sxs-lookup"><span data-stu-id="be9af-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="be9af-108">Ďalšie informácie o obnovení certifikátov federácie nájdete v téme Obnovenie [certifikátov federácie pre Microsoft 365 a Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)</span><span class="sxs-lookup"><span data-stu-id="be9af-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
