---
title: E-mail pracovného postupu sa odosiela
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072535"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail pracovného postupu sa odosiela pre SharePoint alebo knižnicu

1. E-maily z pracovných postupov sa neposiela všetkým používateľom ani len konkrétnym používateľom, prípadne sa zobrazí chyba E-mailová správa sa nedá odoslať. Uistite sa, že **e-mail má platného príjemcu.**

    Skontrolujte, či používateľ existuje v **skupine povolení Všetci** ľudia (zoznam informácií o používateľovi) pre túto kolekciu lokalít.  Vzorová priama URL adresa: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Ak používateľ neexistuje, uistite sa, že je na stránku prihlásený. 
    - Ak ide o externého používateľa, uistite sa, že jeho pozvánka bola prijatá.
    - Ak používateľ existuje v skupine povolení, skontrolujte správnosť e-mailovej adresy.
    - Ak tu nie je nastavená e-mailová adresa používateľa, vytvorte pre tohto používateľa vzorové upozornenie, ktoré vynútene synchronizáciu tohto používateľského konta z používateľského SharePoint tejto kolekcie lokalít.
 
2. E-maily z pracovných postupov sa odošlú správcom kolekcie lokalít, ale nie ostatným používateľom, a zobrazí sa chyba HTTP Zakázané pre **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Pozrite [si časť Prístup odmietnutý pri odosielaní e-mailu SharePoint skupine.](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)

    Overte tiež, či nie je aktívna funkcia kolekcie lokalít **s režimom uzamknutia** s povolením obmedzeného prístupu používateľa.


## <a name="related-topics"></a>Súvisiace témy
Chcete sa o Microsoft Flow v SharePoint Online?
- [Vytvorenie Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


