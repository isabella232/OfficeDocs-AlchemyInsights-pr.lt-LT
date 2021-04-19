---
title: Senstelėjusių dialogų įdėjimo įgalinimas norint atidaryti ataskaitas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814272"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="1fa91-102">Senstelėjusių dialogų įdėjimo įgalinimas norint atidaryti ataskaitas</span><span class="sxs-lookup"><span data-stu-id="1fa91-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="1fa91-103">**Požymis**</span><span class="sxs-lookup"><span data-stu-id="1fa91-103">**Symptom**</span></span>

<span data-ttu-id="1fa91-104">Vartotojai negali atidaryti ataskaitų.</span><span class="sxs-lookup"><span data-stu-id="1fa91-104">Users are unable to open reports.</span></span> <span data-ttu-id="1fa91-105">"Kažkas nutiko.</span><span class="sxs-lookup"><span data-stu-id="1fa91-105">"Something has gone wrong.</span></span> <span data-ttu-id="1fa91-106">Daugiau informacijos žr. techninėje išsamioje informacija."</span><span class="sxs-lookup"><span data-stu-id="1fa91-106">Check technical details for more details."</span></span>

<span data-ttu-id="1fa91-107">**Priežastis**</span><span class="sxs-lookup"><span data-stu-id="1fa91-107">**Cause**</span></span>

<span data-ttu-id="1fa91-108">Ataskaitos nepavyksta įkelti į UCI su klaida "Formos aprašas yra neapibrėžtas arba neapibrėžtas".</span><span class="sxs-lookup"><span data-stu-id="1fa91-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="1fa91-109">UCI ataskaitoms vis dar reikia senstelėjusių dialogų, todėl kliento sistemoje turi būti *įgalintas leidimaslegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="1fa91-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="1fa91-110">**Sprendimas**</span><span class="sxs-lookup"><span data-stu-id="1fa91-110">**Solution**</span></span>

1. <span data-ttu-id="1fa91-111">Eikite **į Parametrai >Administravimo > Sistemos parametrai > Skirtukas Bendra**.</span><span class="sxs-lookup"><span data-stu-id="1fa91-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="1fa91-112">Nustatykite "Enable embedding of certain legacy dialogs in Unified Interface browser client" (Įgalinti tam tikrų senstelėjusių dialogų įdėjimo įgalinimas vieningosios sąsajos naršyklės kliente) į **Taip**.</span><span class="sxs-lookup"><span data-stu-id="1fa91-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
