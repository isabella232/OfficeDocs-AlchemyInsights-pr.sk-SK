---
title: Riešenie problémov s podpisom certifikátu SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694449"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Riešenie problémov s podpisom certifikátu SAML

Ak chcete vyriešiť problém s podpisom certifikátu SAML, vykonajte tieto Odporúčané kroky:

1. Keď pridáte podnikovú aplikáciu, ktorá podporuje SSO, Azure vygeneruje certifikát, ktorý sa nazýva [podpisový certifikát SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications). Tento certifikát má dátum uplynutia platnosti 3 roky. Ak chcete zmeniť dátum uplynutia platnosti certifikátu, pozrite si tému [Prispôsobenie dátumu uplynutia platnosti certifikátu federácie a jeho prevrátenie do nového certifikátu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).
2. Azure použije tento certifikát na podpísanie tokenov SAML vyžiadaných aplikáciou a odoslanie žiadosti o úspešné prihlásenie do aplikácie. Ak chcete vykonať tento postup, Stiahnite si certifikát z portálu Azure a odošlite ho dodávateľovi aplikácie a dokončite proces SSO.

Po dokončení tohto procesu bude aplikácia dôverovať tomuto certifikátu a všetky tokeny SAML podpísané týmto certifikátom bude žiadosť akceptovať.

3. Ak platnosť tohto certifikátu uplynie, vytvorte nový certifikát, aktualizujte ho na dodávateľa aplikácie a potom ho aktivujte na stránke Azure. Ďalšie informácie nájdete v téme [obnovenie certifikátu, ktorý bude čoskoro uplynúť](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).

> [!NOTE]
> Ak platnosť certifikátu uplynie, používateľ nebude blokovaný.

4. [Pridajte e-mailovú adresu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , na ktorú sa majú prijímať oznámenia pred uplynutím platnosti aktuálneho certifikátu.

> [!NOTE]
> Krok 4 je voliteľný.

5. Zmeňte možnosti podpisu certifikátu SAML aplikácie a algoritmus podpisu certifikátu. Ďalšie informácie nájdete v téme [Zmena možností podpisu certifikátu a algoritmu podpisu](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).

