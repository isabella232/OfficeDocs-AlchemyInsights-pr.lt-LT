---
title: Saugojimo strategijos "Exchange" administravimo centre neveikia
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952236"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="39122-102">Saugojimo strategijos "Exchange" administravimo centre</span><span class="sxs-lookup"><span data-stu-id="39122-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="39122-103">Jei norite, kad atliktų toliau nurodytų parametrų automatinį patikrinimą, šio puslapio viršuje pasirinkite mygtuką atgal <- ir įveskite vartotojo, kuris susiduria su saugojimo strategijų problemomis, el. pašto adresą.</span><span class="sxs-lookup"><span data-stu-id="39122-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="39122-104">Jei kyla problemų dėl saugojimo strategijų "Exchange" administravimo centre, kurie nėra taikomi pašto dėžutėms arba elementams, kurie nėra perkeliami į archyvo pašto dėžutę, patikrinkite šiuos dalykus:</span><span class="sxs-lookup"><span data-stu-id="39122-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="39122-105">**Pagrindinės priežastys:**</span><span class="sxs-lookup"><span data-stu-id="39122-105">**Root Causes:**</span></span>

- <span data-ttu-id="39122-106">**Valdomų aplankų** asistentas ne apdorojo vartotojo pašto dėžutės.</span><span class="sxs-lookup"><span data-stu-id="39122-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="39122-107">Valdomų aplankų pagalbinė priemonė bando apdoroti kiekvieną pašto dėžutę debesies pagrindu pagrįstoje organizacijoje kartą per septynias dienas.</span><span class="sxs-lookup"><span data-stu-id="39122-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="39122-108">**Sprendimas:** Paleiskite valdomų aplankų pagalbinę priemonę.</span><span class="sxs-lookup"><span data-stu-id="39122-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="39122-109">**Saugojimolaikymas** **įgalintas** pašto dėžutėje.</span><span class="sxs-lookup"><span data-stu-id="39122-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="39122-110">Jei pašto dėžutė buvo įdedama į saugojimo saugyklą, tuo metu pašto dėžutės saugojimo strategija nebus apdorojama.</span><span class="sxs-lookup"><span data-stu-id="39122-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="39122-111">**Sprendimas:** Patikrinkite saugojimo sulaikymo parametro būseną ir atnaujinkite, jei reikia.</span><span class="sxs-lookup"><span data-stu-id="39122-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="39122-112">Daugiau informacijos žr. [Pašto dėžutės saugojimo sulaikymas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="39122-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="39122-113">**Pastaba:** Jei pašto dėžutė mažesnė nei 10 MB, valdomų aplankų asistentas pašto dėžutės automatiškai ne apdoros.</span><span class="sxs-lookup"><span data-stu-id="39122-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="39122-114">Daugiau informacijos apie saugojimo strategijas "Exchange" administravimo centre žr.:</span><span class="sxs-lookup"><span data-stu-id="39122-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="39122-115">Saugojimo žymės ir saugojimo strategijos</span><span class="sxs-lookup"><span data-stu-id="39122-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="39122-116">[Saugojimo strategijos taikymas pašto dėžutėms](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) arba [Saugojimo žymių įtraukimas arba pašalinimas](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="39122-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="39122-117">Kaip nustatyti pašto dėžutėje laikomos sulaikytos vietos tipą</span><span class="sxs-lookup"><span data-stu-id="39122-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
