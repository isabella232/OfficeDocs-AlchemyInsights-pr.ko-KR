---
title: 액세스 거부 메시지 문제 해결
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505385"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive 관리 센터에서 액세스 거부 메시지 문제 해결

Sharepoint/OneDrive 관리 센터를 탐색 하려고 할 때 액세스 거부 메시지가 표시 되는 경우 [사용자에 게 라이선스를 할당](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)했는지 확인 하세요. 사용자에 게 라이선스가 있는 경우 관리 센터에 액세스할 수 있는 [관리자 역할이 할당](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) 되었는지도 확인 해야 합니다.

동일한 UPN (사용자 계정 이름)을 사용 하 여 삭제 하 고 다시 만든 경우에도이 문제가 발생할 수 있습니다. 새 계정은 다른 PUID (Passport 고유 ID) 값을 사용 하 여 만들어집니다. 사용자가 사이트 모음 또는 OneDrive에 액세스 하려고 하면 사용자에 게 잘못 된 PUID가 있습니다. 두 번째 시나리오에는 Active Directory OU (조직 구성 단위)와의 디렉터리 동기화가 포함 됩니다. 사용자가 이미 SharePoint에 로그인 한 후 다른 OU로 이동 하 고 SharePoint를 사용 하 여 resynced이 문제가 발생할 수 있습니다.

이 문제를 해결 하려면 [Microsoft 365에서 사용자 복원](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)문서의 단계와 함께 원래 UPN을 복원 해야 합니다.

참고: 이전에 액세스 한 여러 사용자가 OneDrive 또는 SharePoint 관리 센터를 사용할 수 없는 경우 일시적인 서비스 문제가 있을 수 있습니다.  [서비스 상태 대시보드를 확인](https://portal.office.com/adminportal/home#/servicehealth)합니다.


