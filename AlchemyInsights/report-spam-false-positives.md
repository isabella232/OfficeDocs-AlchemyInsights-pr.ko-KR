---
title: Microsoft에 스팸 가짓 긍정을 보고하고자 하나요?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396621"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>정상적인 메시지가 스팸으로 표시되고 있나요?

합법적인 전자 메일이 정크 폴더나 정크 메일로 끝나면 좌절됩니다. 가짓 긍정의 가장 일반적인 원인을 고려합니다.

**테넌트 오버라이드(가장 일반적)** 이 컨트롤은 수정을 위해 완전히 컨트롤 내에 있습니다.

영향을 미치는 정책 및 Microsoft 365 Defender 분석을 위해 메시지 제출 rescan details are available within minutes.
적용 가능한 정책 또는 규칙을 검토하거나 수정합니다. 

**최종 사용자 오버라이드(일반)** 이 컨트롤은 수정을 위해 완전히 컨트롤 내에 있습니다. 

영향을 미치는 정책 및 Microsoft 365 Defender 분석을 위해 메시지 제출 rescan details are available within minutes. 

사용자의 수신이 차단된 보낸 사람 목록의 주소에서 보낸 메시지 때문에 메시지가 차단된 경우 헤더에 스팸 필터링 판정 "SFV:BLK"가 포함됩니다.

**보낸 사람 전자 메일 인증** 이 설정은 수정을 위해 컨트롤 내에 부분적으로 있습니다.

메시지를 제출하여 배달 시 보낸 사람 전자 메일 인증의 실패를 분석합니다. 결과는 하루 이내에 사용할 수 있습니다. 

전송 인프라를 소유하고 있는 경우 SPF, DKIM 및 DMARC에 맞추는 방법을 검토하여 대상 전자 메일 시스템이 도메인에서 보낸 메시지를 신뢰하는지 검토합니다. 또는 보낸 사람에 문의하여 DNS 구성에 대한 주소를 입력합니다.

**Microsoft 필터링 판정** 이 설정은 수정을 위해 컨트롤 내에 부분적으로 있습니다.

메시지를 제출하고 메시지를 안전한 것으로 보고합니다. rescan 결과는 하루 이내에 사용할 수 있습니다. 특정 상황에서 필터링 판정에 동의하지 않았다면 테넌트 허용/차단 목록을 사용하세요. 그러나 Microsoft 필터링 판정을 영구적으로 무시하면 안 됩니다. 

자세한 내용은 다음을 참조하세요.

- 최종 사용자가 Microsoft에 메시지를 제출할 수 있도록 합니다. Microsoft는 이러한 제출을 사용하여 전자 메일 보호 기술의 효율성을 개선하고 정책 업데이트 표시로 사용할 수 있는 제출 보고서에 표시됩니다. 

- 분석을 위해 메시지를 제출하는 데 대한 짧은 비디오를 시청하는 경우 [분석을 위해 메시지 제출을 참조합니다.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [관리자 제출을 사용하여 의심스러운 스팸, 피싱, URL 및 파일을 Microsoft에 제출](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [테넌트 허용/차단 목록 관리](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Microsoft 365의 스팸 방지 메시지 헤더](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [EOP의 아웃바운드 스팸 보호](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)