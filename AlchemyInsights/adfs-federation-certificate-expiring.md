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
# <a name="adfs-federation-certificate-expiring"></a>ADFS federácia certifikát uplynie

Ak chcete vyriešiť tento problém, postupujte nasledovne:
  
1. Nainštalovať Microsoft Azure Active Directory modul pre Windows PowerShell na počítači (Ak modul nie je už nainštalovaný). Chcete urobiť, prejdite na [Správa Azure AD pomocou prostredia Windows PowerShell](https://aka.ms/aadposh).

2. Postupujte podľa "Scenár 1: AD FS tokenu podpisovanie certifikátu skončila" časti ["Tam bol problém s prístupom k lokalite" chyba z AD FS pri združenej používateľ prihlasuje do Office 365, Azure, alebo Windows Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Postupujte podľa pokynov [ako aktualizovať alebo opraviť nastavenia združenú doménu v Office 365, Azure, alebo Windows Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Ďalšie informácie o obnovení federácie certifikáty, pozrite [obnoviť federácie certifikáty pre Office 365 a Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
