---
title: Grupių priskyrimas "Azure AD" vaidmeniui
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885391"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="4bec9-102">Grupių priskyrimas "Azure AD" vaidmeniui</span><span class="sxs-lookup"><span data-stu-id="4bec9-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="4bec9-103">Jei norite priskirti "Azure AD" grupę su "Azure AD" funkcijos "Azure AD" funkcijos šaltiniu, atlikite šiuos veiksmus:</span><span class="sxs-lookup"><span data-stu-id="4bec9-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="4bec9-104">Kurti naują grupę – kurti naują grupę:</span><span class="sxs-lookup"><span data-stu-id="4bec9-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="4bec9-105">a.</span><span class="sxs-lookup"><span data-stu-id="4bec9-105">a.</span></span> <span data-ttu-id="4bec9-106">Prisijunkite prie "Azure AD" administravimo centro su **privilegijuotu vaidmenų administratoriumi** arba **visuotinio administratoriaus** teisėmis.</span><span class="sxs-lookup"><span data-stu-id="4bec9-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="4bec9-107">b.</span><span class="sxs-lookup"><span data-stu-id="4bec9-107">b.</span></span> <span data-ttu-id="4bec9-108">Pasirinkite " **Azure Active Directory" > grupės > visos grupės > nauja grupė**.</span><span class="sxs-lookup"><span data-stu-id="4bec9-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="4bec9-109">c.</span><span class="sxs-lookup"><span data-stu-id="4bec9-109">c.</span></span> <span data-ttu-id="4bec9-110">Kurti grupę.</span><span class="sxs-lookup"><span data-stu-id="4bec9-110">Create the group.</span></span>

2. <span data-ttu-id="4bec9-111">Priskirti grupės vaidmenį grupės kūrimo metu arba sukūrus grupę.</span><span class="sxs-lookup"><span data-stu-id="4bec9-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="4bec9-112">a.</span><span class="sxs-lookup"><span data-stu-id="4bec9-112">a.</span></span> <span data-ttu-id="4bec9-113">Norėdami priskirti grupės vaidmenį grupės kūrimo metu, įjunkite " **AZURE AD" vaidmenis** , kuriuos galima priskirti grupei ir kurti grupę.</span><span class="sxs-lookup"><span data-stu-id="4bec9-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="4bec9-114">b.</span><span class="sxs-lookup"><span data-stu-id="4bec9-114">b.</span></span> <span data-ttu-id="4bec9-115">Norėdami priskirti vaidmenį grupei po to, kai jis buvo sukurtas, pereikite į naujai sukurtos grupės skirtuką **priskirti vaidmenys** ir priskirkite grupei vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="4bec9-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="4bec9-116">**"Azure AD" vaidmeniui priskirtos grupės narių valdymas**</span><span class="sxs-lookup"><span data-stu-id="4bec9-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="4bec9-117">Norint išvengti teisių didesnių teisių, pagal numatytuosius numatytuosius, tik privilegijuotieji vaidmenų administratoriai ir visuotiniai administratoriai gali modifikuoti grupės, priskirtos vaidmeniui, narystę.</span><span class="sxs-lookup"><span data-stu-id="4bec9-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="4bec9-118">Tačiau jie gali pasirinkti priskirti tokiai grupei savininką ir pavesti šiai užduočiai.</span><span class="sxs-lookup"><span data-stu-id="4bec9-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="4bec9-119">Daugiau informacijos apie debesies grupių priskyrimo į "Azure AD" vaidmenis ieškokite skyriuje [skelbimų Vaidmenų priskyrimas debesies grupei](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="4bec9-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="4bec9-120">Daugiau informacijos apie trikčių diagnostikos vaidmenis, priskirtus debesies grupėms, ieškokite [vaidmenų, priskirtų debesies grupėms, trikčių šalinimas](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="4bec9-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





