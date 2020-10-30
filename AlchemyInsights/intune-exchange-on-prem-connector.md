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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="8f794-102">"Intune Exchange" vietinis sujungimas</span><span class="sxs-lookup"><span data-stu-id="8f794-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="8f794-103">Išsamios informacijos, kaip nustatyti jungtį tarp "Intune" ir "Exchange", kuri laikoma vietinėje svetainėje, rasite toliau pateiktus dokumentus.</span><span class="sxs-lookup"><span data-stu-id="8f794-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="8f794-104">"Microsoft Intune" "Azure" "Microsoft Intune" vietinio "Exchange" jungties nustatymas</span><span class="sxs-lookup"><span data-stu-id="8f794-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="8f794-105">**DUK**</span><span class="sxs-lookup"><span data-stu-id="8f794-105">**FAQ:**</span></span>

<span data-ttu-id="8f794-106">K: matau klaidą, pvz., "Exchange Connector versija nepalaikoma" bandant nustatyti "Exchange" jungtį.</span><span class="sxs-lookup"><span data-stu-id="8f794-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="8f794-107">Kas gali būti priežastis?</span><span class="sxs-lookup"><span data-stu-id="8f794-107">What could be the cause?</span></span>

<span data-ttu-id="8f794-108">A: jūsų naudojama paskyra licencijuota tinkamai – joje turi būti "Active Intune" licencija</span><span class="sxs-lookup"><span data-stu-id="8f794-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="8f794-109">K: ar galima turėti kelias "Exchange" jungtis?</span><span class="sxs-lookup"><span data-stu-id="8f794-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="8f794-110">A: galite nustatyti tik vieną "Exchange" jungtį per "Intune" nuomotoją vienai "Exchange" organizacijai.</span><span class="sxs-lookup"><span data-stu-id="8f794-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="8f794-111">Jungtis gali būti įdiegta tik viename serveryje kelių serverių "Exchange" organizacijoje.</span><span class="sxs-lookup"><span data-stu-id="8f794-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="8f794-112">Taip pat negalite sukonfigūruoti "Exchange" ir "Exchange Online" konfigūruojamų tame pačiame nuomotojo jungčių.</span><span class="sxs-lookup"><span data-stu-id="8f794-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="8f794-113">K: ar jungtyje galima naudoti CAS masyvą kaip jo jungtį su "Exchange"?</span><span class="sxs-lookup"><span data-stu-id="8f794-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="8f794-114">A: CAS masyvas nurodo, kad jungties nustatyme nėra palaikomos konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="8f794-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="8f794-115">Reikia nurodyti tik vieną serverį ir turi būti kieta jungties konfigūracijos faile, kurį galima rasti</span><span class="sxs-lookup"><span data-stu-id="8f794-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="8f794-116">programos "data\microsoft\microsoft Intune" vietinis Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="8f794-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="8f794-117">Raskite šį įrašą ```<ExchangeWebServiceURL />``` ir pakeiskite URL naudodami "Exchange" serverį.</span><span class="sxs-lookup"><span data-stu-id="8f794-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="8f794-118">**Pavyzdžiui**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="8f794-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="8f794-119">Jei turite papildomų trikčių šalinimo veiksmų, peržiūrėkite šiuos dokumentus: ["Intune" vietinio "Exchange" jungties trikčių diagnostika](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="8f794-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="8f794-120">**Įgalinimo "Exchange" jungties Įgalinę išsamų registravimą**</span><span class="sxs-lookup"><span data-stu-id="8f794-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="8f794-121">Atidarykite "Exchange" jungties sekimo konfigūracijos failą, skirtą redaguoti.</span><span class="sxs-lookup"><span data-stu-id="8f794-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="8f794-122">Failas yra:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="8f794-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="8f794-123">**Pavyzdžiui**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="8f794-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="8f794-124">Raskite "TraceSourceLine" su šiuo raktu: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="8f794-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="8f794-125">Keisti SourceLevel mazgo reikšmę iš informacijos ActivityTracing (numatytoji) į išsamų ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="8f794-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="8f794-126">**Pavyzdžiui**</span><span class="sxs-lookup"><span data-stu-id="8f794-126">**Example:**</span></span>
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
4. <span data-ttu-id="8f794-127">"Microsoft Intune" "Exchange" tarnybos paleidimas iš naujo</span><span class="sxs-lookup"><span data-stu-id="8f794-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="8f794-128">Visas sinchronizavimas "Intune" portale, kol jis baigs ir pakeis XML į "Information ActivityTracing" ir iš naujo paleiskite "Microsoft Intune" "Exchange" tarnybą.</span><span class="sxs-lookup"><span data-stu-id="8f794-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="8f794-129">Žurnalų vieta: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="8f794-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>