---
title: Podmienený prístup s Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c24451fba8b8ab8fe7a1778bb292dec6678e1ef487076d27458c9aeb4963c683
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069727"
---
# <a name="conditional-access-with-intune"></a>Podmienený prístup s Intune

Používanie  **podmieneného prístupu so**  služby Intune vyžaduje 3 kroky:

- Vytvorte **politiku dodržiavania súladu** [(Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) na definovanie nastavení, ktoré musia byť splnené skôr, ako sa zariadenie považuje za spĺňajúce súlad. Príklad: Zariadenie musí mať aspoň 6-číselný PIN kód, aby sa zariadenie považovalo za spĺňajúce súlad.
- Vytvorenie politiky **podmieneného prístupu určujúci,**  aké zdroje sú chránené a aké podmienky musia byť splnené na získanie prístupu k týmto zdrojom.  [Príklad: Zariadenie musí](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  pred prístupom k podnikovým e-mailom spĺňať súlad.
- Skontrolujte, **či sú politiky dodržiavania**  súladu  **aj**  politiky podmieneného prístupu zamerané na požadované skupiny používateľov. Môže to vyžadovať vytvorenie konkrétnych skupín používateľov v Azure Active Directory.

**Užitočné prepojenia:**

[Prehľad súladu zariadení](https://docs.microsoft.com/intune/device-compliance-get-started)

[Riešenie problémov s certifikačnou autoritou](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Politika riešenia problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

Ak chcete zabezpečiť e-mail (Exchange online) pred prístupom v nekompletných zariadeniach, je potrebné dodržať oba dokumenty:

1. [Ochrana e-mailového prístupu zo zariadení pomocou EAS](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [Chráňte prístup k e-mailu pred zariadeniami, ktoré používajú klientov moderného overovania, ako Outlook](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)