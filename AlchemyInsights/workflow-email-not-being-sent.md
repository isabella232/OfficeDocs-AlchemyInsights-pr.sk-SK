---
title: Odoslanie e-mailu v pracovnom postupe
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749004"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>E-mail pracovného postupu sa neodosiela v zozname alebo knižnici SharePointu

1. E-maily z pracovných postupov sa neodosielajú všetkým používateľom ani iba konkrétnym používateľom alebo sa zobrazí chyba, **že sa e-mailová správa nedá odoslať. Skontrolujte, či má e-mail platný príjemca**.

    Skontrolujte, či sa používateľ nachádza v skupine **všetci používatelia** (zoznam informácií o používateľoch) pre danú kolekciu lokalít.  Ukážka priameho URL adresy: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0

    - Ak používateľ neexistuje, skontrolujte, či je používateľ prihlásený na stránku. 
    - Ak ide o externého používateľa, skontrolujte, či bola pozvánka prijatá.
    - Ak používateľ v skupine povolenia existuje, skontrolujte, či je e-mailová adresa správna.
    - Ak tu nie je nastavená e-mailová adresa používateľov, potom vytvorte vzorové Upozornenie pre daného používateľa, ktoré vynúti synchronizáciu daného používateľského konta z používateľských profilov SharePointu do tejto kolekcie lokalít.
 
2. E-maily z pracovných postupov sa odosielajú správcom kolekcie lokalít, ale nie ostatným používateľom a zobrazí sa chyba **http Forbidden to <span>https:</span>//URL/_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.
 

    Pozrite si tému [prístup odmietnutý pri odoslaní e-mailu do skupiny SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Skontrolujte tiež, či nie je aktívna funkcia **obmedzeného prístupu používateľa na uzamknutie režimu uzamknutia** lokality.


## <a name="related-topics"></a>Súvisiace témy
Chcete vyskúšať Microsoft flow v SharePointe Online?
- [Vytvorenie toku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint a tok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


