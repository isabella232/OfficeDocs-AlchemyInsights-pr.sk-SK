---
title: 646 konfigurovaní AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30779526"
---
# <a name="configure-sync-features"></a><span data-ttu-id="07cae-102">Konfigurácia funkcie synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="07cae-102">Configure sync features</span></span>

<span data-ttu-id="07cae-103">Azure AD pripojiť obsahuje niekoľko funkcií, ktoré sú predvolene povolené, alebo že môžete aktivovať neskôr.</span><span class="sxs-lookup"><span data-stu-id="07cae-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="07cae-104">Niektoré funkcie vyžadujú dodatočné konfigurácia v osobitných prostrediach.</span><span class="sxs-lookup"><span data-stu-id="07cae-104">Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="07cae-105">[Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limity objekty sú synchronizované s azúrovo reklamy.</span><span class="sxs-lookup"><span data-stu-id="07cae-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="07cae-106">Predvolené, všetci používatelia, kontakty, skupiny aj Windows 10 sú synchronizované počítačové kontá.</span><span class="sxs-lookup"><span data-stu-id="07cae-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="07cae-107">Môžete zahrnúť alebo vylúčiť objekty založené na domény, organizačné jednotky, alebo iné atribúty.</span><span class="sxs-lookup"><span data-stu-id="07cae-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="07cae-108">[Heslo hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla zo služby Active Directory lokálne Azure AD.</span><span class="sxs-lookup"><span data-stu-id="07cae-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="07cae-109">To umožňuje správu hesiel na jednom mieste, ale používať rovnaké heslo lokálne a cloud prostredí.</span><span class="sxs-lookup"><span data-stu-id="07cae-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="07cae-110">Pretože Active Directory autoritatívny zdroj, môžete použiť svoje vlastné politiky hesla.</span><span class="sxs-lookup"><span data-stu-id="07cae-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="07cae-111">[Samoobslužné heslo reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje užívateľom obnoviť svoje heslá v cloude pri neustálom uplatňovaní lokálne heslo politika.</span><span class="sxs-lookup"><span data-stu-id="07cae-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="07cae-112">[Zariadenie writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje registrovaných zariadení v Azure AD sa zapíše späť do služby Active Directory lokálne, takže môžu byť použité pre podmienený prístup.</span><span class="sxs-lookup"><span data-stu-id="07cae-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="07cae-113">[Zabránenie náhodnému odstráni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je predvolene zabrániť príliš veľa simultánnych objektov odstránenia (viac ako 500 objekty na synchronizácie).</span><span class="sxs-lookup"><span data-stu-id="07cae-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="07cae-114">Môžete zmeniť toto nastavenie, aby vyhovovali potrebám vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="07cae-114">You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="07cae-115">[Automatické aktualizácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) zapnutá predvolene expresné elektroinštalácií a pomáha zabezpečiť vašu verziu Azure AD pripojenie je vždy aktuálny.</span><span class="sxs-lookup"><span data-stu-id="07cae-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

