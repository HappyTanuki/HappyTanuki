정보보호 전공이고, C++로 시스템 가까운 쪽을 주로 다룹니다.
네트워킹, 암호화, 멀티스레딩처럼 직접 만들어봐야 이해가 되는 것들에 관심이 많아서
라이브러리를 쪼개 가며 구조를 잡아보는 작업을 하고 있습니다. 보안 개발도 같이 파는 중입니다.

### 요즘 하는 것

**BSED-Engine** — Browser Sandbox Escape Detection Engine의 코어입니다.
브라우저 샌드박스 탈출을 탐지하는 게 목표로, Windows ETW와 Sysmon 이벤트를
직접 파싱해서 관심 있는 프로바이더와 이벤트 ID만 골라낸 뒤, 이걸 노드 구조로
매핑하는 엔진을 만들고 있습니다. 원시 이벤트 파서, 노드 프로세서, DTO/리포지토리
분리 같은 구조를 잡아가는 중입니다. unX-0wn 조직에서 진행하는 비공개 프로젝트라
저장소는 아직 공개되어 있지 않습니다.

**Bedrock** — C++23 기반으로 직접 쓰고 있는 모듈형 라이브러리입니다.
Common, Encryption, Networking을 각각 별도 저장소로 분리해서 서브모듈로 묶었고,
CMake 프리셋과 PCH까지 정리해 빌드 구조를 다듬는 데 시간을 들이고 있습니다.
Windows에서는 ws2_32, crypt32 같은 시스템 라이브러리에 직접 붙입니다.

- [Bedrock](https://github.com/HappyTanuki/Bedrock) — 전체를 묶는 루트 프로젝트
- [Bedrock-Common](https://github.com/HappyTanuki/Bedrock-Common)
- [Bedrock-Encryption](https://github.com/HappyTanuki/Bedrock-Encryption)
- [Bedrock-Networking](https://github.com/HappyTanuki/Bedrock-Networking)
- [Bedrock-Threading](https://github.com/HappyTanuki/Bedrock-Threading)

**BumbleCee** — DPP로 만든 디스코드 음악 봇입니다.
링크나 제목으로 곡을 큐에 넣고 재생하는 기본 기능을 슬래시 커맨드로 구현했고,
오디오 처리는 FFmpeg, 다운로드는 yt-dlp를 씁니다. Docker 이미지로 배포합니다.
[저장소 보기](https://github.com/HappyTanuki/BumbleCee)

### 그 전에 했던 것

- [FileEncrypt](https://github.com/HappyTanuki/FileEncrypt) — 파일 암복호화와 검증을 하는 유틸리티
- [Asteroid](https://github.com/HappyTanuki/Asteroid) — 멀티플레이로 만들어 본 Asteroid
- [KISIA_API_study](https://github.com/HappyTanuki/KISIA_API_study) — KISIA S-개발자 4기 과정에서 다룬 것들 (보안 개발 학습)

### 주로 쓰는 것

C++ (C++23), CMake, Go, Docker
