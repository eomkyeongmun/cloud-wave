🛠 AWS CodeDeploy 기반 CI/CD 자동화 배포 실습
본 프로젝트는 단순한 코드 작성을 넘어, 클라우드 네이티브 환경에서의 지속적 통합 및 배포(CI/CD) 프로세스를 이해하고 실습하기 위해 진행되었습니다. AWS의 다양한 서비스(S3, CodeDeploy, Aurora DB)를 연동하여 애플리케이션 업데이트가 실제 서버에 어떻게 자동으로 반영되는지 확인하는 것에 중점을 두었습니다.

🎯 실습 목표
CI/CD 파이프라인 이해: Git Push부터 실제 서비스 반영까지의 자동화 흐름 파악
CodeDeploy 활용: appspec.yml과 배포 스크립트를 이용한 무중단 배포 및 서비스 제어 연습
인프라 연동: EC2 인스턴스와 Aurora PostgreSQL, S3 스토리지 간의 보안 및 네트워크 연결 설정

🏗 CI/CD 프로세스 구성도
EC2 (VS Code): 코드 수정 및 git push
GitHub: 소스 코드 저장 및 변경 사항 트리거
AWS S3: 배포 아티팩트 저장
AWS CodeDeploy: appspec.yml 설정에 따라 EC2 내부 배포 스크립트 실행
EC2 (Bastion/Web): 신규 코드 수신 및 Streamlit/Flask 서비스 재시작
