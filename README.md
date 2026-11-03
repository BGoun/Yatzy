
# YATZY CLASSIC

Teachable Machine 기반 손동작 인식 주사위 게임입니다.

## Features

- Classic Yatzy Score Board
- 5 Dice System
- 3 Rolls Per Turn
- Hold / Release Dice
- Automatic Score Calculation
- Upper Section Bonus
- Teachable Machine Gesture Recognition
- Webcam Control
- GitHub Pages Support

## Project Structure

YATZY-CLASSIC/
├── index.html
├── model/
│   ├── model.json
│   ├── metadata.json
│   └── weights.bin
└── README.md

## AI Model Setup

1. Teachable Machine에서 Image Project를 생성합니다.
2. 다음 7개 클래스를 생성합니다.

- roll
- hold_1
- hold_2
- hold_3
- hold_4
- hold_5
- confirm

3. 모델을 학습시킵니다.
4. Export Model에서 TensorFlow.js 형식으로 다운로드합니다.
5. ZIP 파일을 압축 해제합니다.
6. model.json, metadata.json, weights.bin 파일을 model 폴더에 넣습니다.

## Run Locally

카메라 사용을 위해 localhost 또는 HTTPS 환경이 필요합니다.

Python이 설치되어 있다면 프로젝트 폴더에서 실행합니다.

python -m http.server 8000

브라우저에서 접속합니다.

http://localhost:8000

## GitHub Pages

1. GitHub Repository를 생성합니다.
2. 프로젝트 파일 전체를 업로드합니다.
3. Settings → Pages로 이동합니다.
4. Deploy from a branch를 선택합니다.
5. Branch를 main, Folder를 /root로 설정합니다.
6. Save를 누릅니다.

배포 완료 후 제공되는 GitHub Pages 주소로 접속합니다.

## Controls

| Gesture | Action |
|---|---|
| roll | Roll Dice |
| hold_1 | Hold Dice 1 |
| hold_2 | Hold Dice 2 |
| hold_3 | Hold Dice 3 |
| hold_4 | Hold Dice 4 |
| hold_5 | Hold Dice 5 |
| confirm | Confirm Score |

## Requirements

- Modern Web Browser
- Webcam
- Teachable Machine TensorFlow.js Model
- HTTPS or localhost

## License

Personal Project
