# Netflix_clone_coding
* 넷플릭스 클론코딩을 진행하며, 어려웠던 부분이나 새로 알게된 개념, 클론코딩 순서를 기록하고자 합니다. <br>

## 👑 HTML
### 1️⃣ main.html



## <br><br>⭕ CSS
### 1️⃣ style.css (main.html)
🔶 'display: flex' 속성: 어떤 방향에든 위치할 수 있으며, 동적으로 변경가능한 순서를 지정할 수 있고, <b>크기와 위치를 자동으로 지정</b>한다!! <br>
🔶 css 단위: <br>
1. px: 절대 단위<br>
2. em: 상대적인 단어/ 상위 요소의 폰트 사이즈를 기반으로<br>
3. rem: html 루트 요소의 폰트 사이즈가 계산의 기반값임/ 웹 브라우저의 폰트 사이즈를 기반으로 한 상대적인 사이즈/ 웹 브라우저마다 다른 기본 폰트 사이즈에 대응 가능<br>
-> rem이나 px 많이 사용 함! <br>

🔶 position: 요소가 배치되는 방식을 결정/ 기본값: static<br>
1. relative: 원래 위치를 기준으로 한 상대적인 위치/위, 아래, 양 옆의 위치 지정가능 <br>
2. absolute: 첫번째 상위 요소를 기준으로 배치<br>

🔶 'align-items'와 'justify-center' <br>
1. align-items: 세로축<br>
2. justify-center: 가로축<br>

🔶 요소 나란히 배치하기<br>
![image](https://user-images.githubusercontent.com/70849122/229091105-4bc451bf-5442-4fa1-ac55-c35899d0742c.png) <br>
-> 위와 같이 block형태로 나오는 dispay를 해결하기 위해서....... 로그인 버튼과 언어선택 select태그를 모두 감싸는 div에 display: flex 속성을 넣어주었더니 해결되었다. <br>
### 🔺 왜 inline으로 하면 안되는가? 원래 되야하는 거 아님?????


## <br><br>✔ JS
### 1️⃣ main.js 
