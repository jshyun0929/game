# WOLF RPG 실기기 구동 테스트

대상은 갤럭시 S23+와 WOLF RPG Editor 3.737의 공식 샘플입니다. 샘플의 `Game.exe`는 Windows x86 32비트이며 같은 폴더에 `Data`가 있습니다.

## 갤럭시 테스트

1. [공식 샘플 ZIP](https://www.silversecond.com/WolfRPGEditor/Data/WolfRPGEditor_3.737.zip)을 내려받습니다. 갤럭시 내 파일에서 압축을 풀고 `Game.exe`와 `Data`가 들어 있는 `WOLF_RPG_Editor3` 폴더를 내부 저장소의 Download 폴더에 둡니다.
2. [Winlator 11.2 공식 APK](https://github.com/brunodev85/winlator/releases/download/v11.2.0/Winlator_11.2.apk)를 설치하고 초기 설정이 끝날 때까지 기다립니다.
3. Winlator에서 기본 설정으로 컨테이너를 하나 만든 뒤 실행합니다. 파일 탐색기에서 `D:\\WOLF_RPG_Editor3\\Game.exe`를 엽니다. 기본 컨테이너의 D: 드라이브는 Download 폴더입니다.
4. 타이틀 화면이 뜨면 Winlator의 화면 키보드나 입력 컨트롤에서 방향키와 Enter를 눌러 화면이 반응하는지 확인합니다. 실패하면 보이는 오류나 멈춘 화면을 캡처합니다.

## 현재 확인한 범위

클라우드 Linux에서는 Wine 11.22 WoW64로 64비트 메모장 창을 확인했지만, 32비트 시작 과정은 실패했습니다. 이 환경에서 간단한 네이티브 x86 Linux 실행 파일도 기동할 수 없었습니다. 이 결과로 S23+의 Wine·Box64 동작 여부를 판정할 수 없습니다.

Winlator 11.2의 게임 화면 액티비티는 외부 앱 호출을 허용하지 않습니다. 위 테스트는 휴대폰에서 실제 게임과 키 입력의 호환성을 먼저 확인하는 절차입니다. 울프 RPG APK에 Windows 실행 엔진은 아직 포함되어 있지 않습니다.
