---
title: Ištaisyti klaidą Programa neaptikta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666986"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="3cf93-102">Ištaisyti klaidą „Programa neaptikta“</span><span class="sxs-lookup"><span data-stu-id="3cf93-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="3cf93-103">Programos diegimo klaida „Programa nebuvo aptikta po sėkmingo įdiegimo“, apie kurią praneša „Intune“, gali įvykti visose pagrindinėse OS platformose („Windows“, „iOS“ ir „Android“).</span><span class="sxs-lookup"><span data-stu-id="3cf93-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="3cf93-104">Dažniausi scenarijai, kurie sugeneruoja šią klaidą, apima:</span><span class="sxs-lookup"><span data-stu-id="3cf93-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="3cf93-105">Programa buvo atnaujinta ne iš „Intune“ (trečiosios šalies programų parduotuvės) po pradinio diegimo.</span><span class="sxs-lookup"><span data-stu-id="3cf93-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="3cf93-106">Pvz., kai kurios programos, kaip „Google Chrome“, gali atlikti automatinius naujinimus.</span><span class="sxs-lookup"><span data-stu-id="3cf93-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="3cf93-107">Vartotojas pašalino programą po pradinio diegimo.</span><span class="sxs-lookup"><span data-stu-id="3cf93-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="3cf93-108">Norėdami išspręsti šią problemą, pirmiausia atlikite susijusių įrenginių apžvalgą, kad nustatytumėte scenarijų, kuriuo įvyksta klaida.</span><span class="sxs-lookup"><span data-stu-id="3cf93-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="3cf93-109">Jei programa buvo atnaujinta ne iš „Intune“, programos diegimas gali būti nustatytas nepaisyti programos versijos.</span><span class="sxs-lookup"><span data-stu-id="3cf93-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="3cf93-110">Norėdami tai padaryti, dalyje **Programų konfigūravimas > Programos informacija**nustatykite **Nepaisyti programos** versijos į **Taip**.</span><span class="sxs-lookup"><span data-stu-id="3cf93-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="3cf93-111">Orientuojantis į klientą gali būti tikslinga diegti taikomąją programą kaip „būtiną“ ir užtikrinti, kad būtų įdiegta naujausia versija.</span><span class="sxs-lookup"><span data-stu-id="3cf93-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="3cf93-112">Be to, „iOS“ platformoje galima naudoti **automatinio naujinimo** funkcines galimybes, susietas su „Apple Volume“ pirkimo programa, kurią galima konfigūruoti automatiškai atnaujinti į naujas programų versijas, kai jos bus pasiekiamos.</span><span class="sxs-lookup"><span data-stu-id="3cf93-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="3cf93-113">Jei reikia daugiau informacijos apie programų diegimo trikčių šalinimą, žr. [Programų diegimo problemų šalinimas](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="3cf93-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
