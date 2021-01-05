---
title: Postup pridávania a spravovania správcov – Odporúčané kroky
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755850"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Postup pridávania a spravovania správcov – Odporúčané kroky

Na základe popisu problému sme našli riešenie. Väčšina zákazníkov si po vykonaní našej dokumentácie dokázala vyriešiť svoj problém sami.

**Úprava správcu predplatného alebo spolusprávcu**

- Správca konta môže upraviť obe roly, zatiaľ čo správca predplatného môže zmeniť iba správcov na [portáli Azure](https://ms.portal.azure.com/#home).
- [Pridanie alebo zmena správcov predplatného Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Aktualizácia správcu predplatného alebo Co-Administrator pre interné (VYSIELAné) predplatné**

Správca služieb alebo spolusprávca môže túto akciu samostatne podávať pomocou týchto krokov:

1. Prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) a kliknite na položku **Správa nákladov + Fakturácia** v ľavom kotúči.
2. Kliknite na položku riadok s predplatným. Otvorí sa vám prehľad predplatného.
3. Na ostrie **predplatného** kliknite na položku **Vlastnosti**. 
4. Kliknite na tlačidlo **Správca služby** .
5. Zadajte e-mailovú adresu používateľa, ktorého chcete nastaviť ako správcu služby, a kliknite na tlačidlo **OK**.

**Pridanie alebo zmena alebo odstránenie spolusprávcu**

1. Prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) ako správca služieb.
2. Otvorte [predplatné](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) a vyberte predplatné. (Co-Adminstrators môže byť priradená iba v rozsahu predplatného.)
3. Prechod na **Ovládací prvok Access Control (IAM)**  >  **Classic správcovia**  >  **Pridať**  >  **Pridať spolusprávcu** na otvorenie tably **Pridať** spolusprávcu (ak je možnosť pridať spolusprávcu vypnutá, znamená to, že nemáte povolenia).
4. Vyberte používateľa, ktorého chcete pridať, a kliknite na položku **Pridať**.

**zistiť viac:**
- [Pridanie spolusprávcu](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Odstránenie spolusprávcu](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Zmena správcu služby](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Zobrazenie správcu konta](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Správa prístupu pomocou RBAC a Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Pridanie alebo odstránenie používateľov pomocou služby Azure Active Directory (AD)**

Môžete pridať nových používateľov alebo odstrániť existujúcich používateľov zo služby Azure Active Directory (Azure AD) organizácie:

1. Ak chcete pridať nového používateľa, prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) ako používateľ – správca organizácie.
2. Vyberte položku **Azure Active Directory**, vyberte položku **Používatelia** a potom kliknite na položku **Nový používateľ**.
3. Na stránke **používateľ** Vyplňte požadované informácie. Kliknite na položku **vytvoriť**. Používateľ sa vytvorí a pridá do nájomníka služby Azure AD.

Ďalšie **informácie**:

- [Pridanie nového používateľa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Odstránenie používateľa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Pridanie alebo aktualizácia informácií o profile používateľa pomocou služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Odporúčané dokumenty**

- [Čo je riadenie prístupu na základe rolí (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Porozumieť rôznym funkciám v službe Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Povolenia roly správcu v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Kurz: udelenie prístupu používateľovi pomocou RBAC a portálu Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Riešenie problémov s RBAC v službe Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Usporiadanie zdrojov pomocou skupín spravovania služby Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Ako požiadať o kópiu Azure faktúry prostredníctvom e-mailu](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Pridanie, aktualizácia alebo odstránenie kreditnej alebo debetnej karty zo služby Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Spravovanie (Opätovná aktivácia/zrušenie/zmena) predplatného](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



