---
title: Žurnalai ir ataskaitos
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036006"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="dcad2-102">Žurnalai ir ataskaitos</span><span class="sxs-lookup"><span data-stu-id="dcad2-102">Logs and Reporting</span></span>

<span data-ttu-id="dcad2-103">" [Azure Active Directory" ataskaitų DUK](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) atsakymų klausimai dažnai užduodami klausimai apie "Azure Active Directory" ("Azure AD") ataskaitas.</span><span class="sxs-lookup"><span data-stu-id="dcad2-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="dcad2-104">Daugiau informacijos ieškokite " [Azure Active Directory" ataskaitos](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="dcad2-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="dcad2-105">**Audito trikčių diagnostika**</span><span class="sxs-lookup"><span data-stu-id="dcad2-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="dcad2-106">Jei kyla problemų, susijusių su kai kuriomis audito veiklomis ir trūkstama veikla yra šiame [sąraše](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), prašom pateikti palaikymo bilietą.</span><span class="sxs-lookup"><span data-stu-id="dcad2-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="dcad2-107">Jei kyla problemų, susijusių su audito žurnalais jūsų nuomotojuje, pateikite palaikymo bilietą.</span><span class="sxs-lookup"><span data-stu-id="dcad2-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="dcad2-108">Jei jūsų audito veikla nėra rodoma iš karto "Azure" portale, peržiūrėkite mūsų [gaišties informaciją](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) ir failo palaikymo bilietą, jei vėlavimas viršija dokumentuotą gaištį.</span><span class="sxs-lookup"><span data-stu-id="dcad2-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="dcad2-109">"Azure AD" veiklos žurnalų išlaikymas</span><span class="sxs-lookup"><span data-stu-id="dcad2-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="dcad2-110">Jei nematote viso pasirinkto datų intervalo audito, galite atsisiųsti iki 250K eilučių (surūšiuotas pagal naujausius) prisijungimo iš "Azure" portalo.</span><span class="sxs-lookup"><span data-stu-id="dcad2-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="dcad2-111">Daugiau informacijos ieškokite [audito veiklos atsisiuntimas](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="dcad2-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="dcad2-112">**Problemų su prisijungimų trikčių diagnostika**</span><span class="sxs-lookup"><span data-stu-id="dcad2-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="dcad2-113">Galite matyti tik pastarųjų 30 dienų duomenis, jei turite "Azure AD Premium" (P1 arba P2) licenciją jūsų nuomotojui.</span><span class="sxs-lookup"><span data-stu-id="dcad2-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="dcad2-114">Prisijungimo moduliai galimi tik "Azure AD Premium" nuomininkams.</span><span class="sxs-lookup"><span data-stu-id="dcad2-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="dcad2-115">Jos negalima naudoti nemokamiems arba pagrindiniams licencijuotiems nuomotojams.</span><span class="sxs-lookup"><span data-stu-id="dcad2-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="dcad2-116">Jei jūsų Nuomotojas turi aukščiausios formos P1 licenciją ir negalite matyti prisijungimo, peržiūrėkite mūsų [gaišties informaciją](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) ir failo palaikymo bilietą, jei vėlavimas viršija dokumentuotą gaištį.</span><span class="sxs-lookup"><span data-stu-id="dcad2-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="dcad2-117">Jei nematote visų pasirinkto datų intervalo paskyrų, galite atsisiųsti iki 250K eilučių (surūšiuotas pagal naujausius) iš "Azure" portalo.</span><span class="sxs-lookup"><span data-stu-id="dcad2-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="dcad2-118">Daugiau informacijos rasite [prisijungimo veiklos atsisiuntimas](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="dcad2-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="dcad2-119">**Saugos ataskaitų trikčių šalinimas (vartotojams pažymėti rizikos, rizikingas prisijungimas)**</span><span class="sxs-lookup"><span data-stu-id="dcad2-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="dcad2-120">Su rizikos saugos ataskaita pažymėti vartotojai</span><span class="sxs-lookup"><span data-stu-id="dcad2-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="dcad2-121">Rizikingas prisijungimo ataskaita "Azure Active Directory" portale</span><span class="sxs-lookup"><span data-stu-id="dcad2-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="dcad2-122">"Azure Active Directory" rizikos įvykiai</span><span class="sxs-lookup"><span data-stu-id="dcad2-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
