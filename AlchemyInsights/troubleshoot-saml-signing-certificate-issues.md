---
title: Riešenie problémov s podpisom certifikátu SAML
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694449"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="93557-102">Riešenie problémov s podpisom certifikátu SAML</span><span class="sxs-lookup"><span data-stu-id="93557-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="93557-103">Ak chcete vyriešiť problém s podpisom certifikátu SAML, vykonajte tieto Odporúčané kroky:</span><span class="sxs-lookup"><span data-stu-id="93557-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="93557-104">Keď pridáte podnikovú aplikáciu, ktorá podporuje SSO, Azure vygeneruje certifikát, ktorý sa nazýva [podpisový certifikát SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="93557-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="93557-105">Tento certifikát má dátum uplynutia platnosti 3 roky.</span><span class="sxs-lookup"><span data-stu-id="93557-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="93557-106">Ak chcete zmeniť dátum uplynutia platnosti certifikátu, pozrite si tému [Prispôsobenie dátumu uplynutia platnosti certifikátu federácie a jeho prevrátenie do nového certifikátu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="93557-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="93557-107">Azure použije tento certifikát na podpísanie tokenov SAML vyžiadaných aplikáciou a odoslanie žiadosti o úspešné prihlásenie do aplikácie.</span><span class="sxs-lookup"><span data-stu-id="93557-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="93557-108">Ak chcete vykonať tento postup, Stiahnite si certifikát z portálu Azure a odošlite ho dodávateľovi aplikácie a dokončite proces SSO.</span><span class="sxs-lookup"><span data-stu-id="93557-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="93557-109">Po dokončení tohto procesu bude aplikácia dôverovať tomuto certifikátu a všetky tokeny SAML podpísané týmto certifikátom bude žiadosť akceptovať.</span><span class="sxs-lookup"><span data-stu-id="93557-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="93557-110">Ak platnosť tohto certifikátu uplynie, vytvorte nový certifikát, aktualizujte ho na dodávateľa aplikácie a potom ho aktivujte na stránke Azure.</span><span class="sxs-lookup"><span data-stu-id="93557-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="93557-111">Ďalšie informácie nájdete v téme [obnovenie certifikátu, ktorý bude čoskoro uplynúť](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="93557-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="93557-112">Ak platnosť certifikátu uplynie, používateľ nebude blokovaný.</span><span class="sxs-lookup"><span data-stu-id="93557-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="93557-113">[Pridajte e-mailovú adresu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , na ktorú sa majú prijímať oznámenia pred uplynutím platnosti aktuálneho certifikátu.</span><span class="sxs-lookup"><span data-stu-id="93557-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="93557-114">Krok 4 je voliteľný.</span><span class="sxs-lookup"><span data-stu-id="93557-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="93557-115">Zmeňte možnosti podpisu certifikátu SAML aplikácie a algoritmus podpisu certifikátu.</span><span class="sxs-lookup"><span data-stu-id="93557-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="93557-116">Ďalšie informácie nájdete v téme [Zmena možností podpisu certifikátu a algoritmu podpisu](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="93557-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

