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
# <a name="configuring-the-provision-service"></a>프로비전 서비스 구성

자동화된 사용자 프로비전이 작동하려면 Azure AD에 Workday 웹 서비스 API에 연결할 수 있는 유효한 자격 증명이 필요합니다. 또한 Workday에서 AD 사용자 프로비전 앱으로의 연결 테스트 단추는 AD 도메인과 연결된 Azure AD Connect 프로비저닝 에이전트에 연결할 수 있는지 확인합니다.

Azure Portal에서 자격 증명을 저장하면 오류가 반환되는 경우 아래 권장 단계를 따르세요.

1. 자습서 섹션 Workday에서 통합 시스템 사용자 구성 섹션에 설명된 Workday 통합 시스템 사용자 계정을 [구성해야 합니다.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. 서비스 관리 콘솔을 사용하여 Azure AD Connect 프로비저닝 에이전트 서비스가 실행 중인지 확인합니다. Azure Portal에서 에이전트의 상태를 확인하려면 On-premises agents(Azure Portal 에이전트 보기) 단추를 클릭하여 상태를 확인할 수 있습니다.
3. "Workday Username" 필드의 값을 테넌트-username@workday 입력해야 합니다. workday-tenant-name이 없는 경우 Workday 인증이 실패합니다.
4. Workday 구현 테넌트와의 통합을 구성하는 경우 Workday 테넌트의 예약된 다운타임 시간을 유의합니다. Workday는 주말(일반적으로 금요일 오후부터 토요일 오전까지)에 구현 테넌트에 대한 작동 종료 시간을 예약하고, 이 작동 시간 기간 동안의 연결 실패는 구현 테넌트가 다시 온라인 상태인 즉시 자동 해결된 알려진 문제입니다.
5. 드물지만 테넌트 새로 고침으로 인해 통합 시스템 사용자의 암호가 변경되었거나 계정이 잠겨되었거나 만료된 상태인 경우 이 오류가 표시될 수도 있습니다. Workday 관리자와 통합 시스템 사용자의 상태를 확인하시기 바랍니다.

자동화된 프로비전을 위해 작업일을 구성하는 방법에 대한 자세한 내용은 자습서: 자동 사용자 프로비전을 위한 [Workday 구성을 참조합니다.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
