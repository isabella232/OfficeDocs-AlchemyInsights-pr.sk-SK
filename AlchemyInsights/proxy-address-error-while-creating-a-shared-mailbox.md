---
title: Chyba proxy adresy pri vytváraní zdieľanej poštovej schránky
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
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062923"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Chyba adresy servera proxy pri vytváraní poštovej schránky alebo iného objektu s povolenou e-mailovou schránkou

Ak ste sa pokúsili vytvoriť objekt s podporou e-mailu (poštová schránka, zdieľaná poštová schránka atď.) a vyskytla sa chyba "Adresa servera proxy SMTP:alias@domain.com sa už používa...", e-mailová adresa, ktorú ste vybrali, sa už vo vašej organizácii nachádza v inom objekte s e-mailovou schránkou.
  
Je potrebné vyhľadať používateľa, skupinu, zdieľanú poštovú schránku alebo verejný priečinok s touto e-mailovou adresou a odstrániť alebo zmeniť jeho e-mailovú adresu. Potom môžete vytvoriť nový objekt s podporou e-mailu s bezplatnou e-mailovou adresou. Vyhľadajte ju pomocou funkcie vyhľadávania na domovskej stránke. Ak ho chcete vyhľadať, môžete Exchange Online pomocou nasledujúceho príkazu v prostredí PowerShell:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Ak nechcete odstrániť existujúcu e-mailovú adresu, vyberte novú e-mailovú adresu pre nový objekt, ktorý vytvárate.
  