---
title: Išorinių vartotojų įtraukimas į paskirstymo grupę
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910940"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="0dbd2-102">Išorinių vartotojų įtraukimas į paskirstymo grupę</span><span class="sxs-lookup"><span data-stu-id="0dbd2-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="0dbd2-103">Išorinio kontakto įtraukimas į paskirstymo grupę (GD) yra dviejų etapų procesas:</span><span class="sxs-lookup"><span data-stu-id="0dbd2-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="0dbd2-104">Sukurkite išorinio vartotojo pašto kontaktą:</span><span class="sxs-lookup"><span data-stu-id="0dbd2-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="0dbd2-105">Administravimo centre eikite į puslapį **Vartotojų** > [kontaktai.](https://admin.microsoft.com/adminportal/home#/Contact)</span><span class="sxs-lookup"><span data-stu-id="0dbd2-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="0dbd2-106">Pasirinkite **Įtraukti adresatą**.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="0dbd2-107">Įveskite adresato informaciją ir pasirinkite **Įtraukti**.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="0dbd2-108">Įtraukite pašto kontaktą į savo GENERALINĮ DIREKTORATĄ:</span><span class="sxs-lookup"><span data-stu-id="0dbd2-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="0dbd2-109">Administravimo centre eikite į puslapį **Grupių** > [grupės.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="0dbd2-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="0dbd2-110">Raskite GD, į kurį norite įtraukti išorinį vartotoją, ir pasirinkite jį, kad atidarytumėte redagavimo dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="0dbd2-111">Skirtuke **Nariai** pasirinkite **Peržiūrėti visus ir tvarkyti narius**.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="0dbd2-112">Pasirinkite **Įtraukti narius**.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="0dbd2-113">Pasirinkite pašto kontaktą, kurį sukūrėte atlikdami ankstesnį veiksmą, tada pasirinkite **Įrašyti**.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="0dbd2-114">Jei atlikus šiuos veiksmus išoriniai vartotojai negali siųsti el. laiškų GENERALINIAM DIREKTORATUI arba iš jo negauti el. laiškų, gali būti, kad GD pažymėtas taip, kad leistų siųsti tik vidinių naudotojų el. laiškus.</span><span class="sxs-lookup"><span data-stu-id="0dbd2-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="0dbd2-115">Galite patikrinti šią konfigūraciją ir pataisyti ją pagal nuorodas [čia](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="0dbd2-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="0dbd2-116">**Pastaba:** Šios instrukcijos netaikomos, jei jūsų grupės tipas yra "Microsoft 365 grupė", o ne "Paskirstymo grupė".</span><span class="sxs-lookup"><span data-stu-id="0dbd2-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="0dbd2-117">Tokiu atveju išorinį vartotoją galite įtraukti tiesiai į grupę iš "Outlook".</span><span class="sxs-lookup"><span data-stu-id="0dbd2-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="0dbd2-118">Išsamią informaciją apie "Microsoft 365 Groups" svečius ir išorinių svečių įtraukimo instrukcijas rasite [šiame straipsnyje](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="0dbd2-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  