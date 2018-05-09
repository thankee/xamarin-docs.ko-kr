---
title: Xamarin.Essentials 응용 프로그램 정보
description: AppInfo 클래스는 응용 프로그램에 대 한 정보를 제공합니다.
ms.assetid: 15924FCB-19E0-45B2-944E-E94FD7AE12FA
ms.technology: xamarin-crossplatform
author: jamesmontemagno
ms.author: jamont
ms.date: 05/04/2018
ms.openlocfilehash: 5b235fdeb666c3f8f2c1b52a9691c931724ce2b8
ms.sourcegitcommit: 46d3c9daa45350bdd536d9e105517f3c1c753c5b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/07/2018
---
# <a name="xamarinessentials-app-information"></a>Xamarin.Essentials 응용 프로그램 정보

![시험판 NuGet](~/media/shared/pre-release.png)

**AppInfo** 클래스 응용 프로그램에 대 한 정보를 제공 합니다.

## <a name="using-appinfo"></a>AppInfo를 사용 하 여

클래스에 Xamarin.Essentials에 대 한 참조를 추가 합니다.

```csharp
using Xamarin.Essentials;
```

다음 정보는 API를 통해 노출 됩니다.

```csharp
// Application Name
var appName = AppInfo.Name;

// Package Name/Application Identifier (com.microsoft.testapp)
var packageName = AppInfo.PackageName;

// Application Version (1.0.0)
var version = AppInfo.VersionString;

// Application Build Number (1)
var build = AppInfo.BuildString;
```

## <a name="api"></a>API

- [AppInfo 소스 코드](https://github.com/xamarin/Essentials/tree/master/Essentials/AppInfo)
- [AppInfo API 설명서](xref:Xamarin.Essentials.AppInfo)