# 원희찬 · Heechan Won

**Multi-cluster edge–cloud scheduling for real-time robots, built on Kubernetes.**

KETI(한국전자기술연구원) 메디컬IT융합연구센터에서 「미래 모빌리티를 위한 소프트웨어 정의형 인프라스트럭처(SDI)」 과제의 스케줄링 개발을 맡고 있습니다.
로봇 · 엣지 서버 · 클라우드에 흩어진 작업을, 중요한 작업일수록 마감을 지킬 수 있는 곳에 놓는 일을 합니다.

## 하는 일

- **멀티 클러스터 스케줄러** — Karmada 스케줄러 플러그인(Go). 위치마다 정확도 · 지연 · 에너지, 실시간 가능 여부, 배터리, 통신 위험도를 보고 후보를 거른 뒤 점수를 매겨 배치하고, 그곳을 고른 이유를 기록합니다.
- **혼합 중요도 Operator** — Kubernetes Operator(Go, controller-runtime). 작업마다 중요도 등급을 매기고, 가장 중요한 작업은 실시간 기기에서 마감을 지킬 수 있는지 확인한 뒤 그 기기에 고정합니다.
- **미션 번들 API** — Python · FastAPI. 외부에서 받은 미션 요청을 Kubernetes 객체로 바꿔 넣습니다.
- **디바이스 자동 등록** — 로봇(TurtleBot)과 Raspberry Pi 5(PREEMPT_RT 커널)가 KubeEdge 로 엣지 클러스터에 스스로 가입하고 상태 지표를 보내도록 만들었습니다.
- **배치 지연 줄이기** — 요청부터 로봇 위 컨테이너가 뜨기까지의 시간을 단계별로 재고 줄이고 있습니다.

## 기술

![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Karmada](https://img.shields.io/badge/Karmada-0E6BDB?style=flat-square)
![KubeEdge](https://img.shields.io/badge/KubeEdge-1B3E8C?style=flat-square)
![K3s](https://img.shields.io/badge/K3s-FFC61C?style=flat-square&logo=k3s&logoColor=black)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![ROS 2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry_Pi-A22846?style=flat-square&logo=raspberrypi&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

## 관심 있는 것

실시간 보장 스케줄링 · 엣지-클라우드 연속체 · 혼합 중요도 시스템 · 로봇을 위한 클라우드 네이티브 인프라
