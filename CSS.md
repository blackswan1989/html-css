## CSS는 최대한 상세하고 세밀하게 선택자를 써서 정의한 것들이 우선순위가 된다.

즉 그냥 .title { color : black }으로 정의 한 것보다 
#navbar.title { color : red } 로 정의한 것이 최종적으로 적용된다.

또 클래스보다 아이디 선택자가 클래스보다 우위에 있다.
ID(#)는 고유한 특정 아이디를 가진 태그에만 스타일링이 되고
Class(.)는 동일한 클래스를 가진 아이들 모두에게 적용이 되는 개념이다.
따라서 아이디 선택자로 스타일링 된 것이 클래스 선택자로 스타일링 된 것을 덮어씌우게 된다.


그러므로 #navbar 안에 .title이 있는 경우
#navber 에서 먼저 정의한것들이 있다면 .title을 따로 선택해도 변화가 없을 수 있다.
따라서 #navbar.title로 세밀하게 선택해줄 경우 #navbar를 이길 수 있게 된다.



## flex-basis


flex box 안에서 영역지정가능

ex)

box {
	display: flex;
}

box-left {
	flex-basis : 60%;
}

box-right {
	flex-basis : 40%;
}


## flex-wrap & img

parents-box {
	display: flex;
	align-items: center;
	justify-content: center;
	flex-wrap: wrap;
}

child-box {
	display: flex;
	align-items: center;
	justify-content: center;
	/* 가로세로 크기 지정해서 박스크기들 맞춰주기 */
	width: 300px; 
	height: 300px; 
	margin: 2px;
}

child-box img {
	max-width: 100%;
	max-height: 100%;
}

child-box안의 img들을 위처럼 설정해주면 
그 박스안에서 최대치 값으로 계속 보여지게 된다.
