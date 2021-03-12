---
title: Priradenie roly denníka auditu v centre zabezpečenia dodržiavania & zabezpečenia služieb Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749522"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="0d66c-102">Priradenie roly denníka auditu v centre zabezpečenia dodržiavania & zabezpečenia služieb Office 365</span><span class="sxs-lookup"><span data-stu-id="0d66c-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="0d66c-103">Ak chcete vyhľadať denník auditu služieb Office 365, správca musí mať priradenú rolu **denníky auditu iba na zobrazenie** alebo rolu **denníky auditu** v službe Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0d66c-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="0d66c-104">Tieto roly sú predvolene priradené k skupinám rolí Správa súladu a správa organizácie.</span><span class="sxs-lookup"><span data-stu-id="0d66c-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="0d66c-105">Globálnym správcom v Office 365 a Microsoft 365 sa automaticky pridávajú ako členovia skupiny rolí Správa organizácie.</span><span class="sxs-lookup"><span data-stu-id="0d66c-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="0d66c-106">Ak chcete používateľovi povoliť vyhľadávanie s minimálnou úrovňou privilégií, vytvorte vlastnú skupinu rolí v službe Exchange Online, pridajte rolu denníkov **auditu iba zobrazenia** a denníky **auditu** a pridajte používateľa ako člena novej skupiny rolí.</span><span class="sxs-lookup"><span data-stu-id="0d66c-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="0d66c-107">Ďalšie informácie nájdete v téme [Správa skupín rolí v službe Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) a [Prehľadávanie denníka auditu v centre zabezpečenia & dodržiavania súladu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="0d66c-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>