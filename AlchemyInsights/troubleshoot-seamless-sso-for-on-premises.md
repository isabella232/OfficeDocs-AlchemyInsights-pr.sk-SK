---
title: Riešenie problémov s bezproblémovým jediným prihlásením (SSO) pre lokálne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816350"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="592dd-102">Riešenie problémov s bezproblémovým jediným prihlásením (SSO) pre lokálne</span><span class="sxs-lookup"><span data-stu-id="592dd-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="592dd-103">Ak chcete vyriešiť problémy s jediným prihlásením (SSO), vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="592dd-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="592dd-104">**Ako môžem prevrátiť kľúč dešifrovania Kerberos konta AZUREADSSO?**</span><span class="sxs-lookup"><span data-stu-id="592dd-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="592dd-105">Dôrazne odporúčame, aby ste prepísali kľúč dešifrovania Kerberos minimálne každých 30 dní.</span><span class="sxs-lookup"><span data-stu-id="592dd-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="592dd-106">Ak to chcete urobiť manuálne, pozrite si tému postup pri priradení [šifrovacích kľúčov Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="592dd-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="592dd-107">**Konfigurácia bezproblémového SSO**</span><span class="sxs-lookup"><span data-stu-id="592dd-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="592dd-108">Ak chcete nasadiť bezproblémové SSO, postupujte podľa krokov v téme [Azure Active Directory bezproblémové jediné prihlásenie: QuickStart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="592dd-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="592dd-109">**Poradný**</span><span class="sxs-lookup"><span data-stu-id="592dd-109">**Advisory**</span></span>

- <span data-ttu-id="592dd-110">[Jednoduché prihlásenie v službe Azure Active Directory: najčastejšie otázky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) – v tomto článku sa riešia najčastejšie otázky o službe Azure Active Directory bezšvíkové jednoduché Sign-On (bezproblémové SSO).</span><span class="sxs-lookup"><span data-stu-id="592dd-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="592dd-111">Udržujte opätovnú kontrolu nad novým obsahom.</span><span class="sxs-lookup"><span data-stu-id="592dd-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="592dd-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) – v tomto článku nájdete informácie o tom, ako vykonávať žiadosti o funkcie alebo klásť technické otázky o bezproblémovom SSO.</span><span class="sxs-lookup"><span data-stu-id="592dd-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="592dd-113">**Riešenie**</span><span class="sxs-lookup"><span data-stu-id="592dd-113">**Troubleshoot**</span></span>

<span data-ttu-id="592dd-114">[Riešenie problémov so službou Azure Active Directory bezproblémové jediné prihlásenie – v](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) tomto článku nájdete informácie o riešení problémov s bežnými problémami týkajúcimi sa bežných problémov so službou Azure Active Directory (Azure AD) jednoduché Sign-On (bezšvíkové SSO).</span><span class="sxs-lookup"><span data-stu-id="592dd-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







