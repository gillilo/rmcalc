# rmcalc

`rmcalc` 저장소는 `rmcalc-express`와 `rmcalc-web` 두 개의 도커 컨테이너로 구성되어 있으며, 이는 `docker-compose.yml` 파일에 정의되어 있습니다. 
이 컨테이너들은 간단한 원-렙 맥스(OneRM) 계산 서비스를 제공하며, OneRM과 그 계산 공식을 설명하는 웹 인터페이스를 포함합니다.

## 저장소 구조

- **rmcalc-express**
  - 깃허브 저장소: [gillilo/rmcalc-express](https://github.com/gillilo/rmcalc-express)
  - 도커 이미지: `gillilo/rmcalc-express:latest`
  - 설명: OneRM을 계산해주는 간단한 Express.js API입니다.

- **rmcalc-web**
  - 깃허브 저장소: [gillilo/rmcalc-web](https://github.com/gillilo/rmcalc-web)
  - 도커 이미지: `gillilo/rmcalc-web:latest`
  - 설명: `rmcalc-express`의 API 문서(api-docs)를 포함하여, OneRM이 무엇인지, 그리고 계산 공식에 대해 설명하는 웹 페이지입니다.

## 사용 방법

### Docker Compose 사용

이 프로젝트는 Docker Compose를 사용하여 간편하게 설정할 수 있습니다. 다음 명령어를 통해 두 개의 컨테이너를 모두 시작할 수 있습니다.

```bash
docker-compose up
```

## 기여 방법

기여를 원하시면 이 저장소를 포크하고, 개선 사항을 추가한 후 풀 리퀘스트를 보내주세요. 버그 신고나 기능 요청은 이슈 트래커를 통해 해주시면 감사하겠습니다.

## 라이선스

이 프로젝트는 MIT 라이선스 하에 배포됩니다. 자세한 내용은 LICENSE 파일을 참조하세요.
