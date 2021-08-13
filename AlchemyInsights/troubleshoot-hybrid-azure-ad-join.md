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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939277"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>하이브리드 Azure AD 가입 문제 해결

[장치 등록 연결 테스트 스크립트](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)를 사용하여 장치가 시스템 계정 아래의 장치 등록 엔드포인트에 액세스할 수 있는지 확인하는 것을 적극 권장합니다.

1. 장치 등록을 처음 설정하는 경우 [Azure Active Directory에서 장치 관리 소개](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)를 검토하여 Azure AD의 제어 하에 장치를 가져오는 방법에 대해 알아보세요.
1. 장치를 Azure AD에 직접 등록하고 Intune에 등록하는 경우 [Intune을 구성](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support)하고 [라이선스](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)를 먼저 확보해야 합니다.
1. Azure AD 및 온-프레미스 AD에서 작업을 수행할 권한이 부여되어 있는지 확인하세요. Azure AD의 전역 관리자만 장치 등록 설정을 관리할 수 있습니다. 또한, 온-프레미스 Active Directory에서 자동 등록을 설정하는 경우 Active Directory 및 AD FS의 관리자(해당하는 경우)에게 문의해야 합니다.

하이브리드 조인에서 발생할 수 있는 문제를 해결하는 방법에 대한 자세한 내용은 [하이브리드 조인 문제 해결](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)을 참조하십시오. 하이브리드 Azure AD 가입 및 Azure Ad Portal을 사용하여 장치 관리를 설정하려면 [하이브리드 Azure AD 조인(온-프레미스 도메인 조인) 장치 설정](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) 및 [Azure 포털을 사용하여 장치 관리](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)를 참조하십시오.

하이브리드 Azure AD (Active Directory) 가입과 관련된 일반적인 문제를 해결 하려면 [하이브리드 Azure AD 가입 FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)를 참조하세요.
