---
title: "\"Azure\" atsiskaitymo nuosavybės perdavimas"
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
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922163"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="08f76-102">"Azure" atsiskaitymo nuosavybės perdavimas</span><span class="sxs-lookup"><span data-stu-id="08f76-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="08f76-103">Prisijunkite prie " [Azure" portalo](https://portal.azure.com/) kaip atsiskaitymo paskyros, kurioje yra norima perduoti prenumeratą, administratorius.</span><span class="sxs-lookup"><span data-stu-id="08f76-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="08f76-104">Jei nesate tikri, ar esate ir administratorius, arba jei reikia nustatyti, kas yra, peržiūrėkite [paskyros atsiskaitymo administratoriaus](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)nustatymas.</span><span class="sxs-lookup"><span data-stu-id="08f76-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="08f76-105">**Išlaidų valdymo ir atsiskaitymo** ieška.</span><span class="sxs-lookup"><span data-stu-id="08f76-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="08f76-106">Kairiojoje srityje pasirinkite **prenumeratos** .</span><span class="sxs-lookup"><span data-stu-id="08f76-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="08f76-107">Atsižvelgiant į "Access", gali tekti pasirinkti atsiskaitymo aprėptį ir **prenumeratos** arba "Azure" **prenumeratas**.</span><span class="sxs-lookup"><span data-stu-id="08f76-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="08f76-108">Pasirinkite prenumeratos, kurią norite perkelti, **nuosavybę**</span><span class="sxs-lookup"><span data-stu-id="08f76-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="08f76-109">Įveskite vartotojo, kuris yra paskyros administratorius, kuris bus naujas prenumeratos savininkas, elektroninio pašto adresą, tada pasirinkite **Siųsti perkėlimo užklausą**</span><span class="sxs-lookup"><span data-stu-id="08f76-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="08f76-110">Vartotojas gauna laišką su nurodymais, kaip peržiūrėti savo perkėlimo užklausą.</span><span class="sxs-lookup"><span data-stu-id="08f76-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="08f76-111">Norėdami patvirtinti perkėlimo užklausą, vartotojas pasirenka saitą el. laiške ir vadovaujasi nurodymais.</span><span class="sxs-lookup"><span data-stu-id="08f76-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="08f76-112">**Pastaba** : jei persiunčiate savo prenumeratos nuosavybėn vartotojo paskyrą kitame "Azure AD" nuomotojuje, visi [vaidmenimis pagrįsti "Access" valdymo (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)priskyrimai, skirti išteklių prenumeratai, yra visam laikui pašalinti.</span><span class="sxs-lookup"><span data-stu-id="08f76-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="08f76-113">Tik naujasis savininkas turės prieigą prie prenumeratos išteklių valdymo.</span><span class="sxs-lookup"><span data-stu-id="08f76-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="08f76-114">Daugiau informacijos ieškokite [vartotojo prenumeratos perdavimas kitam "AZURE AD" nuomotojui](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="08f76-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="08f76-115">**Rekomenduojami dokumentai**</span><span class="sxs-lookup"><span data-stu-id="08f76-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="08f76-116">Atsiskaitymo už "Azure" prenumeratos nuosavybės perdavimas į kitą paskyrą</span><span class="sxs-lookup"><span data-stu-id="08f76-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="08f76-117">Apie "Azure" prenumeratos atsiskaitymo nuosavybės perdavimą</span><span class="sxs-lookup"><span data-stu-id="08f76-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="08f76-118">"Visual Studio", "Microsoft" partnerių tinklo (MPN) perkėlimas ir mokėjimas už "dev/Test" prenumeratas</span><span class="sxs-lookup"><span data-stu-id="08f76-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="08f76-119">Perduoti nuosavybės DUK</span><span class="sxs-lookup"><span data-stu-id="08f76-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="08f76-120">Perdavimo nuosavybės problemų šalinimas</span><span class="sxs-lookup"><span data-stu-id="08f76-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
