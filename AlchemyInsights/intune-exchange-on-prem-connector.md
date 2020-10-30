---
title: "\"Intune Exchange\" vietinis sujungimas"
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
ms.contentlocale: lt-LT
ms.lasthandoff: 10/28/2020
ms.locfileid: "48808148"
---
# <a name="intune-exchange-on-premise-connector"></a>"Intune Exchange" vietinis sujungimas

Išsamios informacijos, kaip nustatyti jungtį tarp "Intune" ir "Exchange", kuri laikoma vietinėje svetainėje, rasite toliau pateiktus dokumentus.

["Microsoft Intune" "Azure" "Microsoft Intune" vietinio "Exchange" jungties nustatymas](https://docs.microsoft.com/intune/exchange-connector-install)

**DUK**

K: matau klaidą, pvz., "Exchange Connector versija nepalaikoma" bandant nustatyti "Exchange" jungtį. Kas gali būti priežastis?

A: jūsų naudojama paskyra licencijuota tinkamai – joje turi būti "Active Intune" licencija

K: ar galima turėti kelias "Exchange" jungtis?

A: galite nustatyti tik vieną "Exchange" jungtį per "Intune" nuomotoją vienai "Exchange" organizacijai. Jungtis gali būti įdiegta tik viename serveryje kelių serverių "Exchange" organizacijoje.

Taip pat negalite sukonfigūruoti "Exchange" ir "Exchange Online" konfigūruojamų tame pačiame nuomotojo jungčių.

K: ar jungtyje galima naudoti CAS masyvą kaip jo jungtį su "Exchange"?

A: CAS masyvas nurodo, kad jungties nustatyme nėra palaikomos konfigūracijos. Reikia nurodyti tik vieną serverį ir turi būti kieta jungties konfigūracijos faile, kurį galima rasti

programos "data\microsoft\microsoft Intune" vietinis Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Raskite šį įrašą ```<ExchangeWebServiceURL />``` ir pakeiskite URL naudodami "Exchange" serverį.

**Pavyzdžiui**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Jei turite papildomų trikčių šalinimo veiksmų, peržiūrėkite šiuos dokumentus: ["Intune" vietinio "Exchange" jungties trikčių diagnostika](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Įgalinimo "Exchange" jungties Įgalinę išsamų registravimą**

1. Atidarykite "Exchange" jungties sekimo konfigūracijos failą, skirtą redaguoti.  
Failas yra:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Pavyzdžiui**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Raskite "TraceSourceLine" su šiuo raktu: OnPremisesExchangeConnectorService  
  
3. Keisti SourceLevel mazgo reikšmę iš informacijos ActivityTracing (numatytoji) į išsamų ActivityTracing  

**Pavyzdžiui**
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
4. "Microsoft Intune" "Exchange" tarnybos paleidimas iš naujo  
5. Visas sinchronizavimas "Intune" portale, kol jis baigs ir pakeis XML į "Information ActivityTracing" ir iš naujo paleiskite "Microsoft Intune" "Exchange" tarnybą.  
6. Žurnalų vieta: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`