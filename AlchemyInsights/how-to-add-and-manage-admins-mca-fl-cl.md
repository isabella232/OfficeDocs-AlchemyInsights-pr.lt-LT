---
title: Kaip įtraukti ir valdyti administratoriai – MCA FL/CL
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
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692306"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="b8beb-102">Kaip įtraukti ir valdyti administratoriai – MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="b8beb-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="b8beb-103">Norėdami valdyti savo "Microsoft" kliento sutarties (MCA) atsiskaitymo paskyrą, galite naudoti skirtingus vaidmenis naudodami norimą "Access" lygį.</span><span class="sxs-lookup"><span data-stu-id="b8beb-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="b8beb-104">Šie vaidmenys yra be įtaisytųjų "Azure" tarnybų vaidmenų, padedančių jums valdyti išteklius.</span><span class="sxs-lookup"><span data-stu-id="b8beb-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="b8beb-105">**Norėdami įtraukti atsiskaitymo vaidmenis "Azure" portale:**</span><span class="sxs-lookup"><span data-stu-id="b8beb-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="b8beb-106">Prisijunkite prie " [Azure" portalo](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="b8beb-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="b8beb-107">Ieškokite *išlaidų valdymo + atsiskaitymas*.</span><span class="sxs-lookup"><span data-stu-id="b8beb-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="b8beb-108">Pasirinkite prieigos valdymo (IAM) sritį, pvz., atsiskaitymo paskyrą, atsiskaitymo profilį arba sąskaitos faktūros sekciją, kurioje norite suteikti prieigą.</span><span class="sxs-lookup"><span data-stu-id="b8beb-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="b8beb-109">"Access" valdiklio (IAM) puslapyje išvardijami vartotojai ir grupės, priskirtos kiekvienam tos aprėpties vaidmeniui.</span><span class="sxs-lookup"><span data-stu-id="b8beb-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="b8beb-110">Norėdami suteikti prieigą vartotojui, puslapio viršuje pasirinkite **įtraukti** .</span><span class="sxs-lookup"><span data-stu-id="b8beb-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="b8beb-111">Išplečiamajame sąraše *vaidmuo* pasirinkite vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="b8beb-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="b8beb-112">Įveskite vartotojo, kuriam norite suteikti prieigą, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="b8beb-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="b8beb-113">Pasirinkite **įrašyti** , kad priskirtumėte vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="b8beb-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="b8beb-114">Norėdami pašalinti vartotojo prieigą, pažymėkite vartotoją su vaidmens priskyrimu, kurį norite pašalinti.</span><span class="sxs-lookup"><span data-stu-id="b8beb-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="b8beb-115">Pasirinkite **Šalinti**.</span><span class="sxs-lookup"><span data-stu-id="b8beb-115">Select **Remove**.</span></span>

<span data-ttu-id="b8beb-116">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="b8beb-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="b8beb-117">Atsiskaitymo vaidmens aprašai</span><span class="sxs-lookup"><span data-stu-id="b8beb-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="b8beb-118">Atsiskaitymo paskyros vaidmenys ir užduotys</span><span class="sxs-lookup"><span data-stu-id="b8beb-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="b8beb-119">Darbo su "MCA" atsiskaitymo paskyra Pradžia</span><span class="sxs-lookup"><span data-stu-id="b8beb-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="b8beb-120">Prieigos prie "Microsoft" kliento sutarties tikrinimas</span><span class="sxs-lookup"><span data-stu-id="b8beb-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
