---
title: Konfigurácia LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885577"
---
# <a name="configure-ldap"></a><span data-ttu-id="1ce39-102">Konfigurácia LDAP</span><span class="sxs-lookup"><span data-stu-id="1ce39-102">Configure LDAP</span></span>

<span data-ttu-id="1ce39-103">Ak chcete nakonfigurovať LDAP, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="1ce39-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="1ce39-104">Skontrolujte stav svojej domény na [portáli Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="1ce39-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="1ce39-105">Skontrolujte, či je k dispozícii platné predplatné služby Azure AD a či je povolená služba Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="1ce39-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="1ce39-106">Certifikát potrebný na povolenie zabezpečeného LDAP musí byť získaný od dôveryhodného verejného certifikačného úradu alebo je certifikát s vlastným podpisom.</span><span class="sxs-lookup"><span data-stu-id="1ce39-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="1ce39-107">Skontrolujte, či sa certifikát riadi požadovanými [pokynmi](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="1ce39-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="1ce39-108">**Neplatný certifikát**</span><span class="sxs-lookup"><span data-stu-id="1ce39-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="1ce39-109">Ak chcete obnoviť certifikát, postupujte podľa krokov na vytvorenie nového certifikátu a opätovného nahrania: [Konfigurácia LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1ce39-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="1ce39-110">Ak chcete vyriešiť známy problém so zabezpečenými upozorneniami LDAP v doménových službách Azure Active Directory, pozrite si tému [vyriešenie upozornení LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="1ce39-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
