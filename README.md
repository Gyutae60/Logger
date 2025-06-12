
# Logger

## 개요

`Logger`는 C++로 작성된 모듈형 시스템으로, 다음과 같은 기능을 제공합니다:

- **카메라 모듈**: 실시간 카메라 데이터 캡처 및 처리
- **MQTT 모듈**: MQTT 프로토콜을 통한 메시지 송수신
- **객체 탐지 모듈**: 입력 데이터에 대한 객체 탐지
- **설정 관리**: `config.json`을 통해 설정 로드

## 프로젝트 구조

```
Logger/
├── camera/
│   ├── camera.cpp        # 카메라 관련 코드
│   ├── camera.h          # 카메라 헤더 파일
│   ├── create_cid.cpp    # CID 생성 코드
│   └── create_cid.h      # CID 헤더 파일
├── config/
│   ├── Config.cpp        # 설정 관련 코드
│   └── Config.h          # 설정 헤더 파일
├── Mqtt/
│   ├── Mqtt.cpp          # MQTT 관련 코드
│   └── Mqtt.h            # MQTT 헤더 파일
├── object_detection/
│   ├── object_detection.cpp  # 객체 탐지 코드
│   └── object_detection.h    # 객체 탐지 헤더 파일
├── result_data/
│   └── result_data.h     # 결과 데이터 형식
├── Logger.cpp            # 메인 진입점 코드
└── Makefile              # 빌드 스크립트
```

## 빌드 방법

1. `Logger` 디렉토리로 이동합니다.
   ```bash
   cd Logger
   ```
2. `make` 명령어로 빌드를 실행합니다.
   ```bash
   make
   ```

   빌드가 완료되면 실행 파일이 생성됩니다.

## 설정

- 설정 파일: `config.json` (프로젝트 루트에 위치)

## 사용 방법

1. `config.json` 파일을 적절하게 수정합니다.
2. `make` 명령어로 빌드를 수행합니다.
3. 빌드된 실행 파일을 실행합니다.

