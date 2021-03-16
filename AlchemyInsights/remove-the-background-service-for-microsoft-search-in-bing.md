---
title: Odstránenie služby na pozadí pre Microsoft Search v službe Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816337"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Odstránenie služby na pozadí pre Microsoft Search v službe Bing

Ak chcete odstrániť službu na pozadí pre Microsoft Search v službe Bing, môžete vyskúšať tieto opravné prostriedky:

1. Ak sa chcete vrátiť k pôvodnému nastaveniu vyhľadávacieho nástroja, vykonajte tieto kroky:

    a. Prepnutie na prepínač **použiť Bing ako predvolený vyhľadávací [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) nástroj je vypnutý**.

    b. [Prejdite do centra spravovania služieb Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) a zrušte začiarknutie nastavenia, ktoré ovplyvní všetkých používateľov vo vašej organizácii.

2. Ak chcete odstrániť službu na pozadí z jedného zariadenia, vykonajte tieto úlohy:

    a. Vyberte položku **Ovládací Panel > programy > programy a súčasti**.

    b. Kliknite pravým tlačidlom myši na položku **Microsoft Search v Bingu** v zozname nainštalovaných programov a potom kliknite na položku **odinštalovať**.

3. Ak chcete odstrániť službu na pozadí z viacerých zariadení vo vašej organizácii, prihláste sa ako správca a v skripte spustite nasledujúci príkaz: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
