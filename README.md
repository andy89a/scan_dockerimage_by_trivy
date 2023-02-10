2023.02.10 
- 목적: 오픈소스인 trivy 이용하여 docker image repository 내 docker image os, library 취약점 점검
- 설명: github action 실행 단계에서 PROJECT_NAME(repo), IMAGE_NAME 입력 시 동작 함. 트리거가 workflow_disapatch 설정해서 수동 실행. 필요 시 이 부분을 push, schedule, pull_request 등등 변경하여 트리거 변경 가능
- 실행 방법: githun action 탭에서 workflow 클릭 후 변수 입력
- 참고: 아래 값은 github secret에 저장되어 있는 변수들이며, 인증서 파일은 테스트 용도로 만들었던 거라 의미 없음. TLS 통신 필요 시 다시 직접 생성해야 됨
  . DOCKERHUB_IP
  . DOCKERHUB_USERNAME
  . DOCKERHUB_TOKEN
  . ELASTICSEARCH_IP_PORT 
  . ELASTIC_PASSWORD
  . ELASTIC_USERNAME 
