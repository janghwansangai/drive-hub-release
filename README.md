# Drive Hub 받기

여러 구글 계정(개인 Gmail + 학교·회사 계정)의 드라이브를 한 화면에서 공유하고, 공유 현황을 확인하고, 계정 사이에 파일을 복사·이동하는 **무료 데스크톱 앱**이에요.

> 이 저장소는 **설치 파일 배포용**이에요. 소스 코드는 공개하지 않아요.
> 안내 사이트: https://drive-hub-guide.pages.dev

## 받기

[Releases](../../releases/latest)에서 내 컴퓨터에 맞는 파일을 받으세요.

| 컴퓨터 | 파일 | 요구 사항 |
|---|---|---|
| macOS | `Drive-Hub-버전.dmg` | macOS 12 이상, 애플 실리콘·인텔 모두 |
| Windows | `Drive-Hub-Setup-버전.exe` | Windows 10·11 (64비트) |

받은 파일이 공식 파일인지는 릴리스 설명의 **SHA-256 지문**과 비교해 확인할 수 있어요.

```bash
shasum -a 256 Drive-Hub-0.1.0.dmg
```

```
certutil -hashfile Drive-Hub-Setup-0.1.0.exe SHA256
```

## 처음 열 때

개인이 무료로 만든 앱이라 유료 서명이 없어 처음 한 번만 허용이 필요해요.

- **맥**: `.dmg`를 열고 Drive Hub를 응용 프로그램 폴더로 끌어 놓기 → 열면 뜨는 경고는 **완료** → **시스템 설정 › 개인정보 보호 및 보안 › 그래도 열기**
- **윈도우**: “Windows의 PC 보호” 창에서 **추가 정보 → 실행**

## 처음 설정 (약 15분)

Drive Hub는 각자 **자기 Google Cloud 키**로 구글에 연결해요. 그래서 만든 사람을 포함해 누구도 내 드라이브에 접근할 수 없어요.
[그림으로 보는 키 만들기 안내](https://drive-hub-guide.pages.dev/desktop-setup)를 따라 하세요.

## 업데이트

새 버전이 나오면 앱이 알려 줘요. **받아서 설치하기 → 앱 닫고 설치하기**를 누르면 돼요.

## 개인정보 · 문의

- [개인정보 처리 안내](https://drive-hub-guide.pages.dev/privacy) — 앱은 내 정보를 모으지 않아요.
- 오류·제안: 앱 왼쪽 아래 **오류 신고**

만든 사람: 다있쌤 로디
