---
title: DLP 정책 팁이 작동하지 않습니다.
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958708"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="d4f94-102">DLP 정책 팁 문제</span><span class="sxs-lookup"><span data-stu-id="d4f94-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="d4f94-103">**중요**: 이 시기에는 SharePoint Online 및 OneDrive 서비스를 항상 사용할 수 있도록 하는 단계를 진행하고 있습니다. 자세한 내용은 [SharePoint Online 임시 기능 조정](https://aka.ms/ODSPAdjustments)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d4f94-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d4f94-104">전체 적용 모드에서 보안 및 준수 센터에서 DLP 정책에 & 팁을 구성하기 위해 다음을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="d4f94-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="d4f94-105">DLP 규칙에서 정책 **팁이** 사용하도록 설정되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="d4f94-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="d4f94-106">단계는 전자 메일 알림 보내기 및 DLP 정책에 대한 정책 [팁 표시를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="d4f94-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="d4f94-107">콘텐츠가 중요한 정보 유형 엔터티 정의 에 설명된 규칙을 트리거하는 데 필요한 내용과 [일치하는지 확인](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="d4f94-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="d4f94-108">정책 팁은 OWA와 Outlook 둘 다에 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4f94-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="d4f94-109">그러나 Outlook 2013 이상을 사용하는 경우 정책 팁은 특정 조건에서만 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="d4f94-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="d4f94-110">특정 조건 목록에 대한 자세한 내용은 정책 팁 표시를 위해 [Outlook 2013](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)이상에 지원되는 조건을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d4f94-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="d4f94-111">DLP 정책 팁에 대한 자세한 내용은 [DLP](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) 정책 팁 참조 및 DLP 정책 팁에 대한 [지원 매트릭스를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="d4f94-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>