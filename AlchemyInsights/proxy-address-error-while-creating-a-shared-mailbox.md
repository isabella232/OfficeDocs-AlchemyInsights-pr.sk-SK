---
title: Chyba adresy proxy pri vytváraní zdieľanej poštovej schránky
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568305"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="f90f8-102">Chyba adresy servera proxy pri vytváraní poštovej schránky alebo iného objektu s povoleným e-mailom</span><span class="sxs-lookup"><span data-stu-id="f90f8-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="f90f8-103">Ak ste sa pokúsili vytvoriť objekt s podporou e-mailu (poštová schránka, zdieľaná poštová schránka atď.) a zobrazilo sa chybové hlásenie "adresa proxy" SMTP:alias@domain.com "sa už používa...", vybratá e-mailová adresa je už v organizácii prijatá iným objektom s podporou e-mailu.</span><span class="sxs-lookup"><span data-stu-id="f90f8-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="f90f8-104">Potrebujete nájsť používateľa, skupinu, zdieľanú poštovú schránku alebo verejný priečinok, ktorý má túto e-mailovú adresu, a odstrániť ho alebo zmeniť jeho e-mailovú adresu.</span><span class="sxs-lookup"><span data-stu-id="f90f8-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="f90f8-105">Potom môžete vytvoriť nový objekt s podporou e-mailu s uvoľnenou e-mailovou adresou.</span><span class="sxs-lookup"><span data-stu-id="f90f8-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="f90f8-106">Pomocou vyhľadávania na domovskej stránke ho vyhľadajte.</span><span class="sxs-lookup"><span data-stu-id="f90f8-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="f90f8-107">Na jeho vyhľadanie môžete použiť aj tento príkaz prostredia Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f90f8-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="f90f8-108">Ak nechcete odstrániť existujúcu e-mailovú adresu, vyberte novú e-mailovú adresu pre nový objekt, ktorý vytvárate.</span><span class="sxs-lookup"><span data-stu-id="f90f8-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  