---
title: 하위 도메인 추가
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475985"
---
# <a name="adding-a-sub-domain"></a>하위 도메인 추가

하위 도메인은 상위 도메인과 동일한 테넌트 또는 다른 테넌트에 추가할 수 있습니다. 두 경우 모두 등록 기관의 웹 사이트에서 자체 DNS 설정을 관리해야 합니다. Microsoft에서 NS 레코드를 사용하여 DNS 설정을 관리하게 했거나 Microsoft에서 도메인을 구입한 경우 먼저 변경하지 않고 하위 도메인을 추가할 수 없습니다.

상위 도메인을 먼저 추가한 다음 하위 도메인을 추가합니다. 하위omain이 동일한 테넌트에 있는 경우 추가 확인이 필요하지 않습니다. 하위 도메인을 별도의 테넌트에 추가하는 경우 선택한 서비스에 대한 도메인 및 추가 DNS 레코드를 추가하기 전에 소유권 확인을 위해 DNS txt 레코드가 필요합니다.

- 도메인 또는 하위 도메인을 추가하려면 [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)도메인 추가 마법사 를 따르거나 도메인 추가 도메인 설정으로 하여 수동으로 도메인 또는 하위 도메인을  >    >  **추가합니다.**

필요한 경우:

- 기존 도메인에 대한 DNS 설정을 관리하는 사용자 변경하려면 설정 도메인으로 이동하여 도메인 **옆의** 확인란을 선택한 다음 DNS 관리를  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **선택합니다.** 마법사에서 자체 **DNS 레코드** 추가를 선택하고 마법사를 완료합니다.
- Microsoft에서 구입한 도메인에 하위 도메인을 추가하려면 먼저 도메인을 다른 등록 기관으로 전송한 다음 위의 변경을 통해 자체 DNS 레코드를 관리합니다. 자세한 내용은 [Microsoft에서 다른 호스트로 도메인 전송을 참조하세요.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- 조직의 다른 구성원이나 사용자가 도메인을 이미 사용하고 있는 경우 도메인을 사용하기 전에 먼저 관리되지 않는 계정을 대신해야 합니다. 자세한 내용은 [에서 관리되지](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)않는 디렉터리를 관리자 권한으로 Azure Active Directory.
