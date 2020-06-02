---
title: Riešenie problémov s odmietnutým hlásením prístupu
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505394"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Riešenie problémov s odmietnutým správam prístupu v Centre spravovania služby SharePoint alebo OneDrive

Ak pri pokuse o prehľadávanie Centra spravovania služby Sharepoint/OneDrive sa zobrazí hlásenie o odmietnutí prístupu, uistite sa, že [používateľovi priradíte licenciu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ak má používateľ licenciu, mali by ste sa tiež uistiť, že im bude [priradená rola správcu,](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) ktorá má prístup k centrám spravovania.

Tento problém sa môže vyskytnúť aj pri odstránení používateľa a znova vytvorené s rovnakým hlavným menom používateľa (UPN). Nové konto sa vytvorí pomocou inej hodnoty PUID (Passport Unique ID). Keď sa používateľ pokúsi získať prístup k kolekcii lokalít alebo onedrive, používateľ má nesprávne PUID. Druhý scenár zahŕňa synchronizáciu adresárov s organizačnou jednotkou služby Active Directory (OU). Ak sa používatelia už prihlásili do služby SharePoint a potom sa premiestnia do inej ou a znova synchronizujú so službou SharePoint, môžu sa vyskytnúť tento problém.

Ak chcete vyriešiť tento problém, mali by ste obnoviť pôvodné UPN s krokmi v článku [Obnoviť používateľa v Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Poznámka: Ak OneDrive alebo SharePoint Admin Center nie je k dispozícii pre viacerých používateľov, ktorí predtým mali prístup, môže ísť o dočasný problém služby.  [Skontrolujte tabuľu stavu služby](https://portal.office.com/adminportal/home#/servicehealth).


