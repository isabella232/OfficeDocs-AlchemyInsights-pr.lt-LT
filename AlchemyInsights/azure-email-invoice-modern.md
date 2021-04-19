---
title: Modernus "Azure" el. pašto sąskaitų faktūrų išrašymas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820834"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="96a5f-102">El. pašto sąskaitų faktūrų išrašymas "Azure"</span><span class="sxs-lookup"><span data-stu-id="96a5f-102">Email invoicing in Azure</span></span>

<span data-ttu-id="96a5f-103">Turite turėti savininko arba bendraautoriaus vaidmenį atsiskaitymo profilyje arba jo atsiskaitymo paskyroje, kad atnaujinsite savo el. pašto sąskaitos faktūros nuostatas.</span><span class="sxs-lookup"><span data-stu-id="96a5f-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="96a5f-104">Kai pasirinksite, visi vartotojai, kurie atsiskaitymo profilyje turi savininko, bendraautorių, skaitytojų ir sąskaitų faktūrų tvarkytuvo vaidmenis, gaus sąskaitą faktūrą el. paštu.</span><span class="sxs-lookup"><span data-stu-id="96a5f-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="96a5f-105">Prisijunkite prie [„Azure“ portalo](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="96a5f-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="96a5f-106">Ieškokite dalies **Išlaidų valdymas + Atsiskaitymas**.</span><span class="sxs-lookup"><span data-stu-id="96a5f-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="96a5f-107">**Kairėje** pusėje pasirinkite Sąskaitos faktūros, tada puslapio viršuje pasirinkite **El.** pašto sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="96a5f-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="96a5f-108">Jei turite kelis atsiskaitymo profilius, pasirinkite atsiskaitymo profilį, tada pasirinkite **Pasirinkti**.</span><span class="sxs-lookup"><span data-stu-id="96a5f-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="96a5f-109">Pasirinkite **Naujinti**.</span><span class="sxs-lookup"><span data-stu-id="96a5f-109">Select **Update**.</span></span>
6. <span data-ttu-id="96a5f-110">Jei turite kelis atsiskaitymo profilius, pasirinkite atsiskaitymo profilį, tada pasirinkite **Pasirinkti**.</span><span class="sxs-lookup"><span data-stu-id="96a5f-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="96a5f-111">Kitiems suteikiate prieigą peržiūrėti, atsisiųsti ir apmokėti sąskaitas faktūras priskirdami jiems MCA arba MPA atsiskaitymo profilio sąskaitų tvarkytuvo vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="96a5f-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="96a5f-112">Jei nusprendėte gauti sąskaitą faktūrą el. paštu, vartotojai taip pat gauna sąskaitas faktūras el. paštu.</span><span class="sxs-lookup"><span data-stu-id="96a5f-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="96a5f-113">Prisijunkite prie [„Azure“ portalo](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="96a5f-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="96a5f-114">Ieškokite dalies **Išlaidų valdymas + Atsiskaitymas**.</span><span class="sxs-lookup"><span data-stu-id="96a5f-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="96a5f-115">Kairėje **pusėje** pasirinkite Atsiskaitymo profiliai.</span><span class="sxs-lookup"><span data-stu-id="96a5f-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="96a5f-116">Atsiskaitymo profilių sąraše pasirinkite atsiskaitymo profilį, kuriam norite priskirti sąskaitų faktūrų tvarkytuvo vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="96a5f-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="96a5f-117">Kairėje pusėje pasirinkite Prieigos valdymas **(IAM),** **tada** puslapio viršuje pasirinkite Įtraukti.</span><span class="sxs-lookup"><span data-stu-id="96a5f-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="96a5f-118">Išplečiamajame sąraše Vaidmuo pasirinkite Sąskaitų **faktūrų tvarkytuvas**.</span><span class="sxs-lookup"><span data-stu-id="96a5f-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="96a5f-119">Įveskite vartotojo el. pašto adresą, kad suteikite prieigą.</span><span class="sxs-lookup"><span data-stu-id="96a5f-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="96a5f-120">Pasirinkite **Įrašyti,** kad priskirtumėte vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="96a5f-120">Select **Save** to assign the role.</span></span>
