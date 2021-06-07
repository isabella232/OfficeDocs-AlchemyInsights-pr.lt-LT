---
title: Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793896"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="76dcb-102">Saugos "Microsoft Intune" naudojimas norint konfigūruoti Windows 10 įrenginius</span><span class="sxs-lookup"><span data-stu-id="76dcb-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="76dcb-103">"Intune" saugos bazinės linijos padeda apsaugoti vartotojus ir įrenginius.</span><span class="sxs-lookup"><span data-stu-id="76dcb-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="76dcb-104">Saugos bazinės linijos yra Windows parametrai iš anksto sukonfigūruotos grupės, naudojamos norint taikyti žinomų parametrų grupę ir numatytąsias reikšmes, kurias rekomenduoja atitinkamos saugos komandos.</span><span class="sxs-lookup"><span data-stu-id="76dcb-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="76dcb-105">Sukurdami saugos bazinį profilį "Intune", sukuriate šabloną, kurį sudaro keli įrenginio konfigūracijos profiliai.</span><span class="sxs-lookup"><span data-stu-id="76dcb-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="76dcb-106">Kai diegiate saugos bazines linijas vartotojų arba įrenginių grupėms, parametrai taikomi įrenginiams, veikiaems Windows 10 arba naujesnėse versijose.</span><span class="sxs-lookup"><span data-stu-id="76dcb-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="76dcb-107">Pvz., "Microsoft" mobiliųjų įrenginių valdymo (MDM) saugos bazinė linija automatiškai įgalina ""BitLocker"" keičiamiesiems diskams, reikalingas įrenginio atrakinimo slaptažodis ir išjungiamas bazinis autentifikavimas.</span><span class="sxs-lookup"><span data-stu-id="76dcb-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="76dcb-108">Kai numatytoji reikšmė neveikia jūsų aplinkoje, galite tinkinti bazinę liniją, kad pritaikytų norimus parametrus.</span><span class="sxs-lookup"><span data-stu-id="76dcb-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="76dcb-109">Saugos bazinės linijos taip pat padeda sukurti saugią darbo eigą Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="76dcb-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="76dcb-110">Saugos bazinė linija apima geriausias saugos parametrų praktikas ir rekomendacijas.</span><span class="sxs-lookup"><span data-stu-id="76dcb-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="76dcb-111">Intune partners with the Windows team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span><span class="sxs-lookup"><span data-stu-id="76dcb-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="76dcb-112">Jei tik pradedate naudoti "Intune" ir neįtikite, kur pradėti, saugos bazinės linijos padeda greitai sukurti ir įdiegti saugų profilį.</span><span class="sxs-lookup"><span data-stu-id="76dcb-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="76dcb-113">Jei šiuo metu naudojate grupės strategiją, perkelti į "Intune" valdymo tikslais yra daug lengviau naudojant saugos bazines linijas, nes jos integruotos į "Intune" ir apima pažangiausias valdymo galimybes.</span><span class="sxs-lookup"><span data-stu-id="76dcb-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="76dcb-114">Norėdami sužinoti daugiau, [žr. Windows bazinės linijos](/windows/security/threat-protection/windows-security-baselines) ir [mobiliųjų įrenginių valdymas.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="76dcb-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

