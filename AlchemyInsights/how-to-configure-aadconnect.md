---
title: 646 ako nakonfigurovať AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722578"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f542a-102">Konfigurácia funkcií synchronizácie</span><span class="sxs-lookup"><span data-stu-id="f542a-102">Configure sync features</span></span>

<span data-ttu-id="f542a-103">Azure AD Connect obsahuje niekoľko funkcií, ktoré sú predvolene povolené, alebo ktoré môžete povoliť neskôr.</span><span class="sxs-lookup"><span data-stu-id="f542a-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="f542a-104">Niektoré funkcie vyžadujú dodatočnú konfiguráciu v konkrétnych prostrediach.</span><span class="sxs-lookup"><span data-stu-id="f542a-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="f542a-105">[Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obmedzuje objekty synchronizované Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f542a-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="f542a-106">Predvolene sa synchronizujú všetci používatelia, kontakty, skupiny a počítačové kontá systému Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f542a-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="f542a-107">Môžete zahrnúť alebo vylúčiť objekty na základe domén, OUs alebo iných atribútov.</span><span class="sxs-lookup"><span data-stu-id="f542a-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="f542a-108">[Password hash synchronizácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla z lokálnej služby Active Directory Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f542a-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="f542a-109">To umožňuje správu hesiel na jednom mieste, ale použitie rovnakého hesla v lokálnom aj cloudovom prostredí.</span><span class="sxs-lookup"><span data-stu-id="f542a-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="f542a-110">Keďže služba Active Directory je autoritatívnym zdrojom, môžete použiť vlastné heslo politiky.</span><span class="sxs-lookup"><span data-stu-id="f542a-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="f542a-111">[Samoobslužné obnovenie hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje používateľom obnoviť svoje vlastné heslá v cloude, zatiaľ čo stále uplatňujú svoje lokálne heslo politiky.</span><span class="sxs-lookup"><span data-stu-id="f542a-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="f542a-112">[Zariadenie writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje registrované zariadenia v Azure AD sa zapíše späť do lokálnej služby Active Directory tak môžu byť použité pre podmieneného prístupu.</span><span class="sxs-lookup"><span data-stu-id="f542a-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="f542a-113">[Zabrániť náhodnému vymazaniu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) je povolená v predvolenom nastavení zabrániť príliš veľa simultánne objekt odstránenia (viac ako 500 objektov na synchronizáciu).</span><span class="sxs-lookup"><span data-stu-id="f542a-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="f542a-114">Toto nastavenie môžete zmeniť tak, aby spĺňate potreby vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="f542a-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="f542a-115">[Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je predvolene povolená pre expresné inštalácie a pomáha zabezpečiť, aby vaša verzia Azure AD Connect bola vždy aktuálna.</span><span class="sxs-lookup"><span data-stu-id="f542a-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
