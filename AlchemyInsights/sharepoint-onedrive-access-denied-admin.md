---
title: Riešenie problémov s hlásením odmietnutia prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767678"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Riešenie problémov s prístupom odmietnutých správ v centre spravovania SharePointu a OneDrivu

Ak sa pri pokuse o vyhľadanie v centre spravovania služby SharePoint/OneDrive zobrazuje hlásenie o odmietnutí prístupu, skontrolujte, či ste [používateľom priradili licenciu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ak má používateľ licenciu, mali by ste tiež uistiť, že im je [priradená rola správcu](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , ktorá môže získať prístup k centru spravovania.

Tento problém sa môže vyskytnúť aj po odstránení používateľa a opätovnom vytvorení s rovnakým hlavným menom používateľa (UPN). Nové konto sa vytvorí s použitím inej hodnoty PUID (jedinečného ID konta Passport). Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo k ich OneDrivu, má používateľ nesprávny PUID. Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU). Ak sa používatelia už prihlásili do SharePointu a potom sa prenesú do inej OU a opätovne sa synchronizujú so SharePointom, tento problém sa môže vyskytnúť.

Ak chcete tento problém vyriešiť, mali by ste obnoviť pôvodné meno používateľa podľa krokov v článku a [obnoviť používateľa v službe Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Poznámka: Ak centrum spravovania služby OneDrive alebo SharePoint nie je k dispozícii viacerým používateľom, ktorí mali predtým prístup, môže sa vyskytnúť dočasný problém so službou.  [Skontrolujte tabuľu stavu služby](https://portal.office.com/adminportal/home#/servicehealth).


