---
title: Nie je nastavený certifikát push apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440011"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="82e6a-102">Nie je nastavený certifikát push apple MDM</span><span class="sxs-lookup"><span data-stu-id="82e6a-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="82e6a-103">Certifikát push mdm apple mdm (známy aj ako certifikát služby APNS (Apple Push Notification Service) nebol nakonfigurovaný pre vaše predplatné.</span><span class="sxs-lookup"><span data-stu-id="82e6a-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="82e6a-104">Bez nakonfigurovaného push certifikátu Apple MDM sa nedarí zaregistrovať a spravovať zariadenia so systémom iOS a Mac OS.</span><span class="sxs-lookup"><span data-stu-id="82e6a-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="82e6a-105">Po pridaní certifikátu do služby Intune môžu používatelia nainštalovať aplikáciu Portál spoločnosti na registráciu svojich zariadení so systémom iOS.</span><span class="sxs-lookup"><span data-stu-id="82e6a-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="82e6a-106">Vyberte **"Súhlasím".**</span><span class="sxs-lookup"><span data-stu-id="82e6a-106">Select **"I agree."**</span></span> <span data-ttu-id="82e6a-107">spoločnosti Microsoft povolenie na odosielanie údajov spoločnosti Apple.</span><span class="sxs-lookup"><span data-stu-id="82e6a-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="82e6a-108">Vyberte **položku Download your CSR** the Intune certificate signing request required to create a Apple MDM push certificate.</span><span class="sxs-lookup"><span data-stu-id="82e6a-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="82e6a-109">Súbor sa používa na vyžiadanie certifikátu vzťahu dôveryhodnosti z portálu Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="82e6a-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="82e6a-110">Výberom **položky Create your MDM push Certificate (Vytvoriť certifikát push MDM)** prejdite na portál Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="82e6a-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="82e6a-111">Prihláste sa pomocou svojho firemného účtu Apple ID a vyberte **položku Vytvoriť certifikát**.</span><span class="sxs-lookup"><span data-stu-id="82e6a-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="82e6a-112">Vyberte **položku Vybrať súbor**, vyhľadajte súbor žiadosti o podpisovanie certifikátov a potom vyberte položku **Odovzdať**.</span><span class="sxs-lookup"><span data-stu-id="82e6a-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="82e6a-113">Na stránke Potvrdenie vyberte **položku Prevziať,** ak chcete prevziať súbor certifikátu (.pem) a súbor uložte lokálne.</span><span class="sxs-lookup"><span data-stu-id="82e6a-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="82e6a-114">**Poznámka:** Certifikát je priradený k účtu Apple ID, ktorý sa používa na jeho vytvorenie.</span><span class="sxs-lookup"><span data-stu-id="82e6a-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="82e6a-115">Ako osvedčený postup použite na správu úloh apple ID spoločnosti a uistite sa, že poštovú schránku monitoruje viac ako jedna osoba alebo pomocou distribučného zoznamu.</span><span class="sxs-lookup"><span data-stu-id="82e6a-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="82e6a-116">Nikdy nepoužívajte osobný účet Apple ID.</span><span class="sxs-lookup"><span data-stu-id="82e6a-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="82e6a-117">Na obnovenie certifikátu Apple Push každých 12 mesiacov použite rovnaký účet Apple ID.</span><span class="sxs-lookup"><span data-stu-id="82e6a-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="82e6a-118">Zadajte účet Apple ID použitý na vytvorenie certifikátu push Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="82e6a-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="82e6a-119">Zaznamenajte túto identifikáciu ako pripomenutie, keď potrebujete certifikát obnoviť.</span><span class="sxs-lookup"><span data-stu-id="82e6a-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="82e6a-120">Prejdite do súboru certifikátu (.pem), vyberte položku **Otvoriť a**potom vyberte položku **Odovzdať**.</span><span class="sxs-lookup"><span data-stu-id="82e6a-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="82e6a-121">Pomocou push certifikátu môže intune zaregistrovať a spravovať zariadenia Apple.</span><span class="sxs-lookup"><span data-stu-id="82e6a-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>