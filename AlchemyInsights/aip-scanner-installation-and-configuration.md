---
title: 'AIP 스캐너: 설치 및 구성'
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
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686648"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="c9082-102">AIP 스캐너: 설치 및 구성</span><span class="sxs-lookup"><span data-stu-id="c9082-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="c9082-103">**AIP 스캐너를 설치하려면 다음 권장 지침을 따릅니다.**</span><span class="sxs-lookup"><span data-stu-id="c9082-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="c9082-104">새로 설치 대신 업그레이드를 하는 경우, [Azure Information Protection 스캐너 업그레이드](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) 지침을 따르고, 통합 레이블 클라이언트의 경우, [Azure Information Protection 스캐너 업그레이드](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c9082-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="c9082-105">전체 [방화벽 및 네트워크 인프라 설정 요구 사항](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)을 준수하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="c9082-106">자동 레이블에 맞게 [정책이 설정되었거나](https://docs.microsoft.com/azure/information-protection/configure-policy) 정책에 기본 레이블이 설정되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="c9082-107">[Azure Information Protection 클라이언트가 지원하는 파일 형식](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)에 설명된 대로 관련 파일 형식이 레이블/보호를 위해 구성되어 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="c9082-108">또한, 기본 동작을 변경하고자 할 경우, 다음과 같은 지침을 따르세요. [파일의 기본 보호 수준 변경](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="c9082-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="c9082-109">스캐너 서비스를 실행하도록 구성된 사용자 계정에 모든 구성 리포지토리를 액세스할 수 있는 권한이 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="c9082-110">문제가 계속 발생하는 경우 스캐너 로그를 내보내서 지원 티켓에 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="c9082-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="c9082-111">**Azure Information Protection 스캐너 로그 내보내기**</span><span class="sxs-lookup"><span data-stu-id="c9082-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="c9082-112">스캐너 서비스를 실행하는 사용자 컨텍스트 아래 %localappdata%\Microsoft\MSIP를 탐색합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="c9082-113">MSIP 폴더 아래에 모든 콘텐츠를 압축합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="c9082-114">원하는 위치에 로그를 저장하고 서비스 요청에 첨부합니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="c9082-115">[Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)를 사용할 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c9082-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="c9082-116">**자세한 내용은 다음을 참조하세요**.</span><span class="sxs-lookup"><span data-stu-id="c9082-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="c9082-117">파일을 자동으로 분류하고 보호하는 Azure Information Protection 스캐너 배포</span><span class="sxs-lookup"><span data-stu-id="c9082-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="c9082-118">Set-AIPAuthentication에 토큰 매개 변수 지정 및 사용</span><span class="sxs-lookup"><span data-stu-id="c9082-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="c9082-119">검색 주기 실행 및 스캐너용 보고서 보기</span><span class="sxs-lookup"><span data-stu-id="c9082-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="c9082-120">Azure Information Protection 설명서 검토</span><span class="sxs-lookup"><span data-stu-id="c9082-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c9082-121">Azure Information Protection 요구 사항</span><span class="sxs-lookup"><span data-stu-id="c9082-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="c9082-122">Azure Information Protection 클라이언트 다운로드</span><span class="sxs-lookup"><span data-stu-id="c9082-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
