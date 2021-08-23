---
title: 내 앱이 앱 거버넌스에 표시되지 않습니다.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/16/2021
ms.locfileid: "58362421"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>내 앱이 앱 거버넌스에 표시되지 않습니다.

응용 프로그램이 앱 거버넌스에 표시되지 않는 경우 다음을 검사합니다.

1. Azure [AD로 이동하고](https://aad.portal.azure.com/) 개요 페이지의 위쪽 표시줄에서 앱 이름을 검색하여 응용 프로그램의 앱 ID를 찾아 찾습니다.

1. Access Graph Explorer에서 이 쿼리를 사용하여 관련 앱 ID로 대체하여 서비스 사용자 내에서 앱 <appId> ID를 < https://graph.microsoft.com/v1.0/servicePrincipals? 검색합니다. $search= "appId: <appId> ">

1. 결과가 반환되지 않았다면 이 쿼리를 사용하여 관련 앱 ID로 바꾸어 응용 프로그램 내에서 앱 <appId> ID를 < https://graph.microsoft.com/v1.0/applications? 검색합니다. $search= "appId: <appId> ">

쿼리에 문제가 있는 경우 지원 [보기를 참조하세요.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

앱 거버넌스에서 앱에 대한 자세한 정보 또는 인사이트는 가시성 및 인사이트에 대한 자세한 [정보를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

앱을 보는 데 대한 자세한 내용은 앱 [보기를 참조하세요.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
