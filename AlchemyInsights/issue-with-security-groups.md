---
title: Problema su saugos grupėmis
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177499"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="7c40d-102">Problema su saugos grupėmis</span><span class="sxs-lookup"><span data-stu-id="7c40d-102">Issue with security groups</span></span>

<span data-ttu-id="7c40d-103">**Jei gaunate tinklo klaidos AADDS104**</span><span class="sxs-lookup"><span data-stu-id="7c40d-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="7c40d-104">Netinkamos tinklo saugos grupės taisyklės yra Dažniausios "Azure Active Directory" domenų tarnybos (AD DS) tinklo klaidų priežastys.</span><span class="sxs-lookup"><span data-stu-id="7c40d-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="7c40d-105">Virtualaus tinklo tinklo saugos grupė turi suteikti prieigą prie konkrečių prievadų ir protokolų.</span><span class="sxs-lookup"><span data-stu-id="7c40d-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="7c40d-106">Jei šie prievadai užblokuoti, "Azure" platformoje negalima stebėti arba atnaujinti valdomo domeno.</span><span class="sxs-lookup"><span data-stu-id="7c40d-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="7c40d-107">Taip pat paveikė "Azure AD" ir "Azure AD DS" sinchronizavimas.</span><span class="sxs-lookup"><span data-stu-id="7c40d-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="7c40d-108">Įsitikinkite, kad paliksite numatytuosius prievadus, kad išvengtumėte paslaugos nutraukimo.</span><span class="sxs-lookup"><span data-stu-id="7c40d-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="7c40d-109">Norėdami suprasti ir išspręsti bendruosius įspėjimus apie tinklo saugos grupės konfigūravimo problemas, skaitykite [saugos grupių įtraukimas ir tikrinimas](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="7c40d-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
