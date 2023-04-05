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
-> css에서 영상의 width와 height를 지정해줌으로써, 영상이 나타남! <br><br><br>

### 2️⃣ style1.css (login.html)<br>
🔶 요소의 위치 조정
![image](https://user-images.githubusercontent.com/70849122/229998468-49896d6f-5279-4a75-8731-bea5ae9169e2.png) <br>
-> 배경 이미지 위로 넷플릭스 로고가 뜨길 원했는데, 배경 이미지 아래로 배치 되는 것이다. <br>
![image](https://user-images.githubusercontent.com/70849122/229999356-eafce6cc-f05e-4402-ad80-01b54560f88e.png) <br>
-> 이를 해결하기 위해 position: absolute를 써주었더니, 제대로 실행이 되었다. 부모 요소인 body를 기준으로 배치되는 것이므로 처음에 로고가 배치되는 것이다. <br>
position: absolute- 부모 요소를 기준으로 위치 결정<br><br>

🔶 요소 위에 다른 요소 배치 <br>
![image](https://user-images.githubusercontent.com/70849122/230010593-19a4b2a7-5e10-480d-8fad-6def4d07b418.png) <br>
-> 위와 같이 ipnut창 위에 label이 뜨게끔 처리하고 싶었다. <br>
![image](https://user-images.githubusercontent.com/70849122/230010859-3a36f7c4-f566-45c7-ae39-1f5d974e98c7.png)
![image](https://user-images.githubusercontent.com/70849122/230010907-c1cfade9-1b5e-470f-81eb-707858e796f3.png) <br>
-> 위와 같이 부모요소에 relative, label요소에 absolute를 position시켜줌으로써 실행시킬 수 있다.<br><br>





## <br><br>✔ JS
### 1️⃣ main.js <br><br>


# 🥇👍 어려웠던 부분<br>
1. 
![image](https://user-images.githubusercontent.com/70849122/229307622-95b0d7e7-2edf-4476-8eec-367f6cd6cc9d.png) <br>
-> 메인페이지의 이 부분의 블록을 짜는 것이 어려웠다. 각 요소들 간의 배치가 마음대로 되지 않았고, block형태로 정렬하고 싶은데 계속 나란히 정렬되고..클릭했을 때, 답변이 나오도록 구성하는 부분이 어려웠다. 그렇다면 이 블록을 코딩한 내용을 자세히 기술해 놓겠다. <br>
2023.04.04<br>
![image](https://user-images.githubusercontent.com/70849122/229688784-dc7c6243-7af9-47a2-a3f8-46f5b33c6812.png) <br>
-> 질문 블록에 대한 기본적인 구조는 완성하였다. 질문 블록에서 질문과 +가 세로 가운데 정렬로 오게하는 것을 해결하지 못 했다....


2. <br>
![image](https://user-images.githubusercontent.com/70849122/229994219-60c7e245-08f8-4d9c-a454-93a005b74a34.png) <br>
-> 메인페이지 풋터에서 그리드를 적용하는 것이 어려웠다. grid 개념을 잘 몰랐기 때문에... <br>
https://velog.io/@asj1966/HTMLCSSJS-CSS-GRID <br>
-> 따라서 위와 같이 일단 grid에 대한 학습을 하였다. <br>
![image](https://user-images.githubusercontent.com/70849122/229994388-6b7448b7-add3-4eed-b31d-9ff684723c18.png) <br> 
-> ul을 부모 요소, 즉 컨테이너라 생각하고, li를 각각의 아이템이라 생각하여, 컨테이너에 위와 같이 적용해주었다. 열은 3개를 각 1:1:1의 비율로 지정해주었고, 행은 1:1:1:1의 비율로 4개를 지정해주었다. <br>
