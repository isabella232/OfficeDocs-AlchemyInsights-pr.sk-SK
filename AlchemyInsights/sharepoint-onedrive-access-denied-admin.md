---
title: Riešenie problémov so správami prístup odmietnutý
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760355"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Riešenie problémov s prístup odmietnutý správy služby Sharepoint/OneDrive Admin Center

Ak dostávate prístup odmietnutý správu pri pokuse vyhľadajte centrum správy služby Sharepoint/OneDrive, prosím uistite sa, že [Priradenie licencie k používateľovi](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ak používateľ nemá licenciu, tiež uistite, sú [priradenú rolu správcu](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , ktorá prístup admin centier.

Tento problém sa môže vyskytnúť aj pri používateľa sa odstráni a znova vytvorí s rovnaké hlavné meno používateľa (UPN). Nové konto je vytvorený pomocou rôznych PUID služby (Passport jedinečný identifikátor) hodnotu. Keď sa používateľ pokúsi prístup kolekcie lokalít alebo ich OneDrive, používateľ má nesprávny PUID služby. Druhý scenár zahŕňa adresár synchronizácia so Active Directory organizačnú jednotku (OU). Ak používatelia už prihlásený do služby SharePoint, a potom sa presunie na rôznych OU a resynced so službou SharePoint, tento problém sa môže vyskytnúť.

Ak chcete vyriešiť tento problém, mali obnoviť pôvodný UPN s kroky v tomto článku, [obnovení používateľa v balíku Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Poznámka: Ak OneDrive alebo SharePoint Admin center nie je k dispozícii pre viacerých používateľov, ktorí predtým prístup, môže byť problém pri dočasnej služby.  [Kontrola tabuľa stav služby](https://portal.office.com/adminportal/home#/servicehealth).


