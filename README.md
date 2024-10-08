# Initial-settings
초기 세팅과 관련된 레포지토리

---
## CODEOWNERS
### 용도
pr reviewer를  자동 등록하기 위해 사용한다.

### 모노레포 설정 시 
**주의사항** 
- 사용하려면 code owner 관련 branch 룰을 추가해줘야 한다.
- 반드시 *(아무거나) 이 위로 가야함
~~~
* @lsh1215 @YunJuwon0825 @Gwanghyeon-k @jung2941 @ukongee @kim1387

/frontend/ @jung2941 @ukongee @kim1387

/backend/ @lsh1215 @YunJuwon0825 @Gwanghyeon-k
~~~

## AI code review(ci)

### 용도
pr시 ai가 코드 리뷰를 달아준다.

### 방법
1. gpt api key를 발급받는다.
2. settings -> secrets and variables -> actions에 OPENAI_API_KEY값을 넣는다.<br>
   이때 secrets.GITHUB_TOKEN는 자동 발급되는 값임
3. ci file을 작성하여 테스트한다.