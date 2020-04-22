---
title: ADFS federácia certifikát končí
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710422"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS federácia certifikát končí

Ak chcete vyriešiť tento problém, postupujte nasledovne:
  
1. Nainštalovať Microsoft Azure Active Directory modul pre Windows PowerShell v počítači (Ak modul nie je už nainštalovaný). Ak to chcete urobiť, prejdite na položku [Spravovať Azure AD pomocou prostredia Windows PowerShell](https://aka.ms/aadposh).

2. Postupujte podľa krokov v "Scenár 1: AD FS token podpisu certifikátu skončila" časť ["Vyskytol sa problém s prístupom k lokalite" chyba AD FS, keď externý používateľ prihlási do Microsoft 365, Azure alebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Postupujte podľa krokov v [téme Aktualizácia alebo oprava nastavení externej domény v Microsoft, Azure alebo Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Ďalšie informácie o obnovení federácie certifikátov nájdete [obnoviť federácie certifikáty pre Microsoft 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
