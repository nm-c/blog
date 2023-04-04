---
title: "NuPhy Air60 사용자를 위한 home, end, page up/down key mapping"
header:
  overlay_image: https://source.unsplash.com/random?NuPhy%20Air60
tagline:
description: "NuPhy Air60 키보드 사용자를 위한 home, end, page up 및 page down key mapping 방법을 소개하는 글입니다."
tags: [NuPhy Air60, key mapping, AutoHotkey, home, end, page up, page down, 키보드]
---

## 서론

NuPhy Air60 키보드는 작고 가벼운 기계식 키보드로 크기와 무게를 줄이면서도 성능을 유지하는 데 성공했습니다. 여러 무선 연결 옵션과 유선 연결을 지원하여 사용자들에게 다양한 사용 환경에서의 편리함을 제공합니다. 하지만 이 키보드의 컴팩트한 디자인과 기본 키 배치로 인해 home, end, page up 및 page down 키를 사용할 수 없습니다. 대부분의 작은 키보드들은 fn + 방향키로 해당 기능을 구현하는데 NuPhy Air60의 경우는 그렇지 않습니다. 제조사에서 제공하는 NuPhy Console에도 키 조합으로 다른 키를 mapping하는 기능은 포함되어 있지 않습니다. 이로 인해 일부 사용자들은 생산성이 저하되거나 불편함을 느끼게 됩니다. 본 글에서는 key mapping을 통해 NuPhy Air60 키보드의 이러한 문제를 해결하고 사용자들이 원활하게 작업을 수행할 수 있도록 돕는 방법을 소개합니다. 이를 통해 NuPhy Air60 키보드 사용자들이 기본 제공 기능 외에도 home, end, page up 및 page down 키를 활용하여 생산성을 높일 수 있습니다.

## AutoHotkey 소개

AutoHotkey는 사용자가 키보드, 마우스 및 조이스틱 입력을 매크로, 스크립트 또는 핫키로 매핑할 수 있게 해주는 오픈소스 스크립팅 프로그램입니다. 이를 사용하여 NuPhy Air60 키보드의 key mapping을 변경할 수 있습니다.

## home, end, page up, page down 키 설정 방법

다음은 예제 코드와 설정 방법에 대한 단계별 설명입니다.

```ahk
^Left::Home
^Right::End
^Up::PgUp
^Down::PgDn
```

텍스트 편집기 (예: 메모장)를 열고 위의 코드를 붙여넣습니다.
파일을 .ahk 확장자를 사용하여 저장합니다 (예: remap_keys.ahk).
저장한 .ahk 파일을 더블 클릭하여 실행합니다. AutoHotkey가 설치되어 있어야 합니다.
이제 Ctrl + 왼쪽 화살표를 누르면 Home 키가 동작하고, Ctrl + 오른쪽 화살표를 누르면 End 키가 동작합니다. 또한 Ctrl + 위 화살표를 누르면 Page Up이 동작하고, Ctrl + 아래 화살표를 누르면 Page Down이 동작합니다.

## Windows 시작 시 스크립트 자동 실행 설정

1. 작성한 .ahk 파일을 찾아서 마우스 오른쪽 버튼으로 클릭한 후 "바로 가기 만들기(Create shortcut)"를 선택하여 바로 가기를 생성합니다.

1. 바로 가기를 복사하거나 잘라내기(Cut)합니다.

1. Windows 탐색기에서 주소 표시줄에 다음 경로 중 하나를 입력하고 Enter 키를 누릅니다.

    - Windows 10, Windows 8, Windows 7 및 Windows Vista의 경우:

        ```
        %APPDATA%\Microsoft\Windows\Start Menu\Programs\Startup
        ```

   - Windows XP의 경우:

        ```
        %USERPROFILE%\Start Menu\Programs\Startup
        ```

1. 탐색기 창이 열리면 마우스 오른쪽 버튼을 클릭하고 "붙여넣기(Paste)"를 선택하여 복사한 바로 가기를 붙여넣습니다.

이제 Windows가 시작될 때마다 해당 .ahk 파일이 자동으로 실행됩니다. 이렇게 하면 매번 수동으로 스크립트를 실행할 필요가 없습니다.

## 결론

NuPhy Air60 키보드 사용자를 위한 home, end, page up 및 page down key mapping을 통해 생산성을 향상시킬 수 있습니다. 본 글에서 소개한 방법을 따라 설정하면, 이 키보드를 사용하는데 있어 더욱 편리함을 누릴 수 있습니다. 추가적인 팁 및 참고 자료는 AutoHotkey 공식 문서에서 확인하실 수 있습니다.