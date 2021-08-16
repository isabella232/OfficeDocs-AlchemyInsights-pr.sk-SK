---
title: Príklad programu Microsoft Defender pre Office 365 politiky ochrany pred neoprávneným získavaním údajov
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035021"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Príklad programu Microsoft Defender pre Office 365 politiky ochrany pred neoprávneným získavaním údajov

Tieto nastavenia povolia politiku s názvom Doména a *generálny riaditeľ.* Táto politika poskytuje ochranu používateľa aj domény pred zosobneením a potom použije politiku na všetky e-maily prijaté používateľmi v rámci domény. Najprv pridajte tieto informácie na vytvorenie politiky:

- **Názov:** Popis domény a **riaditeľa:** Zabezpečuje, že výkonný riaditeľ a vaša doména nie sú zosobňovaní.
  **Použité na:** Vyberte **položku Doména príjemcu je**. V **časti Ktorýkoľvek z** týchto vyberte položku **Vybrať** a potom vyberte doménu. Vyberte **položku + Pridať**. Začiarknite políčko vedľa názvu domény v zozname (napríklad Názov contoso.com *)* a potom vyberte položku **Pridať**. Vyberte položku **Hotovo**.
- Po vytvorení politiky môžete politiku doladiť pomocou týchto možností:
  - **Pridanie používateľov na ochranu:** V tomto príklade pridajte minimálne e-mailovú adresu riaditeľa.
  - **Pridanie domén na ochranu:** Pridajte doménu organizácie, ktorá obsahuje kanceláriu riaditeľa.
  - **Výber akcií:** **Ak** e-mail odošle zosobnený používateľ , vyberte položku Presmerovať správu na inú e-mailovú adresu a potom zadajte e-mailovú adresu správcu zabezpečenia *(napríklad securityadmin@contoso.com*). Pre **položku Ak e-mail odosiela zosobnená doména**, vyberte položku **Umiestniť správu do karantény**.
  - **Inteligencia poštovej** schránky: Táto možnosť je predvolene vybratá pri vytváraní novej politiky ochrany proti neoprávnenému získavaniu údajov. Ak chcete dosiahnuť najlepšie **výsledky,** ponechajte toto nastavenie aktívne.
  - **Pridanie dôveryhodných odosielateľov a domén:** V tomto príklade nezadefinujte žiadne prepisy.
- Po revízii nastavení vyberte podľa potreby položku **Vytvoriť túto politiku** alebo Uložiť. 

Ďalšie informácie nájdete v téme Politiky [ochrany pred neoprávneným získavaním údajov v Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
