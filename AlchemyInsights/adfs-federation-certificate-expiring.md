---
title: ADFS federácia certifikát končí
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
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737204"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="46cca-102">ADFS federácia certifikát končí</span><span class="sxs-lookup"><span data-stu-id="46cca-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="46cca-103">Ak chcete vyriešiť tento problém, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="46cca-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="46cca-104">Nainštalovať Microsoft Azure Active Directory modul pre Windows PowerShell v počítači (Ak modul nie je už nainštalovaný).</span><span class="sxs-lookup"><span data-stu-id="46cca-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="46cca-105">Ak to chcete urobiť, prejdite na položku [Spravovať Azure AD pomocou prostredia Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="46cca-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="46cca-106">Postupujte podľa krokov v "Scenár 1: AD FS token podpisu certifikátu skončila" časť ["Vyskytol sa problém s prístupom k lokalite" chyba AD FS, keď externý používateľ prihlási do balíka Office 365, Azure alebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="46cca-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="46cca-107">Postupujte podľa krokov v časti [Aktualizácia alebo oprava nastavení externej domény v balíku Office 365, Azure alebo Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="46cca-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="46cca-108">Ďalšie informácie o obnovení federácie certifikátov nájdete [obnoviť federácie certifikáty pre balík Office 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="46cca-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
