---
title: Správa globálneho zoznamu adries organizácie a adresára offline
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022674"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="0c3cb-102">Správa globálneho zoznamu adries organizácie (GAL) a adresára offline (OAB)</span><span class="sxs-lookup"><span data-stu-id="0c3cb-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="0c3cb-103">Globálny zoznam adries (GAL) je zoznam objektov s e-mailom (ľubovoľný typ príjemcu, ktorý dokáže prijímať e-maily) v organizácii.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="0c3cb-104">Vo všetkých organizáciách sa GAL vytvára automaticky.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="0c3cb-105">Môžete vytvoriť ďalšie GAL a oddeliť používateľov podľa organizácie alebo lokality, ale jeden používateľ môže naraz vidieť len jeden GAL.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="0c3cb-106">Niektorí e-mailoví klienti, ako je napríklad Outlook pre Windows, si GAL sťahujú na používanie offline.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="0c3cb-107">Táto možnosť sa nazýva adresár offline (OAB).</span><span class="sxs-lookup"><span data-stu-id="0c3cb-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="0c3cb-108">V Exchangei online sa OAB aktualizuje len raz za 8 hodín a klienti si ho musia stiahnuť, aby aktualizovali svoju lokálnu kópiu OAB.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="0c3cb-109">Každá zmena príjemcu musí byť viditeľná v GAL, aby sa dostala do OAB.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="0c3cb-110">Tu je niekoľko často používaných postupov pre GAL a OAB:</span><span class="sxs-lookup"><span data-stu-id="0c3cb-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="0c3cb-111">Z rôznych dôvodov možno budete chcieť, aby sa niektoré objekty z GAL skryli.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="0c3cb-112">Pozrite si tému [Skryť príjemcov zo zoznamu adries](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="0c3cb-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="0c3cb-113">Ak potrebujete poskytnúť konkrétnym skupinám používateľov prispôsobené zobrazenia pre GAL organizácie, pozrite si tému [Politiky adresára v službe Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="0c3cb-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="0c3cb-114">[Vytvorte globálny zoznam adries v službe Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) a naučte sa pracovať s povoleniami pre GAL v téme [Zoznamy adries v službe Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="0c3cb-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="0c3cb-115">Nezabudnite, že ak vytvoríte nové zoznamy GAL, mali by ste vytvoriť aj nový OAB.</span><span class="sxs-lookup"><span data-stu-id="0c3cb-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="0c3cb-116">Prejdite si tému [Procesy adresárov offline](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="0c3cb-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
