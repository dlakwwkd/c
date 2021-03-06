작성자: 141033 박수빈
최종 작성일: 2014.06.13
설명: 사용자 입장에서 최대한 간편하게 느낄 수 있도록 하는 것을 목표로 했습니다.
      그리고 어떤 상황에서도 에러가 생기지 않는 안전성을 추구했습니다.

1. 조작키를 방향키, ENTER키, ESC키로 통일 했습니다.

2. 회원 등록시 리스트에 제대로 출력될 수 있는 값 범위 안으로 입력을 제한하였습니다.
	(즉, 너무 길거나 짧은 입력, Tap입력 등은 사전에 방지)
	
3. 어떤 입력 도중 취소하고 나가고 싶을 경우 바로 나갈 수 있도록 구성했습니다.

4. 리스트 화면에서 페이지를 빠르게 탐색할 수 있도록 ENTER키를 입력하면
   페이지를 검색할 수 있도록 하였습니다.

5. 검색 결과가 중복될 경우, 그 목록 창이 출력되도록 하였습니다.
	

=== 변경 사항 (2014.06.13) ===

* 강조색 구현방법 수정
* 종료시 선택지에도 적용
* 회원 등록시에 컬러 추가
* 연락처에 지번이 두 개인 경우도 등록 가능하게 수정
* 프로그램 시작 화면, 종료 화면 구성
* 시작, 종료 사운드 변경

=== 변경 사항 (2014.06.12) ===

* 메인 화면 구성 방법 변경
* 강조색 사용
* 메뉴 선택 숫자키로도 가능하도록 수정
* 페이지 검색 기능 추가
* 경고 메시지 함수로 분리
* define 이름 몇몇 가지 통합사용

=== 변경 사항 (2014.06.10) ===

* bottomMessageC 추가
* deleteMessage -> centerMessage로 함수 이름 변경

=== 변경 사항 (2014.06.08) ===

* 초기 화면 구성 방법 수정


=== 변경 사항 (2014.06.07) ===

* dataInput 함수 3가지 함수로 분리(dataInputA, dataInputB, dataInputWarning)
* 중복되는 UI 분리 (topMessage, bottomMessageA, bottomMessageB)
* 주석 추가
* 사운드 추가
* UI 색상 조금 변경
* 사운드 조정
* UI 개선 (메세지 박스 생성)
* 종료 노래 조정

=== 변경 사항 (2014.06.06) ===

* 회원 등록 중 주소 입력 시 발생할 수 있는 오류 수정
* 회원 수정 중 탭 입력 시 발생할 수 있는 오류 수정
* 데이터 파일 로드 중 띄어쓰기 있는 경우 발생하는 오류 수정
* maxsize, count 전역변수로 변경하고, 전반적인 함수 간소화
* 함수 위치 기능별 순서에 맞게 재배치
* 대대적인 UI 개선 (컬러 도입)
* 파일에 내용이 없을 경우 생기는 오류 수정
* 추가적인 UI 개선

=== 변경 사항 (2014.06.05) ===

* 회원 등록시 매번 maxid를 계산하는 것을 처음 한번만 하도록 수정
* 등록, 삭제, 수정 시에 중첩되는 입력 코드를 함수로 분리해서 단일화
* 마찬가지로 중복되는 검색 코드를 함수로 분리
* 여러 정수값 define 설정
* 검색, 종료 기능 완성
* 전반적으로 디버깅 하여 발견된 버그 모두 수정

=== 변경 사항 (2014.06.03) ===

* 입력키 값 define으로 정의 (ENTER, ESC 등)
* 코드 정돈 (줄 간격, 들여쓰기 등)
* 회원 등록 중도 취소 기능 변경 ('esc' 타이핑 -> ESC키 누르는 것으로)
* 중복되는 메시지 출력 코드 함수로 만들어 압축
* 검색 시 중복되는 값 필터링 기능 추가
* 회원 명단 출력 UI 개선

=== 변경 사항 (2014.06.03)(새벽) ===

* 회원 명단 출력 UI 개선
* 회원 등록시 이름 3글자 제한에서 4글자 제한으로 확대
* 회원 등록시 주소 10 ~ 15글자 에서 5 ~ 15글자로 범위 확대
* 삭제 기능 완성
* 버퍼 오버플로우 방지를 위해 함수 교체 (gets -> fgets)
* fgets는 '\n'을 저장해버리므로 이를 제거하는 과정 추가

=== 변경 사항 (2014.06.02) ===

* 메인 화면 인터페이스 변경 ( 숫자 입력에서 화살표 입력으로 )
* 연락처 입력시 형식에 정확히 맞아야 입력 되도록 입력 제한 기능 강화 
* 검색 기능, 삭제 기능(아직 미완) 추가
* 몇몇 주석 수정
