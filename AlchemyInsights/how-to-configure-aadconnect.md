---
title: 646 ako nakonfigurovať AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704504"
---
# <a name="configure-sync-features"></a><span data-ttu-id="01048-102">Konfigurácia funkcií synchronizácie</span><span class="sxs-lookup"><span data-stu-id="01048-102">Configure sync features</span></span>

<span data-ttu-id="01048-103">Azure AD Connect obsahuje niekoľko funkcií, ktoré sú predvolene zapnuté, alebo ktoré môžete neskôr povoliť.</span><span class="sxs-lookup"><span data-stu-id="01048-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="01048-104">Niektoré funkcie vyžadujú ďalšiu konfiguráciu v konkrétnych prostrediach.</span><span class="sxs-lookup"><span data-stu-id="01048-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="01048-105">[Filtrovanie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) obmedzení objekty sa synchronizujú so službou Azure AD.</span><span class="sxs-lookup"><span data-stu-id="01048-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="01048-106">Predvolene sa synchronizujú všetci používatelia, kontakty, skupiny a kontá počítačov s Windowsom 10.</span><span class="sxs-lookup"><span data-stu-id="01048-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="01048-107">Môžete zahrnúť alebo vylúčiť objekty na základe domén, organizačných jednotkí alebo iných atribútov.</span><span class="sxs-lookup"><span data-stu-id="01048-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="01048-108">[Synchronizácia hash hesla](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizuje hash hesla z lokálnej služby Active Directory do služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="01048-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="01048-109">To umožňuje správu hesiel na jednom mieste, ale použitie rovnakého hesla v lokálnom aj cloudovom prostredí.</span><span class="sxs-lookup"><span data-stu-id="01048-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="01048-110">Keďže Active Directory je autoritatívnym zdrojom, môžete použiť vlastné politiky hesiel.</span><span class="sxs-lookup"><span data-stu-id="01048-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="01048-111">[Samoobslužné vytvorenie nového hesla (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) umožňuje používateľom vytvoriť si nové heslá v cloude a zároveň použiť politiku lokálneho hesla.</span><span class="sxs-lookup"><span data-stu-id="01048-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="01048-112">[Zariadenie zápisom](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) umožňuje zapísať do lokálnej služby Active Directory registrované zariadenia v službe Azure AD, aby sa mohli použiť na podmienený prístup.</span><span class="sxs-lookup"><span data-stu-id="01048-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="01048-113">[Predchádzanie náhodným](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) odstránením je predvolene zapnuté, aby sa predišlo príliš mnohým súčasným odstránením objektov (viac než 500 objektov na synchronizáciu).</span><span class="sxs-lookup"><span data-stu-id="01048-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="01048-114">Toto nastavenie môžete zmeniť tak, aby vyhovovalo potrebám vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="01048-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="01048-115">[Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) je predvolene zapnutá pri expresných inštaláciách a pomáha zabezpečiť, že vaša verzia služby Azure AD Connect je vždy aktuálna.</span><span class="sxs-lookup"><span data-stu-id="01048-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
