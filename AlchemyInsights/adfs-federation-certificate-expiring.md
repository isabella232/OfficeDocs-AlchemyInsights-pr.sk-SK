---
title: Platnosť certifikátu ADFS federácia uplynula
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686765"
---
# <a name="adfs-federation-certificate-expiring"></a>Platnosť certifikátu ADFS federácia uplynula

Ak chcete tento problém vyriešiť, postupujte podľa týchto krokov:
  
1. Nainštalujte modul Microsoft Azure Active Directory pre Windows PowerShell v počítači (Ak modul ešte nie je nainštalovaný). Ak to chcete urobiť, prejdite na položku [Správa služby Azure AD pomocou prostredia Windows PowerShell](https://aka.ms/aadposh).

2. Postupujte podľa krokov v časti Scenár 1: platnosť certifikátu token podpisu tokenu AD FS uplynula časť ["Vyskytol sa problém s prístupom na lokalitu" z AD FS pri združenej používateľ prihlási do služby Microsoft 365, Azure alebo Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Postupujte podľa krokov v téme [Aktualizácia alebo oprava nastavení externej domény v službe Microsoft, Azure alebo Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Ďalšie informácie o obnovovaní certifikátov federácie nájdete v téme [obnovenie certifikátov federácie pre služby Microsoft 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
