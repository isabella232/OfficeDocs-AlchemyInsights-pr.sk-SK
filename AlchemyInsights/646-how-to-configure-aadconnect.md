---
title: 646 konfigurovaní AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28310816"
---
# <a name="configure-sync-features"></a><span data-ttu-id="e8ac1-102">Konfigurácia funkcie synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-102">Configure sync features</span></span>

<span data-ttu-id="e8ac1-p101">Azure AD pripojiť obsahuje niekoľko funkcií, ktoré sú predvolene povolené, alebo že môžete aktivovať neskôr. Niektoré funkcie vyžadujú dodatočné konfigurácia v osobitných prostrediach.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="e8ac1-p102">[Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limity objekty sú synchronizované s azúrovo reklamy. Predvolené, všetci používatelia, kontakty, skupiny aj Windows 10 sú synchronizované počítačové kontá. Môžete zahrnúť alebo vylúčiť objekty založené na domény, organizačné jednotky, alebo iné atribúty.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="e8ac1-p103">[Heslo hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla zo služby Active Directory lokálne Azure AD. To umožňuje správu hesiel na jednom mieste, ale používať rovnaké heslo lokálne a cloud prostredí. Pretože Active Directory autoritatívny zdroj, môžete použiť svoje vlastné politiky hesla.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="e8ac1-111">[Samoobslužné heslo reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje užívateľom obnoviť svoje heslá v cloude pri neustálom uplatňovaní lokálne heslo politika.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="e8ac1-112">[Zariadenie writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje registrovaných zariadení v Azure AD sa zapíše späť do služby Active Directory lokálne, takže môžu byť použité pre podmienený prístup.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="e8ac1-p104">[Zabránenie náhodnému odstráni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je predvolene zabrániť príliš veľa simultánnych objektov odstránenia (viac ako 500 objekty na synchronizácie). Môžete zmeniť toto nastavenie, aby vyhovovali potrebám vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="e8ac1-115">[Automatické aktualizácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) zapnutá predvolene expresné elektroinštalácií a pomáha zabezpečiť vašu verziu Azure AD pripojenie je vždy aktuálny.</span><span class="sxs-lookup"><span data-stu-id="e8ac1-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

