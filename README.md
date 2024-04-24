## MSA 서점 대여 서비스
MSA를 이해하기 위해 간단하게 기능을 만들어 서버간 통신을 해보는 Toy 프로젝트입니다. 우리가 흔히 접하고 명확한 구분이 가능한 서점 대여 서비스를 주제로 프로젝트를 진행했습니다.
<br/>
<br/>
## 프로젝트 구조
<img width="543" alt="image" src="https://github.com/JaeyoungChoi98/study_toy_MSA/assets/107467750/83a5c4e9-b7e8-4745-90a1-855315474c6b">
<br/>
<br/>

- Loan : 대여를 담당하는 서버

- User : 회원 정보와 회원 검증 서버

- Book : 책 정보와 수량 확인 서버

- History : 대여 기록을 저장하는 서버
<br/>

## 프로젝트 설명
1. Loan 서버에서 대여 요청을 받고 요청에 대한 검증을 User와 Book 서버로 보내 검증을 요청받는다.
2. 검증이 완료된 면 마지막으로 History 서버로 요청 데이터를 보내 대여 기록을 저장한다.
3. 그 과정에서 User와 Book 서버들은 history 서버에 대여 기록을 요청해 사용자의 현재 대여 중의 책의 개수를 파악하거나 대여하려고 하는 책의 재고가 얼마 있는지 파악하여 검증을 하게 된다.
<br/>
<br/>
<br/>
<br/>
<br/>


회고록 - https://blog.naver.com/jesikrjeje/223144715449
