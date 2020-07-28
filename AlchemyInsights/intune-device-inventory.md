---
title: Intune įrenginių inventorius
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439658"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="a8f93-102">Intune įrenginių inventorius</span><span class="sxs-lookup"><span data-stu-id="a8f93-102">Intune Device Inventory</span></span>

<span data-ttu-id="a8f93-103">Įrenginių ašmenys suteikia administratoriui įžvalgą apie įrenginius, kurie yra valdomi "Intune", kiekvienam įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="a8f93-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="a8f93-104">Rodoma informacija apima: aparatūrą, aptiktas programas, įrenginio atitikties būseną ir įrenginio konfigūracijos būseną.</span><span class="sxs-lookup"><span data-stu-id="a8f93-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="a8f93-105">Atsargų duomenys aparatinei įrangai ir aptiktosioms programoms renkami septynių dienų ciklu.</span><span class="sxs-lookup"><span data-stu-id="a8f93-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="a8f93-106">Nurodytos taikomosios programos ir konkretūs aparatūros elementai skiriasi priklausomai nuo įrenginio operacinės sistemos ir nuo to, ar įrenginys yra asmeniškai, ar priklausantis įmonei.</span><span class="sxs-lookup"><span data-stu-id="a8f93-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="a8f93-107">Daugiau informacijos [ieškokite įrenginio informacijoje in Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="a8f93-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="a8f93-108">**DUK**</span><span class="sxs-lookup"><span data-stu-id="a8f93-108">**FAQ**</span></span>

<span data-ttu-id="a8f93-109">Klausimas: Aš negaunu visą inventoriaus sąrašą programų, esančių Intune-enrolled Windows prietaisai.</span><span class="sxs-lookup"><span data-stu-id="a8f93-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="a8f93-110">kodėlgi ne?</span><span class="sxs-lookup"><span data-stu-id="a8f93-110">Why not?</span></span>

<span data-ttu-id="a8f93-111">A: Šiuo metu išvardytos tik šiuolaikinės programėlės, skirtos "Windows 10" kompiuteriams, kurie identifikuojami kaip įmonės įrenginiai.</span><span class="sxs-lookup"><span data-stu-id="a8f93-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="a8f93-112">"Intune" nerenka informacijos apie šiuose įrenginiuose įdiegtas "Win32" programas.</span><span class="sxs-lookup"><span data-stu-id="a8f93-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="a8f93-113">Kl.: Kodėl telefono numeriai renkami ne iš visų įrenginių?</span><span class="sxs-lookup"><span data-stu-id="a8f93-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="a8f93-114">A: Telefonai, priskiriami įmonės įrenginiams intune, neidentifikuojami su visu telefono numeriu, kai, pvz., paleidžiate mobiliojo įrenginio atsargų ataskaitą.</span><span class="sxs-lookup"><span data-stu-id="a8f93-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="a8f93-115">Bring-you-own-device telefono numeriai visada iš dalies užmaskuotas žvaigždutėmis (\*\*\*\*), ir rodo tik paskutinius keturis skaitmenis.</span><span class="sxs-lookup"><span data-stu-id="a8f93-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>