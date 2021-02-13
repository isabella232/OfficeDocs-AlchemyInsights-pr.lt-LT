---
title: "\"Microsoft Edge\" diegimas \"iOS\", \"iPadOS\" ir \"Android\""
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194518"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="1ce76-102">"Microsoft Edge" diegimas "iOS", "iPadOS" ir "Android"</span><span class="sxs-lookup"><span data-stu-id="1ce76-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="1ce76-103">Toliau apibendrintas scenarijus padės jums priskirti "Microsoft Edge" "iOS", "iPadOS" ir "Android" įrenginių vartotojams.</span><span class="sxs-lookup"><span data-stu-id="1ce76-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="1ce76-104">Jei užblokuojate vartotojus iš werbowania mobiliųjų įrenginių, Šis vedlys neveiks ir vartotojams reikės įdiegti "Microsoft Edge".</span><span class="sxs-lookup"><span data-stu-id="1ce76-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="1ce76-105">Valdomasis scenarijus apima šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="1ce76-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="1ce76-106">Būtinosios sąlygos</span><span class="sxs-lookup"><span data-stu-id="1ce76-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="1ce76-107">Įvadas</span><span class="sxs-lookup"><span data-stu-id="1ce76-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="1ce76-108">Pagrindai</span><span class="sxs-lookup"><span data-stu-id="1ce76-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="1ce76-109">Konfigūracijos</span><span class="sxs-lookup"><span data-stu-id="1ce76-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="1ce76-110">Užduotis</span><span class="sxs-lookup"><span data-stu-id="1ce76-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="1ce76-111">Peržiūra ir kūrimas</span><span class="sxs-lookup"><span data-stu-id="1ce76-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="1ce76-112">Atlikus veiksmus, nurodytus "Microsoft Intune" "Microsoft Edge" verslui leidžia atlikti šias "Microsoft Edge" funkcijas:</span><span class="sxs-lookup"><span data-stu-id="1ce76-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="1ce76-113">Dviguba tapatybė</span><span class="sxs-lookup"><span data-stu-id="1ce76-113">Dual identity</span></span>
- <span data-ttu-id="1ce76-114">Integravimas su "Microsoft Intune" programų apsaugos strategija</span><span class="sxs-lookup"><span data-stu-id="1ce76-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="1ce76-115">Integravimas su "Azure Active Directory" taikomosios programos tarpinio serverio</span><span class="sxs-lookup"><span data-stu-id="1ce76-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="1ce76-116">Valdomi Parankiniai ir pagrindinio puslapio spartieji klavišai</span><span class="sxs-lookup"><span data-stu-id="1ce76-116">Managed favorites and home page shortcuts</span></span>
