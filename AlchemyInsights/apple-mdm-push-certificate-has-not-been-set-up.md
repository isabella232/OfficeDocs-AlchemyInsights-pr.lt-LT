---
title: Apple MDM Push sertifikatas nenustatytas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lt-LT
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439379"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="43769-102">Apple MDM Push sertifikatas nenustatytas</span><span class="sxs-lookup"><span data-stu-id="43769-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="43769-103">"Apple MDM Push" sertifikatas (dar vadinamas "Apple Push Notification Service" (APNS) sertifikatu) nebuvo sukonfigūruotas jūsų prenumeratai.</span><span class="sxs-lookup"><span data-stu-id="43769-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="43769-104">Be sukonfigūruotos "Apple MDM Push" sertifikato negalite registruotis ir valdyti "iOS" ir "Mac OS" įrenginių.</span><span class="sxs-lookup"><span data-stu-id="43769-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="43769-105">Įtraukę sertifikatą į "Intune", vartotojai gali įdiegti programą Įmonės portalas, kad užregistruotų savo "iOS" įrenginius.</span><span class="sxs-lookup"><span data-stu-id="43769-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="43769-106">Pasirinkite **"Sutinku".**</span><span class="sxs-lookup"><span data-stu-id="43769-106">Select **"I agree."**</span></span> <span data-ttu-id="43769-107">suteikti "Microsoft" leidimą siųsti duomenis "Apple".</span><span class="sxs-lookup"><span data-stu-id="43769-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="43769-108">Pasirinkite **Atsisiųsti savo ĮSA** Intune sertifikato pasirašymo užklausą, reikalingą sukurti Apple MDM push sertifikatą.</span><span class="sxs-lookup"><span data-stu-id="43769-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="43769-109">Failas naudojamas norint prašyti patikimo ryšio sertifikato iš "Apple Push" sertifikatų portalo.</span><span class="sxs-lookup"><span data-stu-id="43769-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="43769-110">Pasirinkite **Sukurti savo MDM push sertifikatą,** kad pereitumėte į "Apple Push" sertifikatų portalą.</span><span class="sxs-lookup"><span data-stu-id="43769-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="43769-111">Prisijunkite naudodami savo įmonės "Apple ID", tada pasirinkite **Sukurti sertifikatą**.</span><span class="sxs-lookup"><span data-stu-id="43769-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="43769-112">Pasirinkite **Pasirinkti failą**, raskite sertifikato pasirašymo užklausos failą, tada pasirinkite **Nusiųsti**.</span><span class="sxs-lookup"><span data-stu-id="43769-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="43769-113">Puslapyje Patvirtinimas pasirinkite **Atsisiųsti,** kad atsisiųstumėte sertifikato (.pem) failą ir įrašytumėte failą vietoje.</span><span class="sxs-lookup"><span data-stu-id="43769-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="43769-114">**Pastaba:** sertifikatas susietas su "Apple ID", naudojamu jam sukurti.</span><span class="sxs-lookup"><span data-stu-id="43769-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="43769-115">Geriausia būtų naudoti įmonės "Apple ID" valdymo užduotims atlikti ir įsitikinti, kad pašto dėžutę stebi daugiau nei vienas asmuo arba naudodami siuntimo sąrašą.</span><span class="sxs-lookup"><span data-stu-id="43769-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="43769-116">Niekada nenaudokite asmeninio "Apple ID".</span><span class="sxs-lookup"><span data-stu-id="43769-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="43769-117">Naudokite tą patį "Apple ID", kad atnaujintumėte "Apple Push" sertifikatą kas 12 mėnesių.</span><span class="sxs-lookup"><span data-stu-id="43769-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="43769-118">Įveskite "Apple ID", naudojamą "Apple MDM" "push" sertifikatui sukurti.</span><span class="sxs-lookup"><span data-stu-id="43769-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="43769-119">Įrašykite šį ID kaip priminimą, kai reikia atnaujinti sertifikatą.</span><span class="sxs-lookup"><span data-stu-id="43769-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="43769-120">Eikite į sertifikato (.pem) failą, pasirinkite **Atidaryti**, tada pasirinkite **Nusiųsti**.</span><span class="sxs-lookup"><span data-stu-id="43769-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="43769-121">Su push sertifikatą, Intune gali registruotis ir valdyti Apple įrenginius.</span><span class="sxs-lookup"><span data-stu-id="43769-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>