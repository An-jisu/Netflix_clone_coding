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

🔶 문서 수평으로 정렬할 때!! <br>
![image](https://user-images.githubusercontent.com/70849122/229290472-f2037e19-31cc-435a-b614-f16edbc8b4b4.png) <br>
-> 부모 요소에 이렇게 text-align: center 해줬더니 바로 해결.... <br>
-> 이거 자꾸 해결이 안되어서 애 먹었다..

🔶 text-align, justify-content, align-items 차이 <br>
- text-align: 말 그대로, 텍스트 문자만을 가운데로 정렬<br>
- justify-content: 주로 영역에 적용! 가로축 기준으로 정렬/ 글자를 감싸고 있는 그 영역 자체를! 주로 부모 요소에 써줌 <br> 
- align-items: 주로 영역에 적용! 수직축 기준으로 아이템들이 정렬/ 부모 요소의 자식들 전체를 묶어서 정렬- 주로 부모 요소에 써줌!<br>

🔶 main 부분에서 영상 삽입이 안되는 문제<br>
![image](https://user-images.githubusercontent.com/70849122/229295908-51cdc1d8-12b0-4a75-89ef-d55dd46e0d7d.png) <br>
-> css에서 영상의 width와 height를 지정해줌으로써, 영상이 나타남! <br>

## <br><br>✔ JS
### 1️⃣ main.js <br><br>


# 🥇👍 어려웠던 부분<br>
1. ![image](https://user-images.githubusercontent.com/70849122/229307622-95b0d7e7-2edf-4476-8eec-367f6cd6cc9d.png) <br>
-> 메인페이지의 이 부분의 블록을 짜는 것이 어려웠다. 각 요소들 간의 배치가 마음대로 되지 않았고, block형태로 정렬하고 싶은데 계속 나란히 정렬되고..클릭했을 때, 답변이 나오도록 구성하는 부분이 어려웠다. 그렇다면 이 블록을 코딩한 내용을 자세히 기술해 놓겠다. <br>
2023.04.04<br>
![image](https://user-images.githubusercontent.com/70849122/229688784-dc7c6243-7af9-47a2-a3f8-46f5b33c6812.png) <br>
-> 질문 블록에 대한 기본적인 구조는 완성하였다. 질문 블록에서 질문과 +가 세로 가운데 정렬로 오게하는 것을 해결하지 못 했다....



