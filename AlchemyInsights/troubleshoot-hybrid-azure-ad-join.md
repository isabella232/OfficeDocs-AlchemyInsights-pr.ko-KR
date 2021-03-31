---
title: 하이브리드 Azure AD 가입 문제 해결
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401913"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="aa288-102">하이브리드 Azure AD 가입 문제 해결</span><span class="sxs-lookup"><span data-stu-id="aa288-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="aa288-103">[장치 등록 연결 테스트 스크립트](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)를 사용하여 장치가 시스템 계정 아래의 장치 등록 엔드포인트에 액세스할 수 있는지 확인하는 것을 적극 권장합니다.</span><span class="sxs-lookup"><span data-stu-id="aa288-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="aa288-104">장치 등록을 처음 설정하는 경우 [Azure Active Directory에서 장치 관리 소개](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)를 검토하여 Azure AD의 제어 하에 장치를 가져오는 방법에 대해 알아보세요.</span><span class="sxs-lookup"><span data-stu-id="aa288-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="aa288-105">장치를 Azure AD에 직접 등록하고 Intune에 등록하는 경우 [Intune을 구성](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)하고 [라이선스](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)를 먼저 확보해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aa288-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="aa288-106">Azure AD 및 온-프레미스 AD에서 작업을 수행할 권한이 부여되어 있는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="aa288-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="aa288-107">Azure AD의 전역 관리자만 장치 등록 설정을 관리할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="aa288-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="aa288-108">또한, 온-프레미스 Active Directory에서 자동 등록을 설정하는 경우 Active Directory 및 AD FS의 관리자(해당하는 경우)에게 문의해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="aa288-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="aa288-109">하이브리드 조인에서 발생할 수 있는 문제를 해결하는 방법에 대한 자세한 내용은 [하이브리드 조인 문제 해결](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)을 참조하십시오. 하이브리드 Azure AD 가입 및 Azure Ad Portal을 사용하여 장치 관리를 설정하려면 [하이브리드 Azure AD 조인(온-프레미스 도메인 조인) 장치 설정](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) 및 [Azure 포털을 사용하여 장치 관리](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)를 참조하십시오.</span><span class="sxs-lookup"><span data-stu-id="aa288-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="aa288-110">하이브리드 Azure AD (Active Directory) 가입과 관련된 일반적인 문제를 해결 하려면 [하이브리드 Azure AD 가입 FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="aa288-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
