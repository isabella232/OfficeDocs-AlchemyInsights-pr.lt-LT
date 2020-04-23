---
title: Vardų serverių keitimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706763"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="07bb9-102">Domeno vardų serverių atnaujinimas į „Microsoft“</span><span class="sxs-lookup"><span data-stu-id="07bb9-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="07bb9-103">Pastaba. Vardų serverių pakeitimų išplatinimas kartais gali trukti iki 48 valandų.</span><span class="sxs-lookup"><span data-stu-id="07bb9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="07bb9-104">Norėdami nustatyti domeną „Microsoft 365“, būtina atnaujinti vardų serverius registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="07bb9-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="07bb9-105">Sukurkite arba redaguokite vardų serverio įrašus domeno registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="07bb9-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="07bb9-106">Eikite į domeno registratoriaus svetainę ir raskite sritį, kurioje galima redaguoti domeno vardų serverius.</span><span class="sxs-lookup"><span data-stu-id="07bb9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="07bb9-107">Sukurkite arba redaguokite du vardų serverio įrašus, kad jie atitiktų šias reikšmes:</span><span class="sxs-lookup"><span data-stu-id="07bb9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="07bb9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="07bb9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="07bb9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="07bb9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="07bb9-110">Įrašyti pakeitimus.</span><span class="sxs-lookup"><span data-stu-id="07bb9-110">Save changes.</span></span>

<span data-ttu-id="07bb9-111">Šiame straipsnyje taip pat rasite išsamesnės informacijos: [Vardų serverių keitimas naudojant bet kokį domenų registratorių](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="07bb9-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  