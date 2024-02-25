---
title: "부록: OBS 연동"
weight: 100
---

다음 기능은 OBS 송출을 위해서 OBS용 Spout2 플러그인 설치가 필요합니다.

* {{< pagelink "/docs/plexchatbox/index.md" >}}

## 다운로드 및 설치

* [OBS Spout2 플러그인 릴리즈 페이지](https://github.com/Off-World-Live/obs-spout2-plugin/releases)에 접속합니다.
* 사용 중인 OBS 버전에 맞는 버전을 확인합니다.
    - 2024/02/26 시점에서 최신 버전의 OBS를 사용중이라면 OBS 29 플러그인과 호환됩니다.
* 플러그인 설치 전에 OBS가 실행 중이라면 OBS를 종료합니다.
    - OBS를 종료해야하기 떄문에 **송출 도중에 설치할 수 없습니다.**
* 이하 설명의 파일명은 **OBS 29 플러그인을 가정**하고 설명합니다. 실제 설치하는 시점의 최신 버전과 다를 수 있습니다.
    - 기본 경로에 OBS를 설치한 경우에는 [OBS_Spout2_plugin_Install_v1.8.exe](https://github.com/Off-World-Live/obs-spout2-plugin/releases/download/v1.8/OBS_Spout2_Plugin_Install_v1.8.exe) 파일을 다운로드하여 실행하면 설치가 완료됩니다.
    - 만약 OBS를 기본 경로가 아닌 다른 곳에 설치한 경우에는, [OBS_Spout2_Plugin_ManualInstall_v1.8.zip](https://github.com/Off-World-Live/obs-spout2-plugin/releases/download/v1.8/OBS_Spout2_Plugin_ManualInstall_v1.8.zip) 파일을 다운로드합니다. 압축을 해제하면 생기는 `data`와 `obs-plugins` 폴더 OBS가 설치된 폴더에 옮겨주면 설치가 완료됩니다.

## 플러그인 사용법

* 플러그인 설치 후 OBS를 실행하면 추가 가능한 소스 목록에 `Spout2 Capture` 항목이 추가됩니다.
* Spout 출력을 지원하는 프로그램이 켜진 상태에서 `Spout2 Capture` 소스를 추가합니다.
    - `SpoutSenders` 항목에서 불러올 항목을 선택합니다. 이름은 프로그램에 따라 다릅니다.
        - 플렉스트림 챗박스는 `PLEXChatBox/...` 형식의 이름을 사용합니다.
    - `Composite mode` 항목을 `Default`로 설정합니다.
* 정상적으로 OBS 화면에 출력되는 것을 확인합니다.
