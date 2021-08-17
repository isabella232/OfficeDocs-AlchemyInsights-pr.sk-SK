---
title: Riešenie problémov s hláseniami o odmietnutí prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085243"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Riešenie problémov s hláseniami o odmietnutí prístupu v Centre spravovania služby SharePoint OneDrive lokality

Ak sa pri pokuse o vyhľadanie Centra spravovania služby SharePoint/OneDrive zobrazí hlásenie o odmietnutí prístupu, uistite sa, že používateľovi priradíte [licenciu.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ak má používateľ licenciu, mali by ste sa uistiť, že má priradenú rolu [správcu,](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ktorá má prístup do centier spravovania.

Tento problém sa môže vyskytnúť aj pri odstránení a vytvorení používateľa s rovnakým hlavným menom používateľa (UPN). Nové konto sa vytvorí pomocou inej hodnoty PUID (Passport Unique ID). Keď sa používateľ pokúsi získať prístup ku kolekcii lokalít alebo OneDrive, používateľovi sa zobrazí nesprávna identifikácia PUID. Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory. Ak sa používatelia už prihlásili do služby SharePoint a potom sa presunú do inej poštovej schránky a znova synchronizujú s SharePoint, môže sa im zobraziť tento problém.

Ak chcete tento problém vyriešiť, je potrebné obnoviť pôvodné používateľské meno používateľa pomocou krokov uvedených v článku Obnovenie [používateľa v Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Poznámka: Ak centrum OneDrive alebo SharePoint spravovania nie je k dispozícii viacerým používateľom, ktorí predtým mali prístup, môže sa vyskytnúť dočasný problém so servisom.  [Skontrolujte tabuľu stavu služby.](https://portal.office.com/adminportal/home#/servicehealth)


