---
title: Perkėlimo paslaugos – perkelti visas RDFE paslaugas į kitą prenumeratą
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692170"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="2d925-102">Perkėlimo paslaugos – perkelti visas RDFE paslaugas į kitą prenumeratą</span><span class="sxs-lookup"><span data-stu-id="2d925-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="2d925-103">**Išteklių perkėlimas**</span><span class="sxs-lookup"><span data-stu-id="2d925-103">**Move resources**</span></span>

<span data-ttu-id="2d925-104">"Azure" išteklius galima perkelti į kitą "Azure" prenumeratą arba išteklių grupę pagal tą pačią prenumeratą, naudojant "Azure" portalą, "Azure PowerShell", "Azure CLI" arba "ILSISI" API išteklių perkėlimą.</span><span class="sxs-lookup"><span data-stu-id="2d925-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="2d925-105">Kad galėtumėte perkelti išteklius, žiūrėkite:</span><span class="sxs-lookup"><span data-stu-id="2d925-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="2d925-106">Kontrolinis sąrašas prieš perkeliant išteklius</span><span class="sxs-lookup"><span data-stu-id="2d925-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="2d925-107">Paslaugos, kurias galima perkelti</span><span class="sxs-lookup"><span data-stu-id="2d925-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="2d925-108">Kaip patikrinti perkėlimą</span><span class="sxs-lookup"><span data-stu-id="2d925-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="2d925-109">Paslaugų gairių perkėlimas</span><span class="sxs-lookup"><span data-stu-id="2d925-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="2d925-110">Norėdami perkelti esamus išteklius į kitą išteklių grupę arba prenumeratą, galite naudoti:</span><span class="sxs-lookup"><span data-stu-id="2d925-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="2d925-111">"Azure" portalas</span><span class="sxs-lookup"><span data-stu-id="2d925-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="2d925-112">"Azure PowerShell"</span><span class="sxs-lookup"><span data-stu-id="2d925-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="2d925-113">"Azure CLI"</span><span class="sxs-lookup"><span data-stu-id="2d925-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="2d925-114">"POILSIU API"</span><span class="sxs-lookup"><span data-stu-id="2d925-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="2d925-115">Vadovėlis: " [Azure" išteklių perkėlimas į kitą išteklių grupę arba prenumeratą](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="2d925-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="2d925-116">**Klaidų šalinimas naudojant "Azure Resource Manager"**</span><span class="sxs-lookup"><span data-stu-id="2d925-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="2d925-117">Skaitykite toliau pateiktus straipsnius, Norėdami sužinoti apie kai kurias įprastas "Azure" diegimo klaidas ir gauti informaciją, kad jas išspręstumėte.</span><span class="sxs-lookup"><span data-stu-id="2d925-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="2d925-118">Jei nerandate diegimo klaidos klaidos kodo, žiūrėkite [rasti klaidos kodą](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="2d925-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="2d925-119">Diegimo klaidų šalinimas</span><span class="sxs-lookup"><span data-stu-id="2d925-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="2d925-120">"Azure" išteklių perkėlimo į naują išteklių grupę arba prenumeratą trikčių šalinimas</span><span class="sxs-lookup"><span data-stu-id="2d925-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="2d925-121">Nepamirškite, kad jei norite atnaujinti savo "Azure" prenumeratą, pvz., pereiti nuo nemokamos iki apmokėjimo, turėsite konvertuoti prenumeratą.</span><span class="sxs-lookup"><span data-stu-id="2d925-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="2d925-122">Jei norite atnaujinti nemokamą bandomąją versiją, peržiūrėkite [nemokamą bandomąją versiją arba "Microsoft" Įsivaizduokite "Azure" prenumeratą, kad galėtumėte sumokėti](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="2d925-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="2d925-123">Norėdami pakeisti "Pay-as-you-go" paskyrą, skaitykite " [Azure Pay-as-you-go" prenumeratos keitimas kitu pasiūlymu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="2d925-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="2d925-124">**Norėdami įtraukti arba susieti "Azure" prenumeratą į "Azure Active Directory" nuomotoją:**</span><span class="sxs-lookup"><span data-stu-id="2d925-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="2d925-125">Prisijunkite ir pasirinkite prenumeratą, kurią norite naudoti " [Azure" portalo puslapyje prenumeratos](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="2d925-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="2d925-126">Pasirinkite **keisti katalogą**.</span><span class="sxs-lookup"><span data-stu-id="2d925-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="2d925-127">Peržiūrėkite visus rodomus įspėjimus ir pasirinkite **keisti**.</span><span class="sxs-lookup"><span data-stu-id="2d925-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="2d925-128">Šis katalogas pakeičiamas į prenumeratą ir gausite pranešimą apie sėkmę.</span><span class="sxs-lookup"><span data-stu-id="2d925-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="2d925-129">Naudokite *katalogo* jungiklį, kad pereitumėte į naują katalogą.</span><span class="sxs-lookup"><span data-stu-id="2d925-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="2d925-130">Gali užtrukti iki 10 minučių, kol viskas rodoma tinkamai.</span><span class="sxs-lookup"><span data-stu-id="2d925-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="2d925-131">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="2d925-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="2d925-132">"Azure" prenumeratos nuosavybės perdavimas</span><span class="sxs-lookup"><span data-stu-id="2d925-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="2d925-133">Išteklių perkėlimas į naują išteklių grupę arba prenumeratą</span><span class="sxs-lookup"><span data-stu-id="2d925-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="2d925-134">Išteklių valdymas naudojant "Azure" portalą</span><span class="sxs-lookup"><span data-stu-id="2d925-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
