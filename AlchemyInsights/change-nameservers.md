---
title: Vardų serverių keitimas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818620"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="5ccca-102">Domeno vardų serverių atnaujinimas į „Microsoft“</span><span class="sxs-lookup"><span data-stu-id="5ccca-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="5ccca-103">Pastaba. Vardų serverių pakeitimų išplatinimas kartais gali trukti iki 48 valandų.</span><span class="sxs-lookup"><span data-stu-id="5ccca-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="5ccca-104">Norėdami nustatyti domeną „Microsoft 365“, būtina atnaujinti vardų serverius registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="5ccca-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="5ccca-105">Sukurkite arba redaguokite vardų serverio įrašus domeno registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="5ccca-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="5ccca-106">Eikite į domeno registratoriaus svetainę ir raskite sritį, kurioje galima redaguoti domeno vardų serverius.</span><span class="sxs-lookup"><span data-stu-id="5ccca-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="5ccca-107">Sukurkite arba redaguokite du vardų serverio įrašus, kad jie atitiktų šias reikšmes:</span><span class="sxs-lookup"><span data-stu-id="5ccca-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="5ccca-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5ccca-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="5ccca-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="5ccca-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="5ccca-110">Įrašyti pakeitimus.</span><span class="sxs-lookup"><span data-stu-id="5ccca-110">Save changes.</span></span>

<span data-ttu-id="5ccca-111">Šiame straipsnyje taip pat rasite išsamesnės informacijos: [Vardų serverių keitimas naudojant bet kokį domenų registratorių](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="5ccca-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  