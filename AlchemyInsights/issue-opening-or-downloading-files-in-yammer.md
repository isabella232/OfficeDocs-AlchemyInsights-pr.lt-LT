---
title: Failų atidarymo arba atsisiuntimo "Yammer" problema
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148334"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="c41b4-102">Failų atidarymo arba atsisiuntimo "Yammer" problema</span><span class="sxs-lookup"><span data-stu-id="c41b4-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="c41b4-103">Klasikinis "Yammer" palaiko kelias failų nusiuntimo į pranešimus ir grupes parinktį.</span><span class="sxs-lookup"><span data-stu-id="c41b4-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="c41b4-104">Atsižvelgiant į tinklo konfigūraciją, failai, kurie yra numatytieji kaip "SharePoint" saugomi.</span><span class="sxs-lookup"><span data-stu-id="c41b4-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="c41b4-105">Failų parinkiklis naujajame "Yammer" dar nepalaiko visų klasikiniame "Yammer" parinkčių.</span><span class="sxs-lookup"><span data-stu-id="c41b4-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="c41b4-106">Ateityje atnaujinus bus pridėtos papildomos funkcijos.</span><span class="sxs-lookup"><span data-stu-id="c41b4-106">A future update will add additional features.</span></span> <span data-ttu-id="c41b4-107">Daugiau informacijos rasite [Failo arba vaizdo pridėjimas prie "Yammer" pokalbio skelbimo](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="c41b4-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="c41b4-108">**Nepavyksta atidaryti arba atsisiųsti failo**</span><span class="sxs-lookup"><span data-stu-id="c41b4-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="c41b4-109">Failas gali būti nusiųstas į "Yammer", bet taip pat gali būti susietas su "SharePoint Online" failu.</span><span class="sxs-lookup"><span data-stu-id="c41b4-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="c41b4-110">Norėdami pašalinti triktis, pirmiausia turite nustatyti failo vietą.</span><span class="sxs-lookup"><span data-stu-id="c41b4-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="c41b4-111">Jei failas buvo įkeltas į "Yammer", jis turės \*.yammer.com URL.</span><span class="sxs-lookup"><span data-stu-id="c41b4-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="c41b4-112">Įsitikinkite, kad būtini URL ir IP adresai yra atblokuoti.</span><span class="sxs-lookup"><span data-stu-id="c41b4-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="c41b4-113">Daugiau informacijos rasite tinklaraščio įraše ["Yammer" užkoduoto IP adresų naudojimas nerekomenduojamas](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="c41b4-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="c41b4-114">Patikrinkite, ar vartotojas, kuris taip pat yra visuotinis administratorius, gali atsisiųsti failą.</span><span class="sxs-lookup"><span data-stu-id="c41b4-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="c41b4-115">Jei failas yra privatus, gali tekti naudoti asmeninio turinio režimą.</span><span class="sxs-lookup"><span data-stu-id="c41b4-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="c41b4-116">Daugiau informacijos rasite ["Yammer" asmeninio turinio stebėjimas](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="c41b4-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="c41b4-117">**"Yammer" tinklo lygio svečiai ir failai "SharePoint Online"**</span><span class="sxs-lookup"><span data-stu-id="c41b4-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="c41b4-118">["Yammer" tinklo lygio svečiai](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) nenaudoja "Azure AD B2B" ir yra vidiniai "Yammer" tarnybai, todėl jie negali pasiekti "Yammer" failų, saugomų "SharePoint".</span><span class="sxs-lookup"><span data-stu-id="c41b4-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="c41b4-119">Sukurkite išorinį AAD B2B vartotoją, kuris gali pasiekti dokumentų bibliotekas "SharePoint Online" naudodamas tą tapatybę.</span><span class="sxs-lookup"><span data-stu-id="c41b4-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="c41b4-120">Informacijos apie būsimą "Azure AD B2B" svečio palaikymą "Yammer", ieškokite ["Business-to business" (B2B) svečio palaikymas "Yammer Preview" – klientų sąlygos ir DUK.](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)</span><span class="sxs-lookup"><span data-stu-id="c41b4-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>