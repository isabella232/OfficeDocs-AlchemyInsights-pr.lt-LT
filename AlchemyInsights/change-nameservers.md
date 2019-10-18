---
title: Vardų serverių keitimas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736657"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="4ad15-102">Domeno vardų serverių atnaujinimas į „Office 365“</span><span class="sxs-lookup"><span data-stu-id="4ad15-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="4ad15-103">Pastaba. Vardų serverių pakeitimų išplatinimas kartais gali trukti iki 48 valandų.</span><span class="sxs-lookup"><span data-stu-id="4ad15-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="4ad15-104">Norėdami nustatyti domeną „Office 365“, būtina atnaujinti vardų serverius registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="4ad15-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="4ad15-105">Sukurkite arba redaguokite vardų serverio įrašus domeno registratoriaus svetainėje.</span><span class="sxs-lookup"><span data-stu-id="4ad15-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="4ad15-106">Eikite į domeno registratoriaus svetainę ir raskite sritį, kurioje galima redaguoti domeno vardų serverius.</span><span class="sxs-lookup"><span data-stu-id="4ad15-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="4ad15-107">Sukurkite arba redaguokite du vardų serverio įrašus, kad jie atitiktų šias reikšmes:</span><span class="sxs-lookup"><span data-stu-id="4ad15-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="4ad15-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4ad15-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="4ad15-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="4ad15-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="4ad15-110">Įrašyti pakeitimus.</span><span class="sxs-lookup"><span data-stu-id="4ad15-110">Save changes.</span></span>

<span data-ttu-id="4ad15-111">Šiame straipsnyje taip pat rasite išsamesnės informacijos: [Vardų serverių keitimas norint nustatyti „Office 365“ domenų registratorių](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="4ad15-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  