이 프로젝트는 kankokutabi.jp 블로그 운영 자동화를 위한 마스터 지침서입니다. 모든 작업은 agents/ 폴더 내의 개별 에이전트 정의를 바탕으로 수행됩니다.

📂 Project Structure
agents/: 각 단계별 에이전트의 상세 역할과 Instruction (.md) 저장소
results/ : 각 단계별 에이전트들의 중간 산출물

Context Loading: 모든 작업 시작 전, 해당 단계의 agents/*.md 파일을 반드시 먼저 읽고 지침을 숙지한다.
Error Handling: 웹 탐색 중 오류 발생 시, 대체 소스를 찾거나 사용자에게 즉시 보고한다. 그리고 한번 실행되면 추가 확인 없이 모든 과정을 실행한다.
각 사이트를 읽어올것인지에 대한 질문은 하지 않고 진행한다.


실행순서 
 1. agents/topic_finder.md
 2. agents/blog_writer.md
 3. agents/seo_optimizor.md
