# 2023 해군 인공지능 경진대회
* 예선 : 5/27(토)
  - 온라인 소양평가
* 본선 : 6/27(화) ~ 29(목)
  - 2박 3일간 팀별 프로젝트 수행
  - 주제 : 인공지능 모델 활용한 EO/IR 영상 및 이미지 내 드론 Detection

## EO/IR 영상 및 이미지 내 드론 실시간 Detect 모델 개발
* 데이터셋
  - EO/IR으로 촬영한 드론 이미지 및 label 데이터 약 16만장
  - 전체 데이터셋은 비공개

* 개발환경 Setting
  - 카카오 i cloud GPU 원격접속
  - CUDA & NVIDIA Driver 설치
  - https://velog.io/@yyk9612/2023-%ED%95%B4%EA%B5%B0-%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C%EB%B3%B8%EC%84%A0-%EC%B9%B4%EC%B9%B4%EC%98%A4-i-cloud-GPU-%EC%9B%90%EA%B2%A9%EC%A0%91%EC%86%8D-%EA%B0%9C%EB%B0%9C%ED%99%98%EA%B2%BD-%EC%84%B8%ED%8C%85%ED%95%98%EA%B8%B0

* 데이터 전처리 및 모델학습 과정
  - Convert COCO format to YOLO format
  - YOLO 학습을 위한 데이터셋 구조 설정
  - pre-trained weight 사용하여 Transfer Learning
  - 외부 데이터셋을 활용한 추가학습
  - https://velog.io/@yyk9612/2023-%ED%95%B4%EA%B5%B0-%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%EA%B2%BD%EC%A7%84%EB%8C%80%ED%9A%8C%EB%B3%B8%EC%84%A0
