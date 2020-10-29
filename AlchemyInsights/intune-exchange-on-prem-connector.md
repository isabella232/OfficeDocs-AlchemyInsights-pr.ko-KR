---
title: Intune Exchange 온-프레미스 커넥터
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791522"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange 온-프레미스 커넥터

Intune과 온-프레미스에 호스트 되는 Exchange 사이에 커넥터를 설정 하는 방법에 대 한 자세한 내용은 다음 설명서를 참조 하세요.

[Microsoft Intune Azure에서 Intune 온-프레미스 Exchange 커넥터 설정](https://docs.microsoft.com/intune/exchange-connector-install)

**자주 묻는 질문(FAQ):**

Q: Exchange connector를 설정 하려고 할 때 "Exchange Connector 버전이 지원 되지 않습니다."와 같은 오류가 표시 됩니다. 원인은 무엇 인가요?

A: 사용 중인 계정에 적절 한 라이선스가 부여 된 경우-활성 Intune 라이선스가 있어야 합니다.

Q: 여러 Exchange 커넥터를 사용할 수 있나요?

A: exchange 조직 당 Intune 테 넌 트 당 하나의 Exchange 커넥터만 설정할 수 있습니다. 커넥터는 다중 서버 exchange 조직의 한 서버에만 설치할 수 있습니다.

또한 같은 테 넌 트에서 구성 된 Exchange 온-프레미스 및 Exchange Online 모두에 대해 커넥터를 구성할 수 없습니다.

Q: 커넥터가 CAS 배열을 Exchange 연결로 사용할 수 있나요?

A: CAS 배열을 지정 하는 것은 커넥터 설정에서 지원 되지 않는 구성입니다. 단일 서버만 지정 해야 하며, 다음 위치에서 찾을 수 있는 커넥터 구성 파일에 하드 코드 되어야 합니다.

온-프레미스 Exchange 커넥터에 data\microsoft\microsoft Intune 프로그램 \ OnpremiseExchangeConnectorServiceConfiguration.xml

다음 항목을 찾아 ```<ExchangeWebServiceURL />``` URL을 exchange 서버로 바꿉니다.

**예에서**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

추가 문제 해결 방법은 다음 설명서를 참조 하세요. [Intune 온-프레미스 Exchange Connector 문제 해결](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Exchange 커넥터에 대해 자세한 정보 표시 로깅 사용**

1. Exchange Connector 추적 구성 파일을 편집용으로 엽니다.  
파일 은%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml에 있습니다.  

**예에서**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. 다음 키를 사용 하 여 TraceSourceLine를 찾습니다. OnPremisesExchangeConnectorService  
  
3. 정보 ActivityTracing (기본값)에서 SourceLevel node 값을 자세한 ActivityTracing로 변경 합니다.  

**예제:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Microsoft Intune Exchange 서비스 다시 시작  
5. Intune 포털에서 전체 동기화-완료 된 다음 XML을 다시 "Information ActivityTracing"로 변경 하 고 Microsoft Intune Exchange 서비스를 다시 시작 합니다.  
6. 로그 위치는 다음과 같습니다. `%ProgramData%\Microsoft\Windows Intune Exchange Connector`