---
title: 'AIP: 정책이 예상대로 작동하지 않음'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663195"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="453de-102">AIP: 정책이 예상대로 작동하지 않음</span><span class="sxs-lookup"><span data-stu-id="453de-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="453de-103">Azure Information Protection: 정책이 예상대로 작동하지 않습니다. 다양한 정책 문제에 대한 권장 지침은 다음을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="453de-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="453de-104">시각적 표시에 문제가 있는 경우 [시각적 표시가 적용되는 경우](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)를 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="453de-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="453de-105">자동 레이블 지정에 문제가 있는 경우 [Azure Information Protection에 대한 자동 및 권장 분류 조건을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) 및 [중요한 정보 유형이 찾는 항목](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="453de-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="453de-106">기본/Pfile 보호와 관련된 문제가 발생하는 경우 [파일 API 구성](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)을 검토하세요.</span><span class="sxs-lookup"><span data-stu-id="453de-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="453de-107">올바르게 구성되지 않은 범위 지정 정책을 사용 중인지 확인합니다. [범위 지정된 정책을 사용하여 특정 사용자에 대한 Azure Information Protection 정책을 구성하는 방법](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="453de-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="453de-108">레이블이 지정된 문서를 첨부할 때 Outlook에서 자동 레이블 지정이 작동하지 않는 경우 여기에 설명된 대로 DRMEncryptProperty가 정의되어 있지 않은지 확인합니다. [보안용 IRM 레지스트리 설정](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="453de-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="453de-109">문제가 계속 발생하는 경우 Azure Information Protection 클라이언트 로그를 수집하고 내보낸 로그를 해당 티켓에 첨부하세요.</span><span class="sxs-lookup"><span data-stu-id="453de-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="453de-110">Office 문서를 열거나 Outlook에서 새 전자 메일을 작성합니다.</span><span class="sxs-lookup"><span data-stu-id="453de-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="453de-111">**보호/민감도** > **도움말 및 피드백**을 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="453de-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="453de-112">**로그 내보내기**를 클릭합니다.</span><span class="sxs-lookup"><span data-stu-id="453de-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="453de-113">원하는 위치에 로그를 저장하고 해당 서비스 요청에 첨부합니다.</span><span class="sxs-lookup"><span data-stu-id="453de-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="453de-114">추가 리소스:</span><span class="sxs-lookup"><span data-stu-id="453de-114">Additional resources:</span></span>

- [<span data-ttu-id="453de-115">Azure Information Protection용 시각적 표시에 대한 레이블을 구성하는 방법</span><span class="sxs-lookup"><span data-stu-id="453de-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="453de-116">Azure Information Protection 설명서 검토</span><span class="sxs-lookup"><span data-stu-id="453de-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="453de-117">Microsoft 365 앱의 민감도 레이블 사용</span><span class="sxs-lookup"><span data-stu-id="453de-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

