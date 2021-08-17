---
title: 테넌트 정책 수정(작업 오버라이드)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896081"
---
# <a name="fix-tenant-policy-action-override"></a>테넌트 정책 수정(작업 오버라이드)

스팸 방지 정책 중 하나에서 이 메시지에 영향을 주었다. 정책을 검토하기 위해 다음 단계를 수행합니다.

1. 의 Microsoft 365 Defender 포털에서 전자 메일 & 공동 작업 정책 & 규칙 위협 정책 스팸 방지 <https://security.microsoft.com/>  \>  \>  \>  **섹션으로** 이동하세요.

   **스팸 방지 정책** 페이지로 직접 이동하려면 <https://security.microsoft.com/antispam>을(를) 사용합니다.

2. 스팸 **방지** 정책 페이지에서 정책의 이름을 클릭하여 정책을 선택합니다.**유형은** **사용자** 지정 스팸 방지 정책 또는 **이름은** 스팸 방지 인바운드 **정책(기본값)입니다.**
3. 세부 정보 플라이아웃이 나타나면  작업 섹션에서 작업 **편집을** 선택합니다.
4. 메시지 **작업 섹션에서** **스팸,** 높은 지수 **스팸,** 피싱 및  높은 지수 피싱에 대한 결과를 검토하여 다음 값 중 어느 것이 선택되어 있는지 검토합니다. 
   - **X-헤더 추가**   지정한 받는 사람에게 메시지를 보내되 해당 메시지를 스팸으로 식별하는 X-헤더 텍스트를 메시지 헤더에 추가합니다.
   - **제목 줄에 텍스트 추가**
   - **전자 메일 주소로 메시지 리디렉션**
   - **메시지 삭제**
   - **작업 없음**

   고객이 메시지에 영향을  주면 모든 Exchange Online Protection 표준 설정이 적용될 수 있습니다.

자세한 내용은 [EOP에서 스팸 방지 정책 구성하기](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)를 참조하세요.
