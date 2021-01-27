---
title: Taikomųjų programų naikinimas arba atkūrimas
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014904"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="b24e1-102">Taikomųjų programų naikinimas arba atkūrimas</span><span class="sxs-lookup"><span data-stu-id="b24e1-102">Delete or restore applications</span></span>

<span data-ttu-id="b24e1-103">**Norėdami panaikinti taikomąją programą iš "AZURE AD" nuomotojo**:</span><span class="sxs-lookup"><span data-stu-id="b24e1-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="b24e1-104">" **AZURE AD" portale** pasirinkite **įmonės taikomosios programos**.</span><span class="sxs-lookup"><span data-stu-id="b24e1-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="b24e1-105">Tada Raskite ir pasirinkite taikomąją programą, kurią norite panaikinti.</span><span class="sxs-lookup"><span data-stu-id="b24e1-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="b24e1-106">Kairiojoje srityje esančioje sekcijoje **tvarkyti** pasirinkite **Ypatybės**.</span><span class="sxs-lookup"><span data-stu-id="b24e1-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="b24e1-107">Pasirinkite **Naikinti**, tada pasirinkite **taip** , kad patvirtintumėte, jog norite panaikinti taikomąją programą iš "Azure AD" nuomotojo.</span><span class="sxs-lookup"><span data-stu-id="b24e1-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="b24e1-108">Daugiau informacijos apie tai, kaip panaikinti programėlę, rasite " [QuickStart": taikomosios programos naikinimas "Azure Active Directory" ("AZURE AD") nuomotojuje](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="b24e1-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="b24e1-109">"PowerShell", " [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) " cmdlet pašalina taikomosios programos tarpinio serverio konfigūracijas iš konkrečios programos "Azure Active Directory" ir gali visiškai panaikinti taikomąją programą, jei nurodyta.</span><span class="sxs-lookup"><span data-stu-id="b24e1-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="b24e1-110">Galite **atkurti panaikintą taikomąją programą** naudodami "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="b24e1-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="b24e1-111">Nustačius programą, kurią norite atkurti, galite ją atkurti naudodami [atkurti – Azureadnaikintiprograma](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="b24e1-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
