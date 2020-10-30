---
title: Pripojenie k lokálnemu serveru Intune Exchange
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808142"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="4eb1f-102">Pripojenie k lokálnemu serveru Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="4eb1f-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="4eb1f-103">Podrobnosti o nastavení konektora medzi službou Intune a Exchangeom, ktorý je hosťovaný lokálne, nájdete v tejto dokumentácii:</span><span class="sxs-lookup"><span data-stu-id="4eb1f-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="4eb1f-104">Nastavenie lokálneho servera Exchange služby Intune v službe Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="4eb1f-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="4eb1f-105">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="4eb1f-105">**FAQ:**</span></span>

<span data-ttu-id="4eb1f-106">Otázka: pri pokuse o nastavenie konektora Exchange sa zobrazí chyba, ako je napríklad "verzia konektora Exchange nie je podporovaná".</span><span class="sxs-lookup"><span data-stu-id="4eb1f-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="4eb1f-107">Čo by mohlo byť príčinou?</span><span class="sxs-lookup"><span data-stu-id="4eb1f-107">What could be the cause?</span></span>

<span data-ttu-id="4eb1f-108">A: konto, ktoré používate, je licencované správne – musí mať aktívnu licenciu služby Intune</span><span class="sxs-lookup"><span data-stu-id="4eb1f-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="4eb1f-109">Otázka: je možné mať viacero konektorov Exchange?</span><span class="sxs-lookup"><span data-stu-id="4eb1f-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="4eb1f-110">A: môžete nastaviť iba jeden konektor Exchange na nájomníka služby Intune na organizáciu Exchange.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="4eb1f-111">Spojnica môže byť nainštalovaná iba na jednom serveri v organizácii s viacerými servermi Exchange.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="4eb1f-112">Nie je možné, že nie sú nakonfigurované spojnice pre lokálny Exchange aj Exchange Online konfigurované v tom istom nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="4eb1f-113">Otázka: môže spojnica použiť pole CAS ako pripojenie k serveru Exchange?</span><span class="sxs-lookup"><span data-stu-id="4eb1f-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="4eb1f-114">A: zadanie poľa CAS nie je podporovanou konfiguráciou v nastavení konektora.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="4eb1f-115">Mal by sa špecifikovať iba jeden server a mal by byť naprogramovaný v konfiguračnom súbore konektora, ktorý možno nájsť v</span><span class="sxs-lookup"><span data-stu-id="4eb1f-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="4eb1f-116">Program data\microsoft\microsoft Intune na premise konektora Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="4eb1f-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="4eb1f-117">Vyhľadajte nasledujúcu položku ```<ExchangeWebServiceURL />``` a nahraďte URL adresu serverom Exchange.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="4eb1f-118">**Napríklad**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="4eb1f-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="4eb1f-119">Ďalšie riešenie problémov nájdete v nasledujúcej dokumentácii: [Riešenie problémov s lokálnym konektorom Exchange služby Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="4eb1f-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="4eb1f-120">**Povolenie podrobného zapisovania do denníka pre konektor Exchange**</span><span class="sxs-lookup"><span data-stu-id="4eb1f-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="4eb1f-121">Otvorte konfiguračný súbor sledovania doplnku Exchange Connector na úpravy.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="4eb1f-122">Súbor je umiestnený na lokalite:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="4eb1f-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="4eb1f-123">**Napríklad**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="4eb1f-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="4eb1f-124">Vyhľadajte TraceSourceLine s nasledujúcim kľúčom: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="4eb1f-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="4eb1f-125">Zmeňte hodnotu uzla SourceLevel z informácií ActivityTracing (predvolené) na verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="4eb1f-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="4eb1f-126">**Napríklad**</span><span class="sxs-lookup"><span data-stu-id="4eb1f-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="4eb1f-127">Reštartovanie služby Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="4eb1f-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="4eb1f-128">Úplná synchronizácia na portáli Intune dovtedy, kým sa nedokončí, a potom zmeňte XML späť na "Information ActivityTracing" a reštartujte službu Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="4eb1f-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="4eb1f-129">Umiestnenie denníkov je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="4eb1f-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>