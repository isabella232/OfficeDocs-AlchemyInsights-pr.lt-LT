---
title: "\"Azure AD\" autentifikavimo ir įgaliojimo (\"AADSTS\") klaidų kodų trikčių šalinimas"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9800"
- "9005744"
ms.openlocfilehash: 14555dfcb1406fd3a3977012393714a713ff80dc
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036510"
---
# <a name="troubleshoot-azure-ad-authentication-and-authorization-aadsts-error-codes"></a><span data-ttu-id="8f0b5-102">"Azure AD" autentifikavimo ir įgaliojimo ("AADSTS") klaidų kodų trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="8f0b5-102">Troubleshoot Azure AD Authentication and Authorization (AADSTS) error codes</span></span>

<span data-ttu-id="8f0b5-103">Norėdami išspręsti AAD autentifikavimo ir autorizavimo klaidų kodus (AADSTS), atlikite šiuos rekomenduojamus veiksmus:</span><span class="sxs-lookup"><span data-stu-id="8f0b5-103">To resolve AAD authentication and authorization error codes (AADSTS), perform the following recommended steps:</span></span>

1. <span data-ttu-id="8f0b5-104">**"Klaidų kodų tvarkymas taikomojoje programoje"**</span><span class="sxs-lookup"><span data-stu-id="8f0b5-104">**Handling error codes in your application**</span></span>

- <span data-ttu-id="8f0b5-105">" **OAuth 2.0 spec**" https://tools.ietf.org/html/rfc6749#section-5.2 , pateikiama rekomendacijų, kaip tvarkyti klaidas autentifikavimo metu naudojant klaidos atsakymo klaidos dalį.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-105">The **OAuth2.0 spec**, https://tools.ietf.org/html/rfc6749#section-5.2, provides guidance on how to handle errors during authentication using the error portion of the error response.</span></span>

    - <span data-ttu-id="8f0b5-106">**klaida**: klaidos kodo eilutė, kurią galima naudoti klasifikuojant kylančias klaidas, ir ją reikia naudoti norint reaguoti į klaidas.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-106">**error**: An error code string that can be used to classify types of errors that occur, and should be used to react to errors.</span></span>
    - <span data-ttu-id="8f0b5-107">**Klaidos** laukas turi kelias galimas reikšmes – Peržiūrėkite protokolų dokumentacijos saitus ir oauth 2,0 specifikacijas, jei reikia daugiau informacijos apie konkrečias klaidas ir kaip jas reaguoti.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-107">The **error** field has several possible values - review the protocol documentation links and OAuth 2.0 specs for more information about specific errors and how to react to them.</span></span>

- <span data-ttu-id="8f0b5-108">Čia pateikiamas klaidos atsakymo pavyzdys:</span><span class="sxs-lookup"><span data-stu-id="8f0b5-108">Here is a sample error response:</span></span>
```
{
  "error": "invalid_scope",
  "error_description": "AADSTS70011: The provided value for the input parameter 'scope' is not 
valid. The scope https://example.contoso.com/activity.read is not valid.\r\nTrace ID: 255d1aef- 8c98-452f-ac51-23d051240864\r\nCorrelation ID: fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7\r\nTimestamp: 2016-01-09 02:02:12Z",
  "error_codes": [
    70011
  ],
  "timestamp": "2016-01-09 02:02:12Z",
  "trace_id": "255d1aef-8c98-452f-ac51-23d051240864",
  "correlation_id": "fb3d2015-bc17-4bb9-bb85-30c5cf1aaaa7", 
  "error_uri":"https://login.microsoftonline.com/error?code=70011"
}
```
2. <span data-ttu-id="8f0b5-109">**Peržvalgos dabartinės klaidos kodo informacija**</span><span class="sxs-lookup"><span data-stu-id="8f0b5-109">**Lookup current error code information**</span></span>

- <span data-ttu-id="8f0b5-110">Klaidų kodai ir pranešimai gali būti keičiami.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-110">Error codes and messages are subject to change.</span></span> <span data-ttu-id="8f0b5-111">Norėdami gauti naujausią informaciją, peržiūrėkite puslapį, https://login.microsoftonline.com/error kad rastumėte AADSTS klaidų aprašus, pataisymus ir kai kuriuos siūlomus sprendimo būdus.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-111">For the most current information, see the https://login.microsoftonline.com/error page to find AADSTS error descriptions, fixes, and some suggested workarounds.</span></span>
- <span data-ttu-id="8f0b5-112">Taip pat galite ieškoti ir šalinti " [Aadsts" klaidų kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) , išvardytus straipsnyje " [Azure AD" autentifikavimo ir autorizavimo klaidų kodai](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span><span class="sxs-lookup"><span data-stu-id="8f0b5-112">You can also search for and troubleshoot [AADSTS error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#aadsts-error-codes) listed in the article [Azure AD Authentication and authorization error codes](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes#handling-error-codes-in-your-application).</span></span>

3. <span data-ttu-id="8f0b5-113">**Gaukite pagalbos**</span><span class="sxs-lookup"><span data-stu-id="8f0b5-113">**Get Help**</span></span>

- <span data-ttu-id="8f0b5-114">[Kūrėjų palaikymo ir žinyno parinktys](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) – jei jums reikia atsakymo į klausimą arba pagalbos sprendžiant problemą, kurios neapima mūsų dokumentacijoje, gali būti, kad laikas susisiekti su ekspertais pagalbos klausimais.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-114">[Support and help options for developers](https://docs.microsoft.com/azure/active-directory/develop/developer-support-help-options) - If you need an answer to a question or help in solving a problem not covered in our documentation, it might be time to reach out to experts for help.</span></span> <span data-ttu-id="8f0b5-115">Šiame straipsnyje pateikiami keli pasiūlymai, kaip gauti atsakymus į klausimus, kaip kurti taikomąsias programas, integruotas su "Microsoft" tapatybės platforma.</span><span class="sxs-lookup"><span data-stu-id="8f0b5-115">This article provides several suggestions for getting answers to your questions as you develop apps that integrate with the Microsoft identity platform.</span></span>







