---
title: Centrum spravovania aplikácie Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826394"
---
# <a name="teams-admin-center"></a><span data-ttu-id="a0e28-102">Centrum spravovania aplikácie Teams</span><span class="sxs-lookup"><span data-stu-id="a0e28-102">Teams Admin Center</span></span>

<span data-ttu-id="a0e28-103">Získajte informácie o spravovaní aplikácie Teams s [Centrom spravovania aplikácie Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a0e28-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="a0e28-104">Ak nemôžete získať prístup do Centra spravovania aplikácie Teams, skontrolujte tieto položky:</span><span class="sxs-lookup"><span data-stu-id="a0e28-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="a0e28-105">Skontrolujte, či ste povolili zodpovedajúce [IP adresy balíka Office 365 a URL adresy](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v obvodových zariadeniach (firewall, atď.) alebo v pravidlách brány firewall vo vašom lokálnom počítači.</span><span class="sxs-lookup"><span data-stu-id="a0e28-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="a0e28-106">Skontrolujte, či prihlasovacie meno, ktoré používate na prístup k portálu na správu tímov, zodpovedá vášmu používateľskému kontu uvedenému v [portáli pre správcov služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="a0e28-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="a0e28-107">Ak sa v Centre spravovania aplikácie Teams nezobrazujú používatelia, skontrolujte tieto položky:</span><span class="sxs-lookup"><span data-stu-id="a0e28-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="a0e28-108">Vytvorili ste za posledných 24 hodín používateľov alebo priradili licencie?</span><span class="sxs-lookup"><span data-stu-id="a0e28-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="a0e28-109">Uistite sa, že pred otvorením tiketu technickej podpory počkajte aspoň 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="a0e28-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="a0e28-110">Skontrolujte, či ste priradili zodpovedajúce licencie.</span><span class="sxs-lookup"><span data-stu-id="a0e28-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="a0e28-111">Ak máte lokálnu službu Active Directory, overte, či je hodnota [msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) alebo adresa SIP v poli ProxyAddresses v lokálnej službe Active Directory jedinečná a formát zodpovedá sip: Meno používateľa z Centra spravovania služby [Microsoft 365.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="a0e28-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="a0e28-112">Ak plánujete nasadenie Skype for Business Servera a máte používateľov lokálne a online, postupujte podľa krokov v časti **Nastavenie hybridného** nasadenia s aplikáciami Teams a Skype for Business Online na ovládacom paneli Skype for Business Servera a presuňte používateľov online.</span><span class="sxs-lookup"><span data-stu-id="a0e28-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
