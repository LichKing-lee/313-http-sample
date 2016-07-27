313 http 발표 예제 코드

AJAX을 위한 래퍼함수 제공  
$http() 함수를 제공하며 jquery의 ajax() 함수와 대동소이함  
-책에 나와있는 설정들  

promise 객체  
-jquery 에서는 success, error 콜백함수를 설정해줬지만 $http()는 promise 라는 객체를 반환함. 해당 객체에 성공과 실패시 작동 함수를 설정.  
-promise는 콜백함수를 인자로 받는 then, success, error 3개의 속성을 갖고있으며 then은 success, error 두 경우에 대한 인자를 받으며 개별함수인 success와 error는 각각 명칭에 맞는 상태일때 호출할 함수 1개만 인자로 받음  
-then과 개별함수 모두 등록되어있으면 then이 먼저 호출.  
-then은 응답에 대한 모든걸 갖고있는 response 객체 하나만을 인자로 받으며 success, error 개별함수들은 각 속성별로 인자를 받음, 결국 받는 인자는 동일함  

단축메서드 제공  
-http 메서드별로 호출가능한 API 제공  
-$http 객체의 속성 형태로 제공되며 메서드별 가독성과 호출의 편이성외에 큰 차이점은 없음  
