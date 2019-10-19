---
title: Domeno vardų serverių atnaujinimas į „Office 365“
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742190"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="35dc0-102">Domeno vardų serverių atnaujinimas į „Office 365“</span><span class="sxs-lookup"><span data-stu-id="35dc0-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="35dc0-103">Pastaba. Vardų serverių pakeitimų išplatinimas kartais gali trukti iki 48 valandų.</span><span class="sxs-lookup"><span data-stu-id="35dc0-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="35dc0-104">Norėdami nustatyti domeną „Office 365“, būtina atnaujinti vardų serverius registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="35dc0-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="35dc0-105">Sukurkite arba redaguokite vardų serverio įrašus domeno registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="35dc0-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="35dc0-106">Eikite į domeno registratoriaus svetainę ir raskite sritį, kurioje galima redaguoti domeno vardų serverius.</span><span class="sxs-lookup"><span data-stu-id="35dc0-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="35dc0-107">Sukurkite arba redaguokite du vardų serverio įrašus, kad jie atitiktų šias reikšmes:</span><span class="sxs-lookup"><span data-stu-id="35dc0-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="35dc0-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="35dc0-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="35dc0-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="35dc0-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="35dc0-110">Įrašyti pakeitimus.</span><span class="sxs-lookup"><span data-stu-id="35dc0-110">Save changes.</span></span>

<span data-ttu-id="35dc0-111">Šiame straipsnyje taip pat rasite išsamesnės informacijos: [Vardų serverių keitimas norint nustatyti „Office 365“ domenų registratorių](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="35dc0-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  