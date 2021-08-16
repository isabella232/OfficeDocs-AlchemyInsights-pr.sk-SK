---
title: Odstránenie alebo obnovenie aplikácií
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102586"
---
# <a name="delete-or-restore-applications"></a>Odstránenie alebo obnovenie aplikácií

**Odstránenie aplikácie z nájomníka služby Azure AD:**

1. Na **portáli Azure AD** vyberte položku **Podnikové aplikácie**. Potom vyhľadajte a vyberte aplikáciu, ktorú chcete odstrániť.
2. V časti **Správa** na ľavej table vyberte položku **Vlastnosti**.
3. Vyberte **položku Odstrániť** a potom **výberom položky Áno** potvrďte, že chcete aplikáciu odstrániť z nájomníka služby Azure AD.

Ďalšie informácie o odstránení aplikácie nájdete v téme Rýchly štart: Odstránenie aplikácie z [nájomníka služieb Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

V prostredí PowerShell rutina typu cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) odstráni konfigurácie proxy aplikácie z konkrétnej aplikácie v službe Azure Active Directory a môže úplne odstrániť aplikáciu, ak je to zadané.

Odstránenú **aplikáciu môžete obnoviť pomocou** prostredia PowerShell. Po identifikovaní aplikácie, ktorú chcete obnoviť, ju môžete obnoviť pomocou možnosti [Obnoviť-AzureADDeletedApplication.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
