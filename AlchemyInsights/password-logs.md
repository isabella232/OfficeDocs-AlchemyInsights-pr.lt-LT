---
title: Slaptažodžių žurnalai
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
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527175"
---
# <a name="password-logs"></a><span data-ttu-id="66d27-102">Slaptažodžių žurnalai</span><span class="sxs-lookup"><span data-stu-id="66d27-102">Password logs</span></span>

<span data-ttu-id="66d27-103">**Kilo problemų prisijungiant prie slaptažodžio nustatymo iš naujo audito žurnalų**</span><span class="sxs-lookup"><span data-stu-id="66d27-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="66d27-104">Norėdami šalinti problemas, susijusias su prieiga prie slaptažodžio nustatymo iš naujo audito žurnalų, atlikite toliau nurodytus veiksmus.</span><span class="sxs-lookup"><span data-stu-id="66d27-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="66d27-105">Įsitikinkite, kad turite teisę peržiūrėti audito žurnalus.</span><span class="sxs-lookup"><span data-stu-id="66d27-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="66d27-106">Autorizuojami tik šie vaidmenys:</span><span class="sxs-lookup"><span data-stu-id="66d27-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="66d27-107">Visuotinis administratorius</span><span class="sxs-lookup"><span data-stu-id="66d27-107">Global administrator</span></span>
 - <span data-ttu-id="66d27-108">Saugos administratorius</span><span class="sxs-lookup"><span data-stu-id="66d27-108">Security administrator</span></span>
 - <span data-ttu-id="66d27-109">Saugos skaitytojas</span><span class="sxs-lookup"><span data-stu-id="66d27-109">Security reader</span></span>

<span data-ttu-id="66d27-110">**Noriu matyti visus slaptažodžio nustatymo iš naujo audito įvykius iš pradžių įdiegto laiko**</span><span class="sxs-lookup"><span data-stu-id="66d27-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="66d27-111">Iki 120 000 slaptažodžio nustatymo iš naujo/registravimo įvykiai saugomi pastarųjų 30 dienų ataskaitose.</span><span class="sxs-lookup"><span data-stu-id="66d27-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="66d27-112">Šis maksimalus apribojimas taikomas vartotojo sąsajoje, kai atsisiunčiate CSV.</span><span class="sxs-lookup"><span data-stu-id="66d27-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="66d27-113">"1 000 000" įvykiai pasiekiami naudojant "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="66d27-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="66d27-114">Daugiau informacijos rasite toliau pateiktose nuorodose:</span><span class="sxs-lookup"><span data-stu-id="66d27-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="66d27-115">Savitarnos slaptažodžio nustatymo iš naujo įvykiai iš "Azure AD" ataskaitų ir įvykių API</span><span class="sxs-lookup"><span data-stu-id="66d27-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="66d27-116">Kaip greitai atsisiųsti slaptažodžio nustatymo iš naujo registraciją "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="66d27-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="66d27-117">**Noriu sužinoti daugiau apie slaptažodžio nustatymo iš naujo ataskaitų galimybes**</span><span class="sxs-lookup"><span data-stu-id="66d27-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="66d27-118">Patikrinkite, kas užregistravo arba iš naujo nustatydama slaptažodžius naudodami "Azure AD" slaptažodžio nustatymo iš naujo audito žurnalus "Azure" portalo dalyje **vartotojai ir grupės**.</span><span class="sxs-lookup"><span data-stu-id="66d27-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="66d27-119">Daugiau informacijos ieškokite šiuose saituose:</span><span class="sxs-lookup"><span data-stu-id="66d27-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="66d27-120">Slaptažodžio nustatymo iš naujo ataskaitų apžvalga</span><span class="sxs-lookup"><span data-stu-id="66d27-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="66d27-121">Kaip peržiūrėti slaptažodžio nustatymo iš naujo ataskaitas "Azure" portale</span><span class="sxs-lookup"><span data-stu-id="66d27-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="66d27-122">Savitarnos slaptažodžio nustatymo iš naujo įvykiai iš "Azure AD" ataskaitų ir įvykių API</span><span class="sxs-lookup"><span data-stu-id="66d27-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="66d27-123">Kaip greitai atsisiųsti slaptažodžio nustatymo iš naujo registraciją "PowerShell"</span><span class="sxs-lookup"><span data-stu-id="66d27-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


