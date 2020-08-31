---
title: Používanie webovej lokality Wix s zakúpenými alebo spravovanými doménami balíka Office 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300736"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>Používanie webovej lokality Wix s zakúpenými alebo spravovanými doménami balíka Office 365

- [Aktualizujte DNS záznamy, aby ste mali webovú lokalitu so súčasným poskytovateľom hostiteľských služieb.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- WIX článok "pripojenie domény k Wix pomocou ukazovacieho postupu" odporúča sa použiť polohovacie (Pridanie DNS záznamov na vyššie uvedené prepojenie) namiesto zmeny názvových serverov pri používaní balíka Office 365
- Ak sa stále rozhodnete zmeniť názvové servery na Wix, budete musieť  [vytvoriť DNS záznamy na lokalite Wix pre Microsoft](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- Ak ste si doménu zakúpili od spoločnosti Microsoft, názvové servery nie je možné zmeniť. Ak potrebujete zmeniť názvy serverov, zakúpená doména spoločnosti Microsoft bude musieť byť [prevedená na iného poskytovateľa hostiteľských služieb po 60 dňoch](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host) .