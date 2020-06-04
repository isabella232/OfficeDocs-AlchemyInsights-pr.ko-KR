---
title: AIP 레이블 정책 만들기
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542132"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="a7719-102">AIP 레이블 정책 만들기</span><span class="sxs-lookup"><span data-stu-id="a7719-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="a7719-103">AIP (Azure Information Protection) 레이블은 조직에서 일반적으로 개인 데이터의 가장 낮은 분류에서 높은 기밀 데이터를 분류 하는 데 사용 하는 전체 데이터 범위와 함께 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a7719-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="a7719-104">Azure Information Protection 정책은 [aip](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)(Azure information protection) 클래식 클라이언트에 적용 되 고 이러한 클라이언트에는 해당 정보가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="a7719-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="a7719-105">다음과 같은 옵션을 포함 하 여 AIP 정책에서 여러 요소를 구성할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="a7719-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="a7719-106">관리자 또는 사용자 분류 및 보호 (선택 사항) 문서 및 전자 메일을 허용 하는 레이블을 지정 하는 옵션</span><span class="sxs-lookup"><span data-stu-id="a7719-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="a7719-107">사용자가 문서를 저장 하 고 전자 메일을 보낼 때 분류를 적용 하는 옵션</span><span class="sxs-lookup"><span data-stu-id="a7719-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="a7719-108">전자 메일 메시지에 첨부 파일을 사용 하 여 자동으로 레이블을 지정 하는 옵션입니다.</span><span class="sxs-lookup"><span data-stu-id="a7719-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="a7719-109">Office 응용 프로그램에 정보 보호 표시줄을 표시할지 여부를 제어 하는 옵션</span><span class="sxs-lookup"><span data-stu-id="a7719-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="a7719-110">Azure Information Protection 정책에 대 한 추가 옵션 및 정보는 [Azure Information protection Policy 개요](https://docs.microsoft.com/azure/information-protection/overview-policy)를 참조 하세요.</span><span class="sxs-lookup"><span data-stu-id="a7719-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="a7719-111">기타 IP 정책과 관련 된 기타 유용한 리소스에 대해서는 다음을 참조 하십시오.</span><span class="sxs-lookup"><span data-stu-id="a7719-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="a7719-112">자습서: Azure Information Protection 정책 설정을 구성 하 고 새 레이블을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="a7719-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a7719-113">Azure Information Protection 정책 구성</span><span class="sxs-lookup"><span data-stu-id="a7719-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="a7719-114">민감도 레이블과 해당 정책 생성 및 구성</span><span class="sxs-lookup"><span data-stu-id="a7719-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="a7719-115">Azure Information Protection을 사용 하는 일반적인 시나리오에 대 한 방법 가이드</span><span class="sxs-lookup"><span data-stu-id="a7719-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="a7719-116">Azure Information Protection 설명서 검토</span><span class="sxs-lookup"><span data-stu-id="a7719-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="a7719-117">Azure Information Protection에 대 한 요구 사항</span><span class="sxs-lookup"><span data-stu-id="a7719-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="a7719-118">Azure Information Protection에 대 한 빠른 시작 자습서</span><span class="sxs-lookup"><span data-stu-id="a7719-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="a7719-119">Azure Information Protection 클라이언트 다운로드</span><span class="sxs-lookup"><span data-stu-id="a7719-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)