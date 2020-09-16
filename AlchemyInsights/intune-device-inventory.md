---
title: "\"Intune\" įrenginių inventorius"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667886"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="445d4-102">"Intune" įrenginių inventorius</span><span class="sxs-lookup"><span data-stu-id="445d4-102">Intune Device Inventory</span></span>

<span data-ttu-id="445d4-103">Įrenginių ašmenys suteikia administratoriui įžvalgų įrenginių dalyje valdymas, kurį naudoja "Intune" vienam įrenginiui.</span><span class="sxs-lookup"><span data-stu-id="445d4-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="445d4-104">Rodoma informacija: aparatūra, aptiktos taikomosios programos, įrenginio atitikties būsena ir įrenginio konfigūracijos būsena.</span><span class="sxs-lookup"><span data-stu-id="445d4-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="445d4-105">Įrenginių atsargų duomenys ir aptiktos taikomosios programos renkamos septynių dienų ciklu.</span><span class="sxs-lookup"><span data-stu-id="445d4-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="445d4-106">Taikomosios programos ir specifiniai aparatūros elementai skiriasi atsižvelgiant į įrenginio operacinę sistemą ir į tai, ar įrenginys yra asmeniškai, ar įmonės nuosavybė.</span><span class="sxs-lookup"><span data-stu-id="445d4-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="445d4-107">Daugiau informacijos rasite [įrenginio informacijos peržiūra "Intune](https://docs.microsoft.com/intune/device-inventory)".</span><span class="sxs-lookup"><span data-stu-id="445d4-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="445d4-108">**DUK**</span><span class="sxs-lookup"><span data-stu-id="445d4-108">**FAQ**</span></span>

<span data-ttu-id="445d4-109">K: aš negavau visos inventorizacijos programos, esančios "Intune", įtrauktų į "Windows" įrenginius.</span><span class="sxs-lookup"><span data-stu-id="445d4-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="445d4-110">kodėlgi ne?</span><span class="sxs-lookup"><span data-stu-id="445d4-110">Why not?</span></span>

<span data-ttu-id="445d4-111">A: šiuo metu "Windows 10" kompiuteriuose, kurie identifikuojami kaip įmonės įrenginiai, nurodomos tik šiuolaikinės taikomosios programos.</span><span class="sxs-lookup"><span data-stu-id="445d4-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="445d4-112">Intune nerenka informacijos apie "Win32" taikomąsias programas, įdiegtas šiuose įrenginiuose.</span><span class="sxs-lookup"><span data-stu-id="445d4-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="445d4-113">K: Kodėl telefono numeriai nerenkami iš visų įrenginių?</span><span class="sxs-lookup"><span data-stu-id="445d4-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="445d4-114">A: kai, pvz., paleidus mobiliųjų įrenginių atsargų ataskaitą, į "Intune" priskiriami telefonai, kurie priskiriami įmonės įrenginiams.</span><span class="sxs-lookup"><span data-stu-id="445d4-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="445d4-115">"Bring-Your-Own" įrenginio telefono numeriai visada yra dalinai užmaskuoti žvaigždute (\* \* \* \*) ir rodomi tik keturi paskutiniai skaitmenys.</span><span class="sxs-lookup"><span data-stu-id="445d4-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>