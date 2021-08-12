---
title: Riešenie problémov s hosťu používateľom
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939394"
---
# <a name="troubleshoot-guest-user-issues"></a>Riešenie problémov s hosťu používateľom

1. Pokyny na správu hosťovského prístupu k aplikáciám nájdete v téme [Správa prístupu hostí pomocou recenzií služby Azure AD na prístup.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Pridanie hostí do adresára na [portáli Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)V tomto rýchlom štarte pridáte nového hosťa do adresára Azure AD prostredníctvom portálu Azure, odošlete pozvánku a uvidíte, ako vyzerá proces na uplatnenie pozvánky hosťa.
1. [Pridanie hosťa pomocou prostredia PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)V tomto rýchlom štarte použijete príkaz New-AzureADMSInvitation a do nájomníka služby Azure pridáte jedného hosťa.
1. Ak chcete zistiť, ako priradiť používateľov a skupiny do podnikových aplikácií v službe Azure Active Directory (Azure AD), buď z portálu Azure, alebo pomocou prostredia PowerShell, pozrite si časť Správa priradenia používateľov k aplikácii v [službe Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory B2B spolupráca (Azure AD) funguje s väčšinou aplikácií integrovaných so službou Azure AD. V tomto [článku](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)nájdete pokyny na konfiguráciu niektorých obľúbených SaaS aplikácií na použitie so službou Azure AD B2B.
1. Ako organizácia, ktorá používa funkcie B2B spolupráce služby Azure Active Directory (Azure AD) na pozvanie hostí z partnerských organizácií do služby Azure AD, môžete týmto používateľom B2B poskytnúť prístup k lokálnym aplikáciám. Tieto lokálne aplikácie môžu používať overovanie na základe protokolu SAML alebo Integrované Windows overovania (IWA) s delegovaním protokolu Kerberos (KCD). Ďalšie informácie nájdete v téme [Udelenie prístupu používateľov B2B v službe Azure AD k lokálnym aplikáciám.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Zistite, ako [poskytnúť lokálne spravované partnerské kontá prístup k zdrojom v cloude pomocou B2B spolupráce služby Azure AD.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)