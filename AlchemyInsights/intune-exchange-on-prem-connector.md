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
# <a name="intune-exchange-on-premise-connector"></a>Pripojenie k lokálnemu serveru Intune Exchange

Podrobnosti o nastavení konektora medzi službou Intune a Exchangeom, ktorý je hosťovaný lokálne, nájdete v tejto dokumentácii:

[Nastavenie lokálneho servera Exchange služby Intune v službe Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ**

Otázka: pri pokuse o nastavenie konektora Exchange sa zobrazí chyba, ako je napríklad "verzia konektora Exchange nie je podporovaná". Čo by mohlo byť príčinou?

A: konto, ktoré používate, je licencované správne – musí mať aktívnu licenciu služby Intune

Otázka: je možné mať viacero konektorov Exchange?

A: môžete nastaviť iba jeden konektor Exchange na nájomníka služby Intune na organizáciu Exchange. Spojnica môže byť nainštalovaná iba na jednom serveri v organizácii s viacerými servermi Exchange.

Nie je možné, že nie sú nakonfigurované spojnice pre lokálny Exchange aj Exchange Online konfigurované v tom istom nájomníkovi.

Otázka: môže spojnica použiť pole CAS ako pripojenie k serveru Exchange?

A: zadanie poľa CAS nie je podporovanou konfiguráciou v nastavení konektora. Mal by sa špecifikovať iba jeden server a mal by byť naprogramovaný v konfiguračnom súbore konektora, ktorý možno nájsť v

Program data\microsoft\microsoft Intune na premise konektora Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Vyhľadajte nasledujúcu položku ```<ExchangeWebServiceURL />``` a nahraďte URL adresu serverom Exchange.

**Napríklad**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Ďalšie riešenie problémov nájdete v nasledujúcej dokumentácii: [Riešenie problémov s lokálnym konektorom Exchange služby Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Povolenie podrobného zapisovania do denníka pre konektor Exchange**

1. Otvorte konfiguračný súbor sledovania doplnku Exchange Connector na úpravy.  
Súbor je umiestnený na lokalite:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Napríklad**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Vyhľadajte TraceSourceLine s nasledujúcim kľúčom: OnPremisesExchangeConnectorService  
  
3. Zmeňte hodnotu uzla SourceLevel z informácií ActivityTracing (predvolené) na verbose ActivityTracing  

**Napríklad**
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
4. Reštartovanie služby Microsoft Intune Exchange  
5. Úplná synchronizácia na portáli Intune dovtedy, kým sa nedokončí, a potom zmeňte XML späť na "Information ActivityTracing" a reštartujte službu Microsoft Intune Exchange.  
6. Umiestnenie denníkov je: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`