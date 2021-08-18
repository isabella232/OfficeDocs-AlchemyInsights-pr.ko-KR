---
title: 오류 코드 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: RDS(원격 데스크톱 서비스) 배포에서 Office 2013을 활성화하는 동안 오류가 발생하는 경우 레지스트리를 편집하여 ADAL을 사용하도록 설정하는 것이 좋습니다.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316692"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>원격 데스크톱 서비스에서 Office 2013을 활성화하는 동안 오류가 발생했습니다.

RDS(원격 데스크톱 서비스) 배포에서 Office 2013을 활성화하는 동안 오류가 발생하는 경우 레지스트리를 편집하여 ADAL을 사용하도록 설정하는 것이 좋습니다.
  
|**레지스트리 키**|**유형**|**값**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

자세한 내용은 모바일 장치에서 [Office 2013에](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)대해 최신 인증 Windows 참조하세요.
  
**참고:** ADAL은 2016 및 엔터프라이즈용 Microsoft 365 앱 Office 사용하도록 설정되어 있습니다. RDS(원격 데스크톱 서비스)의 이름은 이전에 터미널 서비스입니다.
  