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
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952984"
---
# <a name="adfs-federation-certificate-expiring"></a>Uplynutie platnosti certifikátu federácie ADFS

Ak chcete tento problém vyriešiť, postupujte takto:
  
1. Nainštalujte Microsoft Azure Active Directory Module Windows PowerShell do počítača (ak modul ešte nie je nainštalovaný). Ak to chcete urobiť, prejdite do [časti Spravovanie služby Azure AD Windows PowerShell.](https://aka.ms/aadposh)

2. Postupujte podľa krokov v časti Scenár 1: Platnosť podpisového certifikátu tokenu služby ADFS uplynula v časti Vyskytol sa problém s prístupom na lokalitu zo služby AD FS, keď sa externý používateľ prihlási do služieb [Microsoft 365, Azure alebo Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Postupujte podľa krokov v [článku Aktualizácia alebo oprava nastavení federnej domény v službe Microsoft, Azure alebo Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Ďalšie informácie o obnovení certifikátov federácie nájdete v téme [Obnovenie certifikátov federácie pre Microsoft 365 a Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
