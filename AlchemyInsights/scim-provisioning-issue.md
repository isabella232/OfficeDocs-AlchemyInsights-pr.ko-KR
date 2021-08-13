---
title: SCIM 프로비전 문제
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: dc2068bbfde7b633e75b3d42f597cee8e4e5f5a72fbf22ebd6c2d0b768945dc9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061654"
---
# <a name="scim-provisioning-issue"></a>SCIM 프로비전 문제

자동 프로비전은 사용자가 액세스해야 하는 클라우드 응용 프로그램에서 사용자 ID 및 역할을 만드는 것을 말합니다. 사용자 ID를 만드는 것 외에, 자동 프로비전에는 상태 또는 역할이 변경될 때 사용자 ID의 유지 관리와 제거가 포함됩니다. 배포를 시작하기 전에 먼저 [프로비전 작동 방식](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)을 검토하여Azure AD(Active Directory) 프로비전 작동 방식에 대해 알아보고 구성 권장 사항을 확인할 수 있습니다.

응용 프로그램 개발자는 SCIM(System for Cross-Domain Identity Management) 사용자 관리 API를 사용하여 응용 프로그램과 Azure AD 간에 사용자 및 그룹을 자동으로 프로비전할 수 있습니다. [SCIM 엔드포인트 빌드 및 Azure AD를 사용하여 사용자 프로비전 구성](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) 문서에서는 SCIM 엔드포인트를 빌드하고 Azure AD 프로비전 서비스에 통합하는 방법을 설명합니다.



