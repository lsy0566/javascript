

# javascript

## 불 자료형

- 비교 연산자
  - === 
  - !== 
    - 둘다 데이터 타입까지 비교

```javascript
            console.log('가방'>'하마');
            alert('가방'<'하마');
            alert('가방'=='하마');

            var a = 10;
            var b = '10';
            console.log(a == b);
            console.log(a === b);

            const userVal = prompt("값을 입력하세요. ");
            //짝수 홀수 판단

            if (userVal%2 == 0){
                console.log("짝수");
            }
                else{
                console.log("홀수");
                }    
                userVal = "test";
                console.log("당신이 입력한 값은 = " + userVal);
```





alert(), confirm() 확인버튼 보여줌, prompt() 입력받는 창 출력



- 변수 선언 방법
  - var
    - 일반변수
      - 비추천 계속 사용 가능해서 구별이 힘듦
  - let
    - 로컬변수
      - 두번 선언 불가
  - const
    - 상수변수
      - 두번 선언 불가





- window.onload

- 전위 후위

  ```javascript
                  console.log(a);
                  console.log(a++);
                  console.log(++a);
                  console.log(a);
  ```

  

## HTML 문법

```html
<!DOCTYPE html>
<html>
    <head>
        <script>

        </script>
    </head>
    <body>
        <table width= "100%" border="1">
        <tr>
            <td>A</td>
            <td>B</td>
            <td>B</td>
            <td>B</td>
        </tr>
        <tr>
            <td>E</td>
            <td>F</td>
            <td>G</td>
            <td>H</td>
        </tr>
    </table>
    </body>
</html>
```

- <tr>
  - 테이블 제목
- <tb>
  - 테이블명
- width=""
  - 테이블 넓이
- border=""
  - 테이블 외곽선 채우기
- ​      <td colspan="2">C</td>
  - 이 다음칸과 합치기
- ​      <td rowspan= "2">A</td>
  - 아래칸과 합치기

```javascript
<!DOCTYPE html>
<html>
    <head>
        <script>

        </script>
    </head>
    <body>
        <table width= "100%" border= "100">
            <tr>
                <th>Name</th>
                <th>Phone</th>
                <th>Address</th>
                <th colspan="2">Class</th>
            </tr>
        <tr>
            <td rowspan= "2">A</td>
            <td>B</td>
            <td>C</td>
            <td colspan="2">D</td>
        </tr>
        <tr>
            <!--<td>E</td>-->
            <td>F</td>
            <td>G</td>
            <td colspan="2">H</td>
        </tr>
        <tr>
            <td>I</td>
            <td>J</td>
            <td colspan="3">K</td>
        </tr>
        <tr>
            <td>L</td>
            <td>N</td>
            <td>M</td>
            <td>O</td>
            <td>P</td>
        </tr>
    </table>
    </body>
</html>
```





- placeholder
- textarea
- <input type="text" placeholder="이름을 입력하세요">
  -  한칸 유형 집어넣기
- <br>
  - 한줄 바꾸기/띄우기
- input type="password

```javascript
<!DOCTYPE html>
<html>
    <head>

        <script>
        </script>
    </head>
    <body>
        <form>
            이름 : <input type="text" placeholder="이름을 입력하세요">
            <br/>
            아이디 : <input type="text" placeholder="아이디를 입력하세요">  
            <br/>
            비밀번호 : <input type="password"" placeholder="비밀번호를 입력하세요">          
            <br/>
            남자: <input type="radio" name="gender">
            여자: <input type="radio" name="gender">
            <br/>
            사용하는 SNS:
            <input type="checkbox" name="sns">facebook
            <input type="checkbox" name="sns">twitter
            <input type="checkbox" name="sns">instagram
            <input type="checkbox" name="sns">google +
        </form>
    </body>
</html>
```

- ​      여자: <input type="radio" name="gender">

- <input type="file">

```javascript
            <textarea cols="40" rows="5">  </textarea>
                <br/>
                <input type="submit" value="회원가입">
                <input type="reset" value="초기화">
                <input type="button" value="임시 저장">
```

- POST/GET

```javascript
    <body>
        <form action="regist.html" method="POST">
```

- POST
  - 사용자가 입력한 내용을 -> 서버에 **전달**(가입, 저장)
  - request body
- GET
  - 사용자가 서버의 resource를 **요청**
  - 웹 브라우저 -> URL 요청
  - querystring

- querystring
  - GET 방식에서 사용
  - 데이터가 길거나 패스워드가 노출되므로 권장 X
  - 보안 수준이 낮음
  - url? + name=value &

- ​	OPTION/PUT/DELETE/TRACE/HEAD ... 
  - 별도 프로그램 사용

- casting -> 문자형을 숫자형으로 형변환

```javascript
let coverteData = Number(userData);
```



### 조건문

분기문

- switch

  ```javascript
              switch(avg) {
                  case 90:
                  console.log("A");
                  break;
                  case 80:
                  console.log("B");
                  break;
                  case 70:
                  console.log("C");
                  break;
                  case 60:
                  console.log("D");
                  break;
                  default:
                  console.log("F");
                  break;
              }
  ```



- switch >= 값 이용
  
  ```javascript
      switch(true) {
          case avg>=90:
          console.log("A");
          break;
          case avg>=80:
          console.log("B");
          break;
          case avg>=70:
          console.log("C");
          break;
          case avg>=60:
          console.log("D");
          break;
          default:
          console.log("F");
          break;
      }
  ```



- AND && -> &
- OR || -> |



- indexof()
  - 값이 들어있지 않다면 -1 출력
  - 몇번째부터 출력되었는지 확인 가능



- 배열

  ```javascript
             let array = [232, 12, 35, 234, 34];
              console.log(array);
              console.log(typeof array);
              console.log(array.length);
              console.log(array[0]);
              array[1] = 100;
              console.log(array[1]);
  ```

  - 배열 for문 이용

    ```javascript
                let array = [232, 12, 35, 234, 34];
                for (let i=0 ; i<=5 ; i++){
                console.log(array[i]);
                }
    ```



- 랜덤함수를 이용한 랜덤게임

  ```javascript
                  let comNum = Math.floor(Math.random() * 100 );// 0~1
              for (var i = 0 ; i<10; i++){
                  let userNum 
                      = Number(prompt("당신의 " + i + "번 째 예측한 숫자는? "));
                  if (comNum > userNum) {
                      alert("보다 큰 수를 입력하시오. ");
                  }
                  else if (comNum < userNum) {
                      alert("보다 작은 수를 입력하시오. ");
                  }
                  else {
                      alert("정답입니다. ");
                      break;
                  }
                  console.log(comNum);
              }
  ```

  