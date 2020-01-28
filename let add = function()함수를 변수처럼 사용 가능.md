- let add = function()
  - 함수를 변수처럼 사용 가능

- function func2(name)



- 가변, 고정배열

  ```javascript
          <script>
              let myArray1 = ["apple", "banana", "orange"]; //고정배열
              let myArray2 = new Array(); //가변배열
              myArray2[0] = "grape";
              myArray2[1] = "lemon";
  
              console.log(myArray1);
              console.log(myArray2);
          </script>
  ```

- eval

  ```javascript
              let willEval = "";
              willEval += "var number=10;";
              willEval += "console.log(number);";
  
              eval(willEval);
  ```

  동적함수, 문자열을 코드로 실행하는 함수



- 변환 함수 , Number 함수 NaN 발생

  ```javascript
             let willEval = "";
              willEval += "var number=10;";
              willEval += "console.log(number);";
  
              eval(willEval);
  
  
  
              let a = parseInt("123원");        //string을 정수형으로 변환
              let b = parseFloat('1.22원');     //string을 유리수로 변환
              console.log( a);
              console.log( b);
              // Number() -> NaN
  
              let won = "1000원";
              let dollar = "1.5$";
              console.log(won + "/" + Number(dollar)); //Number 함수 NaN
     
  ```



- 함수 간략화(둘이 같은 문법)

  ```javascript
  
              let func = function() {
                 // console.log("Hello");
              }
              let func2 = () => {
                  console.log("Hello");
              }
  
  ```

  