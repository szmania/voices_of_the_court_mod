# 자주 묻는 질문

## 1. 대화창이 뜨지 않습니다
이 모드를 실행하려면 추가 백엔드 프로그램이 필요합니다. 여기에서 현지화된 백엔드 프로그램을 다운로드하세요: [https://github.com/szmania/Voices_of_the_Court/releases/latest](https://github.com/szmania/Voices_of_the_Court/releases/latest). 다운로드한 .exe 파일은 실행 시 자동으로 설치됩니다.

## 2. API 설정 문제
공식 DeepSeek API 사용을 권장합니다. 대화 모델 연결 드롭다운 메뉴에서 `custom(openai-compatible)` 페이지를 선택하여 다음과 같이 설정하세요:
- 서버 URL: `https://api.deepseek.com/beta`
- API 키: [https://platform.deepseek.com](https://platform.deepseek.com)에서 신청한 본인의 API 키를 입력하세요.

OpenAI 및 OpenRouter도 호환될 것입니다.

## 3. 설치 후 백엔드 프로그램이 실행 중인데도 대화창이 뜨지 않습니다
**해결책**: 현지화 모드를 사용해야 합니다.

설치 방법 (택일):
1. 다운로드한 현지화 모드 파일의 압축을 푼 후, Steam Workshop 디렉토리의 원본 모드 파일에 직접 덮어씁니다.
2. 압축을 푼 모드 폴더 `voices_of_the_court_mod-1.2.1-beta`를 게임의 모드 폴더에 넣습니다. 그런 다음 메모장을 사용하여 `Documents\Paradox Interactive\Crusader Kings III\mod` 폴더에 `voices_of_the_court_mod-1.2.1-beta.mod`라는 이름의 새 파일을 만들고 다음 내용을 입력합니다:
version="1.0"
tags={
"Gameplay"
}
name="Voices of the Court mcc"
supported_version="1.13.1"
path="C:/Users/ [사용자 PC 이름] / Documents/Paradox Interactive/Crusader Kings III/mod/voices_of_the_court_mod-1.2.1-beta"

현지화 모드를 설치하고 활성화했는데도 대화창이 나타나지 않는다면, CK3 사용자 폴더 경로가 잘못 설정되었거나 게임이 아이언맨 모드일 수 있습니다. 이 모드는 아이언맨 모드에서 작동하지 않습니다.

## 4. 채팅창을 열 때 빨간색 텍스트로 "TypeError: Cannot read properties of undefined (reading 'playerID')" 오류가 발생합니다
**해결책**: `Documents\Paradox Interactive\Crusader Kings III` 안에 `run`이라는 이름의 폴더를 만듭니다. 해당 폴더로 들어가 `votc.txt`라는 이름의 텍스트 파일을 만듭니다.

## 5. 캐릭터와 대화할 때 최근 기억이 읽히지 않습니다
**해결책**:
1. 이것은 원작자의 백엔드 프로그램에 있는 작은 버그입니다. 현지화된 백엔드를 다운로드하면 해결됩니다.
2. 메모리 토큰 제한 때문일 수도 있습니다. 백엔드 프로그램의 설정 페이지에서 `max memory tokens` 크기를 조정하세요. 메모리 토큰을 조정한 후에는 `max new tokens`도 늘려야 합니다. `max new tokens`가 `max memory tokens`보다 큰 것이 가장 좋습니다.

## 6. 백엔드 프로그램을 재시작하면 프롬프트 생성 스크립트가 초기화됩니다
**해결책**:
`custom` 폴더에 별도의 파일로 저장하세요.

Mod Name: Voices of the Court - Community Edition
License: GNU General Public License v3.0 (GPLv3)

Credits & Attribution
This project is a derivative work based on VOTC / AliChat. We would like to extend our deep gratitude to the developers who kept this project alive and pushed the boundaries of AI in Crusader Kings III:

Original Creators: The VOTC Team and community contributors.

Continued Development: Special thanks to the Chinese development community, including Lisiyuan233, zhaowendao2005, and others who provided critical updates and support.

Community Support: Thanks to Durond and MrAndroPC and the broader community for their insights and historical context regarding the project.

Licensing Information
Some of original source material for this mod was released under the Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) license.

In accordance with Section 4(b) of the CC BY-SA 4.0 license, this derivative work is being licensed under a BY-SA Compatible License: the GNU General Public License v3.0 (GPLv3).

Original License: CC BY-SA 4.0

Current License: GPLv3
