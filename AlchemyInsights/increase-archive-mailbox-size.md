---
title: 305 zväčšiť veľkosť archívnej poštovej schránky
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36661815"
---
# <a name="increase-the-archive-mailbox-size"></a>Zväčšiť veľkosť archívnej poštovej schránky

Balík Office 365 [obmedzuje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) veľkosť archívnych poštových schránok na základe licencie priradenej k používateľskému kontu. Keď archívna poštová schránka dosiahne 90% povolenej veľkosti, používateľ dostane e-mailové upozornenie. Keď archívna poštová schránka dosiahne limit veľkosti, používateľ nemôže premiestniť viac položiek do archívnej poštovej schránky. Office 365 nezvýši veľkosť archívnej poštovej schránky po dosiahnutí limitu veľkosti. Namiesto toho môžu používatelia vykonať nasledujúce akcie uvoľniť miesto v archívnej poštovej schránke:

- Exportujte položky do súboru. pst pomocou programu Outlook.

- Odstrániť položky z archívnej poštovej schránky.

Office 365 poskytuje **neobmedzenú archiváciu** pre Office 365 Enterprise E3 a E5 licencie. Správca musí povoliť túto funkciu pred archívnej poštovej schránky dosiahne maximálnu veľkosť. Ak je povolená neobmedzená archivácia, môže trvať až 30 dní, kým sa do archívnej poštovej schránky pridá voľné miesto. Preto odporúčame, aby správcovia overiť voľné miesto v archívnej poštovej schránke, ktorý umožňuje používateľovi naďalej používať archívnu poštovú schránku, kým sa rozbalí. Ďalšie informácie nájdete v téme [Prehľad neobmedzenej archivácie v balíku office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) a [umožnenie neobmedzenej archivácie v balíku Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Ďalšie informácie o prístupe k archívnej poštovej schránke z programu Outlook nájdete [v téme požiadavky programu Outlook na prístup k položkám v automatickom rozbalenom archíve](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Konfigurácia politiky uchovávania údajov, ktorá automaticky presunie položky do archívnej poštovej schránky, nájdete [v téme Nastavenie politiky archivácie a odstránenia poštových schránok v organizácii balíka Office 365](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Poznámka**: automatické rozširovanie archívov nie sú podporované pre primárne poštové schránky na serveri Exchange 2010.
