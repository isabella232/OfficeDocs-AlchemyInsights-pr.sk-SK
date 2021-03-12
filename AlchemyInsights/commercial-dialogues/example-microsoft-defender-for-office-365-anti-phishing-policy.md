---
title: Príklad Microsoft Defendera pre Office 365 anti-phishing Policy
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750796"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Príklad Microsoft Defendera pre Office 365 anti-phishing Policy

Tieto nastavenia umožňujú politiku s názvom *domain and CEO*. Táto politika poskytuje ochranu používateľov aj domény pred zosobnením a potom použije politiku na všetky e-maily prijaté používateľmi v rámci domény. Najprv pridajte nasledujúce informácie na vytvorenie politiky:

- **Názov**: Domain and CEO **Popis**: zabezpečuje, že generálny riaditeľ a vaša doména nie sú zosobnené.
  **Použiť na**: vyberte **doménu príjemcu**. V časti **niektoré z týchto** vyberte položku **vybrať** a potom vyberte doménu. Vyberte položku **+ Pridať**. Začiarknite políčko vedľa názvu domény v zozname (napríklad *contoso.com*) a potom vyberte položku **Pridať**. Vyberte položku **Hotovo**.
- Po vytvorení politiky môžete politiku jemne doladiť pomocou nasledujúcich možností:
  - **Pridanie používateľov na ochranu:** V tomto príklade pridajte e-mailovú adresu CEO na minimum.
  - **Pridanie domén na ochranu**: Pridajte organizačnú doménu, ktorá obsahuje kanceláriu generálneho riaditeľa.
  - **Vyberte položku akcie**: v **prípade odoslania e-mailu prostredníctvom zosobneného používateľa** vyberte položku **presmerovať správu na inú e-mailovú adresu** a potom zadajte e-mailovú adresu správcu zabezpečenia (napríklad *securityadmin@contoso.com*). **Ak je e-mail odoslaný** vybratou doménou, vyberte položku **karanténa správy**.
  - **Poštová schránka inteligencia**: Táto možnosť je predvolene vybratá pri vytváraní novej politiky ochrany pred neoprávneným získavaním údajov. Ak chcete najlepšie výsledky, nechajte toto nastavenie **zapnuté** .
  - **Pridanie dôveryhodných odosielateľov a domén:** V tomto príklade nedefinujte žiadne prepíše.
- Po skontrolovaní nastavení vyberte v prípade potreby položku **vytvoriť túto politiku** alebo **Uložiť**.

Ďalšie informácie nájdete v téme [politiky ochrany pred neoprávneným získavaním údajov v Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
