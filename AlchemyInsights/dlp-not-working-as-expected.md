---
title: DLP가 예상 대로 작동 하지 않음
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679699"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="d0b39-102">DLP가 예상 대로 작동 하지 않음</span><span class="sxs-lookup"><span data-stu-id="d0b39-102">DLP not working as expected</span></span>

<span data-ttu-id="d0b39-103">**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d0b39-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="d0b39-104">**DLP 설정**</span><span class="sxs-lookup"><span data-stu-id="d0b39-104">**Setting up DLP**</span></span>

<span data-ttu-id="d0b39-105">Office 365에서 **DLP (데이터 손실 방지)** 에 대 한 문제가 예상 대로 작동 하지 않습니까?</span><span class="sxs-lookup"><span data-stu-id="d0b39-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="d0b39-106">이 경우 **dlp 정책이** 올바르게 설정 되어 있고 데이터에 **dlp 정책이** 평가 되는 동안 검색 하는 작업이 포함 되어 있는지 확인 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0b39-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="d0b39-107">DLP 정책을 사용 하면 조직의 중요 한 정보를 식별 하 고 보호할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d0b39-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="d0b39-108">DLP 정책을 설정 하려면 [여기](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)에서 정보를 사용 합니다.</span><span class="sxs-lookup"><span data-stu-id="d0b39-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="d0b39-109">**DLP 정책에서 찾는 사항**</span><span class="sxs-lookup"><span data-stu-id="d0b39-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="d0b39-110">보안 및 준수 센터에서 **기본 제공 중요 한 정보 유형을** 사용 하는 경우 DLP 정책은 이러한 중요 한 유형을 검색할 때 특정 패턴 및 요소를 찾습니다.</span><span class="sxs-lookup"><span data-stu-id="d0b39-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="d0b39-111">**기본 제공 중요 한 정보 유형**</span><span class="sxs-lookup"><span data-stu-id="d0b39-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="d0b39-112">기본 제공 중요 한 유형과 중요 한 유형을 검색할 때 DLP 정책에서 찾는 사항에 대 한 자세한 내용은 [중요 한 정보 유형에서 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="d0b39-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="d0b39-113">**사용자 지정 중요 한 정보 유형**</span><span class="sxs-lookup"><span data-stu-id="d0b39-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="d0b39-114">사용자 지정 중요 한 정보 유형을 만들려는 경우에는 사용자 지정 중요 한 [정보](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)유형을 만드는 방법에 대 한 자세한 내용은 다음 문서를 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="d0b39-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="d0b39-115">**DLP 정책 테스트**</span><span class="sxs-lookup"><span data-stu-id="d0b39-115">**Test a DLP policy**</span></span>

<span data-ttu-id="d0b39-116">기본 제공 또는 사용자 지정 중요 한 정보 유형을 사용 하 여 데이터를 테스트 하려면 **분류**중요 정보 유형에 서 **테스트 유형** 옵션을 사용  >  **Sensitive info types**합니다.</span><span class="sxs-lookup"><span data-stu-id="d0b39-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="d0b39-117">자세한 내용은 [사용자 지정 중요 한 정보 유형 테스트](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="d0b39-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="d0b39-118">**보고서**</span><span class="sxs-lookup"><span data-stu-id="d0b39-118">**Reports**</span></span>
  
- <span data-ttu-id="d0b39-119">DLP 보고서를 사용 하 여 중요 한 데이터를 파악 [합니다.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="d0b39-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="d0b39-120">이벤트에 대 한 구체적인 세부 정보를 [문제 보고서](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)와 함께 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="d0b39-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
