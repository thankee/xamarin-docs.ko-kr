---
title: 시기와 방법을 제출 해야 하나요 버그 보고서를?
description: 이 문서에서는 설명 하면 위치 및 버그 보고서를 파일에 있습니다. 또한 문제를 진단 하는 가장 하기 위해 엔지니어가 사용 하도록 설정 하는 모범 사례는 버그 보고서를 제공 합니다.
ms.topic: troubleshooting
ms.prod: xamarin
ms.assetid: 8AD9CFBF-282A-4C1F-95E9-25F21141B052
author: asb3993
ms.author: amburns
ms.date: 06/05/2018
ms.openlocfilehash: b70fe29a79e099f1141c1295d907b48afaa2c3c7
ms.sourcegitcommit: aa9b9b203ab4cd6a6b4fd51e27d865e2abf582c1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/30/2018
ms.locfileid: "39351608"
---
# <a name="when-and-how-should-i-file-a-bug-report"></a>시기와 방법을 제출 해야 하나요 버그 보고서를?

Xamarin의 Bugzilla 버그 추적기 여기에 버그: [ https://bugzilla.xamarin.com/enter_bug.cgi?classification=__all ](https://bugzilla.xamarin.com/enter_bug.cgi?classification=__all)합니다.

## <a name="file-a-bug-if"></a>경우에 버그를 신고 하는 중...

Xamarin 엔지니어 Xamarin에서 발생 하는 문제를 재현 하는 데 수를 생각 하는 단계 집합이 있습니다.

또는

문제와 관련 된 경우에 따라 정확 하 게도 설명할 수 있습니다 하는 경우에 특히 문제의 표시 증상을 신중 하 게 설명할 수 있습니다. <sup> [[1]](#note-1)</sup>


## <a name="best-practices-to-help-xamarin-address-bugs-quickly-and-efficiently"></a>빠르고 효율적으로 Xamarin 주소 버그 하는 데 유용한 정보


1. <a name="ref-1" />검색 [Bugzilla](https://bugzilla.xamarin.com/query.cgi?format=specific&amp;bug_status=__all__) 및 버그 보고서 또는 직접 문제를 해결할 수 있는 사용 제안 하는 기존 웹.<sup> [[2]](#note-2)</sup><sup>[[3]](#note-3)</sup>

1. <a name="ref-2" />수행 합니다 [지침을 작성 하는 버그](https://bugzilla.xamarin.com/page.cgi?id=bug-writing.html) 동작을 명확 하 고 가능한 한 간결 하 게 발생 한 내용과 된에 대 한 설명을 포함 하 여 예상 대로 문제를 설명 하 합니다.

1. <a name="ref-3" />충돌 로그 또는 모든 관련 된 스택 추적, 오류 메시지 텍스트 포함 됩니다. <sup>[[4]](#note-4)</sup>

1. <a name="ref-4" />모든 중요 한 나타나는 오류 메시지 스크린 샷 첨부 파일에 일반 텍스트로 너무 적어 둡니다.

1. <a name="ref-5" />가능 하면 코드를 적게 사용 하 여 버그를 재현 하는 소규모의 자체 포함 된 테스트 사례를 포함 합니다.  (기본 제공 템플릿 중 하나를 사용 하 여 만든) 새 프로젝트를 사용 하 여 문제를 재현할 수 없는 문제를 보여 주는 프로젝트를 압축 한 다음 고 버그 보고서에 연결 합니다.  연결 하기 전에 가능한 한 단순하게 예제 프로젝트를 확인 합니다. <sup> [[5]](#note-5)</sup><sup>[[6]](#note-6)</sup>

1. <a name="ref-6" />운영 체제를 포함 하 여, 버그가 발견 된 환경을 설명 하 고 [버전의 Xamarin](~/cross-platform/troubleshooting/questions/version-logs.md) 및 모든 종속성입니다.

---

## <a name="additional-details"></a>추가 세부 정보

1. <a name="note-1" />[*^*](#ref-1) 이상적으로 통해 "표시 증상" 설명은 다른 고객에 게 동일한 문제가 표시 되 고 있는지 여부를 확인할 수 있도록 충분 한 세부 정보를 포함 해야 (동일한 오류 메시지, 동일한 성능 저하, 충돌이 발생 한 동일한 스택 추적 _등입니다._ ). "정확한 경우" 좋은 예로 됩니다 하는 경우와 같이 말할 수 있습니다. "일반적으로 누르면 문제 75%의 시간, 하지만 한 가지 사항을 변경 하면 다음 방지할 수 있습니다 문제 완전히." "정확한 경우" 다른 비슷한 예는 Xamarin의 이전 버전으로 다운 그레이드 중지 문제입니다.

1. <a name="note-2" />[*^*](#ref-2) 짐작할 수 있겠지만 오류 텍스트 (또는 다른 고유 하 게 설명 텍스트)의 조각은 일반적으로 최상의 검색어입니다. 기존 버그 보고서를 완료 하는 경우 라면 세부 정보를 추가 하거나 새 파일을 더 잘 버그 보고서를 시작 합니다.

1. <a name="note-3" />[*^*](#ref-3) 또 다른 좋은 문제는 모든 Java에 대 한 동일한 문제를 보고 된 여부 Objective-c 또는 Swift 앱. 그렇다면 Xamarin의 일부가 아니라 가능성이 부분 Android 또는 iOS 자체 문제가입니다.

1. <a name="note-4" />[*^*](#ref-4) 몇 가지 정보를 포함 합니다.

    1. 프로젝트를 빌드할 때 발생 하는 오류 주십시오 전체에 대 한 [진단 빌드 출력](~/android/troubleshooting/troubleshooting.md#Diagnostic_MSBuild_Output) 버그 보고서입니다.
    
    1. 빌드 또는 Visual Studio에서 iOS 프로젝트를 디버깅 하는 경우 발생 하는 오류에 대 한 실행 하십시오 _도움말 > Xamarin > Zip 로그_ 후 오류에 도달 하 고 버그 보고서에 있는 결과.zip 파일을 포함 합니다.
    
    1. Android 또는 iOS 앱에서 충돌, 예외에 대 한 주십시오 관련 "[Xamarin.iOS 및 Xamarin.Android 앱에 대 한 로그 디버그](~/cross-platform/troubleshooting/questions/version-logs.md#debug-logs-for-xamarin-apps)."

1. <a name="note-5" />[*^*](#ref-5) 가능한 경우 특정 문제에 대 한 하나의 뛰어난 옵션은 원래 솔루션에서 새 솔루션으로 적은 수의 파일을 추가 하 여 문제가 다시입니다. Xamarin 팀 (재현 하는 단계는 명확 하 게 설명 가정), 더 큰 테스트 사례 하지만 최상의 버그를 빠르게 해결할 수는 변경 하는 간단한 테스트 사례 제공 에서도 문제를 조사할 수 경우가 많습니다.


1. <a name="note-6" />[*^*](#ref-6) 있으면 _되지_ 새로운 솔루션에 적은 수의 파일을 추가 하 여 문제를 재현할 수 다음 압축 하는 전체 앱에 대 한 전체 솔루션 폴더를 연결 합니다. 삭제 하십시오 합니다 `bin`, `obj`, `Components`, 및 `packages` 폴더를 zip 더 작은 파일을 확인 합니다. (IDE 및 빌드 프로세스는 일반적으로 복원 하거나 필요에 따라 이러한 폴더의 콘텐츠를 다시 만듭니다.) 또한 생성 되는 솔루션은 여전히 원래 문제를 보여주는으로 만큼 코드 및 리소스 파일 프로젝트에서 원하는 삭제할 수 있습니다.

