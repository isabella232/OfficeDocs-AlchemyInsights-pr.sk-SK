---
title: ADFS federácia certifikát uplynie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: b014e350d5f6f1a61feb223e3d3fd0a1f56f5872
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357980"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="1dc17-102">ADFS federácia certifikát uplynie</span><span class="sxs-lookup"><span data-stu-id="1dc17-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="1dc17-103">Ak chcete vyriešiť tento problém, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="1dc17-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="1dc17-104">Nainštalovať Microsoft Azure Active Directory modul pre Windows PowerShell na počítači (Ak modul nie je už nainštalovaný).</span><span class="sxs-lookup"><span data-stu-id="1dc17-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="1dc17-105">Chcete urobiť, prejdite na [Správa Azure AD pomocou prostredia Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="1dc17-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="1dc17-106">Postupujte podľa "Scenár 1: AD FS tokenu podpisovanie certifikátu skončila" časti ["Tam bol problém s prístupom k lokalite" chyba z AD FS pri združenej používateľ prihlasuje do Office 365, Azure, alebo Windows Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="1dc17-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="1dc17-107">Postupujte podľa pokynov [ako aktualizovať alebo opraviť nastavenia združenú doménu v Office 365, Azure, alebo Windows Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="1dc17-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="1dc17-108">Ďalšie informácie o obnovení federácie certifikáty, pozrite [obnoviť federácie certifikáty pre Office 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="1dc17-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
