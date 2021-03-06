---
title: 프로비전 서비스 구성
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480751"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="06b9a-102">프로비전 서비스 구성</span><span class="sxs-lookup"><span data-stu-id="06b9a-102">Configuring the Provision service</span></span>

<span data-ttu-id="06b9a-103">자동화된 사용자 프로비전이 작동하려면 Azure AD에 Workday 웹 서비스 API에 연결할 수 있는 유효한 자격 증명이 필요합니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="06b9a-104">또한 Workday에서 AD 사용자 프로비전 앱으로의 연결 테스트 단추는 AD 도메인과 연결된 Azure AD Connect 프로비저닝 에이전트에 연결할 수 있는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="06b9a-105">Azure Portal에서 자격 증명을 저장하면 오류가 반환되는 경우 아래 권장 단계를 따르세요.</span><span class="sxs-lookup"><span data-stu-id="06b9a-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="06b9a-106">자습서 섹션 Workday에서 통합 시스템 사용자 구성 섹션에 설명된 Workday 통합 시스템 사용자 계정을 [구성해야 합니다.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="06b9a-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="06b9a-107">서비스 관리 콘솔을 사용하여 Azure AD Connect 프로비저닝 에이전트 서비스가 실행 중인지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="06b9a-108">Azure Portal에서 에이전트의 상태를 확인하려면 On-premises agents(Azure Portal 에이전트 보기) 단추를 클릭하여 상태를 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="06b9a-109">"Workday Username" 필드의 값을 테넌트-username@workday 입력해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="06b9a-110">workday-tenant-name이 없는 경우 Workday 인증이 실패합니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="06b9a-111">Workday 구현 테넌트와의 통합을 구성하는 경우 Workday 테넌트의 예약된 다운타임 시간을 유의합니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="06b9a-112">Workday는 주말(일반적으로 금요일 오후부터 토요일 오전까지)에 구현 테넌트에 대한 작동 종료 시간을 예약하고, 이 작동 시간 기간 동안의 연결 실패는 구현 테넌트가 다시 온라인 상태인 즉시 자동 해결된 알려진 문제입니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="06b9a-113">드물지만 테넌트 새로 고침으로 인해 통합 시스템 사용자의 암호가 변경되었거나 계정이 잠겨되었거나 만료된 상태인 경우 이 오류가 표시될 수도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="06b9a-114">Workday 관리자와 통합 시스템 사용자의 상태를 확인하시기 바랍니다.</span><span class="sxs-lookup"><span data-stu-id="06b9a-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="06b9a-115">자동화된 프로비전을 위해 작업일을 구성하는 방법에 대한 자세한 내용은 자습서: 자동 사용자 프로비전을 위한 [Workday 구성을 참조합니다.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="06b9a-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
