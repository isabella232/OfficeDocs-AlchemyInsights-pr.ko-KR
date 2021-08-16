---
title: GPO 배포
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067846"
---
# <a name="gpo-deployment"></a>GPO 배포

Azure AD DS(Azure Active Directory Domain Services)의 사용자 및 컴퓨터 개체에 대한 설정은 일반적으로 GPOS(그룹 정책 개체)를 사용하여 관리됩니다. Azure AD DS에는 AADDC 사용자 및 AADDC 컴퓨터 컨테이너에 대한 기본 제공 GPOS가 포함되어 있습니다. 필요에 따라 이러한 기본 제공 GPOS를 사용자 지정하여 환경에 맞게 그룹 정책을 구성할 수 있습니다. Azure AD DC 관리자 그룹의 구성원은 Azure AD DS 도메인의 그룹 정책 관리 권한을 가지며 사용자 지정 GPOS 및 OUS(조직 단위)를 만들 수도 있습니다. 그룹 정책의 기능 및 작동 방식에 대한 자세한 내용은 그룹 정책 개요 [를 참조하세요.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

하이브리드 환경에서는 온-프레미스 AD DS 환경에서 구성된 그룹 정책이 Azure AD DS와 동기화되지 않습니다. Azure AD DS의 사용자 또는 컴퓨터에 대한 구성 설정을 정의하려면 기본 GPO 중 하나를 편집하거나 사용자 지정 GPO를 만들 수 있습니다.

이 [그룹 정책 관리](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) 문서는 그룹 정책 관리 도구를 설치하는 방법, 기본 제공 GOS를 편집하는 방법 및 사용자 지정 GOS를 만드는 방법을 보여줍니다.
