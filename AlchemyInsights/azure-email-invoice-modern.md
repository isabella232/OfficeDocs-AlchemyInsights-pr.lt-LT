---
title: Šiuolaikinės "Azure" elektroninio pašto sąskaitos faktūros
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922137"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="98ad1-102">Pašto sąskaitų faktūrų išrašymas "Azure"</span><span class="sxs-lookup"><span data-stu-id="98ad1-102">Email invoicing in Azure</span></span>

<span data-ttu-id="98ad1-103">Turite turėti savininko arba bendraautorio vaidmenį atsiskaitymo profilyje arba jo atsiskaitymo paskyroje, kad atnaujintumėte savo el. pašto sąskaitos faktūros nuostatas.</span><span class="sxs-lookup"><span data-stu-id="98ad1-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="98ad1-104">Kai pasirinksite, visi vartotojai, turintys savininko, bendraautorio, skaitytojų ir sąskaitų faktūrų tvarkymo profilį, gaus sąskaitą faktūrą el. paštu.</span><span class="sxs-lookup"><span data-stu-id="98ad1-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="98ad1-105">Prisijunkite prie " [Azure" portalo](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="98ad1-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="98ad1-106">Ieškokite **išlaidų valdymo + atsiskaitymas**.</span><span class="sxs-lookup"><span data-stu-id="98ad1-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="98ad1-107">Kairėje pusėje pasirinkite **sąskaitos faktūros** kairėje ir puslapio viršuje pasirinkite **Siųsti sąskaitą faktūrą** .</span><span class="sxs-lookup"><span data-stu-id="98ad1-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="98ad1-108">Jei turite kelis atsiskaitymo profilius, pasirinkite atsiskaitymo profilį ir pasirinkite **pasirinkti**.</span><span class="sxs-lookup"><span data-stu-id="98ad1-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="98ad1-109">Pasirinkite **Naujinti**.</span><span class="sxs-lookup"><span data-stu-id="98ad1-109">Select **Update**.</span></span>
6. <span data-ttu-id="98ad1-110">Jei turite kelis atsiskaitymo profilius, pasirinkite atsiskaitymo profilį ir pasirinkite **pasirinkti**.</span><span class="sxs-lookup"><span data-stu-id="98ad1-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="98ad1-111">Jūs suteikiate kitiems prieigą prie peržiūrėti, atsisiųsti ir apmokėti sąskaitas faktūras, priskirdami jiems "invoice Manager" vaidmenį MCA arba MPA atsiskaitymo profiliui.</span><span class="sxs-lookup"><span data-stu-id="98ad1-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="98ad1-112">Jei pasirinkote gauti sąskaitą elektroniniu paštu, vartotojai taip pat gauna sąskaitas faktūras el. paštu.</span><span class="sxs-lookup"><span data-stu-id="98ad1-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="98ad1-113">Prisijunkite prie " [Azure" portalo](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="98ad1-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="98ad1-114">Ieškokite **išlaidų valdymo + atsiskaitymas**.</span><span class="sxs-lookup"><span data-stu-id="98ad1-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="98ad1-115">Pasirinkite **atsiskaitymo profiliai** iš kairės pusės.</span><span class="sxs-lookup"><span data-stu-id="98ad1-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="98ad1-116">Sąraše atsiskaitymo profiliai pasirinkite atsiskaitymo profilį, kuriam norite priskirti sąskaitos faktūros vadovo vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="98ad1-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="98ad1-117">Kairėje pusėje pasirinkite " **Access" valdiklis (iam)** ir pasirinkite **įtraukti** iš puslapio viršaus.</span><span class="sxs-lookup"><span data-stu-id="98ad1-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="98ad1-118">Išplečiamajame sąraše vaidmuo pasirinkite **sąskaitos vadybininkas**.</span><span class="sxs-lookup"><span data-stu-id="98ad1-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="98ad1-119">Įveskite vartotojo el. pašto adresą, kad suteiktumėte prieigą.</span><span class="sxs-lookup"><span data-stu-id="98ad1-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="98ad1-120">Pasirinkite **įrašyti** , kad priskirtumėte vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="98ad1-120">Select **Save** to assign the role.</span></span>
