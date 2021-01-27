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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015016"
---
# <a name="delete-or-restore-applications"></a>Odstránenie alebo obnovenie aplikácií

**Ak chcete odstrániť aplikáciu zo svojho nájomníka služby Azure AD**:

1. Na **portáli Azure AD** vyberte položku **podnikové aplikácie**. Potom vyhľadajte aplikáciu, ktorú chcete odstrániť, a vyberte ju.
2. V časti **Spravovať** na ľavej table vyberte položku **Vlastnosti**.
3. Vyberte položku **odstrániť** a potom výberom položky **Áno** potvrďte, že chcete aplikáciu odstrániť zo svojho nájomníka služby Azure AD.

Ďalšie informácie o odstránení aplikácie nájdete v téme rýchly štart [: odstránenie aplikácie z nájomníka služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

Rutina cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) v prostredí PowerShell odstraňuje konfigurácie aplikačných serverov proxy z konkrétnej aplikácie v službe Azure Active Directory a môže ju úplne odstrániť, ak je určená.

**Odstránenú aplikáciu môžete obnoviť** pomocou prostredia PowerShell. Po identifikácii aplikácie, ktorú chcete obnoviť, ju môžete obnoviť pomocou [obnovenia – AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
