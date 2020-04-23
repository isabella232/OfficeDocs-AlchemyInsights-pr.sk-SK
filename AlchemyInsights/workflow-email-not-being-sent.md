---
title: E-mail pracovného postupu sa neodosiela
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766148"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail pracovného postupu sa neodosiela pre zoznam alebo knižnicu lokality SharePoint

1. E-maily z pracovných postupov sa neodosielajú všetkým používateľom alebo len konkrétnym používateľom, alebo sa zobrazí chyba, **e-mailová správa sa nedá odoslať. Uistite sa, že e-mail má platného príjemcu**.

    Skontrolujte, či používateľ existuje v skupine **všetky osoby** povolenia (zoznam informácií o používateľovi) pre túto kolekciu lokalít.  Ukážka priamej adresy URL:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/People.aspx? MembershipGroupId = 0

    - Ak používateľ neexistuje, uistite sa, že používateľ je prihlásený na stránku. 
    - Ak ide o externého používateľa, uistite sa, že ich pozvánka bola prijatá.
    - Ak používateľ existuje v skupine povolenia, uistite sa, že e-mailová adresa je správna.
    - Ak e-mailová adresa používateľov nie je nastavená tu, potom vytvorte ukážkovú výstrahu pre daného používateľa, ktorá vynúti synchronizáciu daného používateľského konta z používateľských profilov lokality SharePoint do tejto kolekcie lokalít.
 
2. E-maily z pracovných postupov sa odosielajú správcom kolekcie lokalít, ale nie ostatným používateľom a zobrazí sa chyba **http zakázané <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.
 

    Pozrite si [prístup odmietnutý pri odosielaní e-mailu do skupiny SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Tiež overiť, že **obmedzený prístup používateľa povolenie Lockdown režime** kolekcie lokalít funkcia nie je aktívna.


## <a name="related-topics"></a>Súvisiace témy
Chcete vyskúšať službu Microsoft flow v SharePointe Online?
- [Vytvoriť tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


