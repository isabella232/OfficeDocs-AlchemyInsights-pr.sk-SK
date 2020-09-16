---
title: Centrum spravovania aplikácie Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670379"
---
# <a name="teams-admin-center"></a><span data-ttu-id="741cb-102">Centrum spravovania aplikácie Teams</span><span class="sxs-lookup"><span data-stu-id="741cb-102">Teams Admin Center</span></span>

<span data-ttu-id="741cb-103">Získajte informácie o spravovaní aplikácie Teams s [Centrom spravovania aplikácie Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="741cb-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="741cb-104">Ak nemôžete získať prístup do Centra spravovania aplikácie Teams, skontrolujte tieto položky:</span><span class="sxs-lookup"><span data-stu-id="741cb-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="741cb-105">Skontrolujte, či ste povolili zodpovedajúce [IP adresy balíka Office 365 a URL adresy](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) v obvodových zariadeniach (firewall, atď.) alebo v pravidlách brány firewall vo vašom lokálnom počítači.</span><span class="sxs-lookup"><span data-stu-id="741cb-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="741cb-106">Skontrolujte, či prihlasovacie meno, ktoré používate na prístup k portálu na správu tímov, zodpovedá vášmu používateľskému kontu uvedenému v [portáli pre správcov služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="741cb-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="741cb-107">Ak sa v Centre spravovania aplikácie Teams nezobrazujú používatelia, skontrolujte tieto položky:</span><span class="sxs-lookup"><span data-stu-id="741cb-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="741cb-108">Vytvorili ste za posledných 24 hodín používateľov alebo priradili licencie?</span><span class="sxs-lookup"><span data-stu-id="741cb-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="741cb-109">Uistite sa, že pred otvorením tiketu technickej podpory počkajte aspoň 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="741cb-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="741cb-110">Skontrolujte, či ste priradili zodpovedajúce licencie.</span><span class="sxs-lookup"><span data-stu-id="741cb-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="741cb-111">Ak máte lokálnu službu Active Directory, overte, či [je v poli proxyAddresses v lokálnej službe Active Directory hodnota msRTCSIP-PrimaryUserAddress alebo adresa SIP, ktorá sa zhoduje s formátom](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**meno** používateľa používateľa z [centra spravovania služby Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="741cb-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="741cb-112">Ak máte v úmysle uchovať nasadenie Skypu for Business Server a mať používateľov doma lokálne a online: postupujte podľa pokynov v časti **Nastavenie hybridného nasadenia v aplikácii teams a Skype for Business online** v ovládacom paneli Skypu for Business Server a premiestnite používateľov online.</span><span class="sxs-lookup"><span data-stu-id="741cb-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
