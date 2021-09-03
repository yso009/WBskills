# RULE

git 브랜치 구조 - git flow
---

**Main Branch** - 3개의 리뷰가 필요   

    1. Main		
    2. Develop		    

**Support Branch** -	2개의 리뷰 필요   

    1. Freshman 
    2. Sophomore
    3. Junior
    4. Senior
    
규칙
---
    1. 작업전 Issues를 통해서 티켓넘버을 생성한다.
    2. 하나의 티켓은 되도록 하나의 commit으로 한다.
    3. reviewer에게 review를 받는다.
    4. Merge는 마지막 Pull Request를 Review한 사람이 한다.   


   > Merge한 사람은 오타 및 코드 수정이 필요 없는지 확인하고 책임을 진다.

설명
---
**작업 순서**

    1. Issues 생성한다. Issue는 반드시 organization 저장소에서 생성한다.
    2. 작업 부분에 알맞은 branch에서 수정한다.
    3. Fork 저장소로 Push한다.
    4. Fork 저장소에서 organization 저장소로 pull request를 한다.
    5. 각 Branch 정책에 맞는 review 후 Develop branch에 병합한다.


**브렌치**

 * Main : Develop branch에서 QA가 끝난 코드만 병합한다. 오류가 없는 최종본.
 * Develop : support branch에서 새로운 기능 추가, 버그를 수정한 commit을 추가한다.
 * Support : Develop branch로부터 시작한다. 기능 추가 작업이 완료되면 Support branch는 Develop branch로 병합한다.

Commit 정책
---

기능 (티켓번호)   
기능 : 학년 + 파트(아이콘, 상세내용, 교과목명) + 내용   
ex) 1학년 아이콘 수정 (#14) ※한글로 명시한다.   
Commit message와 issue title은 같게 한다.   

