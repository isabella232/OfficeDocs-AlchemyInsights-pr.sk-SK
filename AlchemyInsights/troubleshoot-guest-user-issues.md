---
title: Riešenie problémov s hosťujúcimi používateľmi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901589"
---
# <a name="troubleshoot-guest-user-issues"></a>Riešenie problémov s hosťujúcimi používateľmi

1. Pokyny na spravovanie hosťovského prístupu k aplikáciám nájdete v téme [spravovanie hosťovského prístupu pomocou recenzií Azure AD Accessu](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Pridanie hosťovských používateľov do adresára na portáli Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): v tomto rýchlym pridávate nového hosťovského používateľa do adresára služby Azure AD prostredníctvom portálu Azure, odošlite pozvánku a zistite, ako vyzerá proces vyplatenia pozvania používateľa.
1. [Pridanie hosťujúceho používateľa s prostredím PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): v tomto rýchlym vykonaním použite príkaz New-AzureADMSInvitation na pridanie jedného hosťujúceho používateľa do nájomníka Azure.
1. Informácie o priradení používateľov a skupín k podnikovým aplikáciám v službe Azure Active Directory (Azure AD), a to buď z portálu Azure alebo pomocou prostredia PowerShell, nájdete [v téme Správa používateľských priradení aplikácie v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Služby Azure Active Directory (Azure AD) B2B spolupráca spolupracuje s väčšinou aplikácií, ktoré integrujú s Azúrovou REKLAMou. V tomto [článku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)prechádzame pokynmi na konfigurovanie niektorých obľúbených aplikácií SaaS na použitie so službou Azure AD B2B.
1. Ako organizácia využívajúca funkcie na spoluprácu v službe Azure Active Directory (Azure AD) na pozvanie hosťujúcich používateľov z partnerských organizácií na vašu službu Azure AD teraz môžete týmto používateľom B2B poskytnúť prístup k lokálnym aplikáciám. Tieto lokálne aplikácie môžu používať overovanie na základe SAML alebo integrované overovanie systému Windows (IWA) s delegovanou delegovanou protokolom Kerberos (KCD). Ďalšie informácie nájdete v téme [udelenie prístupu používateľom B2B v službe Azure AD Accessu do lokálnych aplikácií](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Zistite, ako [udeliť lokálne spravovaným partnerom kontá prístup k cloudovým zdrojom pomocou služby Azure AD B2B Collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).