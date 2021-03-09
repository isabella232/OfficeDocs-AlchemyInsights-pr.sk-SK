---
title: Chyba adresy proxy pri vytváraní zdieľanej poštovej schránky
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568305"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Chyba adresy servera proxy pri vytváraní poštovej schránky alebo iného objektu s povoleným e-mailom

Ak ste sa pokúsili vytvoriť objekt s podporou e-mailu (poštová schránka, zdieľaná poštová schránka atď.) a zobrazilo sa chybové hlásenie "adresa proxy" SMTP:alias@domain.com "sa už používa...", vybratá e-mailová adresa je už v organizácii prijatá iným objektom s podporou e-mailu.
  
Potrebujete nájsť používateľa, skupinu, zdieľanú poštovú schránku alebo verejný priečinok, ktorý má túto e-mailovú adresu, a odstrániť ho alebo zmeniť jeho e-mailovú adresu. Potom môžete vytvoriť nový objekt s podporou e-mailu s uvoľnenou e-mailovou adresou. Pomocou vyhľadávania na domovskej stránke ho vyhľadajte. Na jeho vyhľadanie môžete použiť aj tento príkaz prostredia Exchange Online PowerShell:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ak nechcete odstrániť existujúcu e-mailovú adresu, vyberte novú e-mailovú adresu pre nový objekt, ktorý vytvárate.
  