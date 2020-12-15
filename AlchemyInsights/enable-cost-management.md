---
title: Išlaidų valdymo įgalinimas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677740"
---
# <a name="enable-cost-management"></a><span data-ttu-id="4290b-102">Išlaidų valdymo įgalinimas</span><span class="sxs-lookup"><span data-stu-id="4290b-102">Enable cost management</span></span>

<span data-ttu-id="4290b-103">**Ką reiškia jūsų organizacijai išjungiamos išlaidos?**</span><span class="sxs-lookup"><span data-stu-id="4290b-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="4290b-104">Organizacijos, naudojančios įmonės sutartį (EA) arba "Microsoft" kliento sutarties (MCA) paskyras, gali išjungti prieigą prie išlaidų informacijos ir kainodaros informacijos.</span><span class="sxs-lookup"><span data-stu-id="4290b-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="4290b-105">Kai prisijungiate prie "Azure" portalo, jos gali naudoti atsiskaitymo API, kad programiškai gautų sąskaitas faktūras (kai pasirinko) ir naudojimo informaciją.</span><span class="sxs-lookup"><span data-stu-id="4290b-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="4290b-106">**Kaip leisti papildomiems vartotojams pasiekti sąskaitas faktūras**</span><span class="sxs-lookup"><span data-stu-id="4290b-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="4290b-107">Eikite į "Azure" portalo **prenumeratos diską** .</span><span class="sxs-lookup"><span data-stu-id="4290b-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="4290b-108">Pasirinkite **sąskaitos faktūros** ir **prieiga prie sąskaitų faktūrų**.</span><span class="sxs-lookup"><span data-stu-id="4290b-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="4290b-109">Įjunkite "Access", o po to įrašykite pokyčius, kad vartotojai galėtų naudoti prenumeratos aprėpties vaidmenis Norėdami atsisiųsti sąskaitas faktūras.</span><span class="sxs-lookup"><span data-stu-id="4290b-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="4290b-110">Sąskaitos administratorius taip pat gali konfigūruoti, kad sąskaitos faktūros būtų siunčiamos elektroniniu paštu.</span><span class="sxs-lookup"><span data-stu-id="4290b-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="4290b-111">Norėdami sužinoti daugiau, peržiūrėkite [savo sąskaitos faktūros gavimas el. paštu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="4290b-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="4290b-112">**Kaip įtraukti vartotojus į atsiskaitymo skaitytuvo vaidmenį**</span><span class="sxs-lookup"><span data-stu-id="4290b-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="4290b-113">Eikite į "Azure" portalo **prenumeratos diską** .</span><span class="sxs-lookup"><span data-stu-id="4290b-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="4290b-114">Pasirinkite **prieigos valdymas (iam)** ir spustelėkite **įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="4290b-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="4290b-115">Puslapyje **pasirinkite vaidmenų** puslapį pasirinkite **atsiskaitymo skaitytojas** .</span><span class="sxs-lookup"><span data-stu-id="4290b-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="4290b-116">Įveskite norimo pakviesti vartotojo laišką, tada spustelėkite **gerai** , kad nusiųstumėte kvietimą.</span><span class="sxs-lookup"><span data-stu-id="4290b-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="4290b-117">Vadovaukitės instrukcijomis, pateiktomis kvietime į kvietimą prisijungti kaip atsiskaitymo skaitytojas.</span><span class="sxs-lookup"><span data-stu-id="4290b-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="4290b-118">Daugiau informacijos rasite [suteikti prieigą prie atsiskaitymo](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="4290b-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="4290b-119">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="4290b-119">**Recommended documents**</span></span>

- [<span data-ttu-id="4290b-120">"DA and AO" peržiūrų per EA portalą įjungimas</span><span class="sxs-lookup"><span data-stu-id="4290b-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="4290b-121">Išlaidos, įtrauktos į išlaidų valdymą</span><span class="sxs-lookup"><span data-stu-id="4290b-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="4290b-122">Palaikomi "Microsoft Azure" pasiūlymai</span><span class="sxs-lookup"><span data-stu-id="4290b-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="4290b-123">Išlaidų analizės išlaidų peržiūra</span><span class="sxs-lookup"><span data-stu-id="4290b-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="4290b-124">Prieigos prie atsiskaitymo informacijos pateikimas</span><span class="sxs-lookup"><span data-stu-id="4290b-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="4290b-125">Prieigos prie "Microsoft" kliento sutarties tikrinimas</span><span class="sxs-lookup"><span data-stu-id="4290b-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






