# JavaScript 런타임과 node.js
이번 시간에는 JavaScript 런타임(runtime)에 대해 알아보겠습니다. 뭔가 런타임하면 어려운 개념인것 같지만 여러분은 이미 JavaScript 런타임을 사용하고 있습니다. 다들 웹 브라우저 사용하시죠?! 이게 바로 JavaScript **런타임**입니다.

**런타임**이란 프로그래밍 언어가 구동되는 환경입니다.환경이라는 말이 조금 어려울 수 있습니다. 쉽게말해 환경은 프로그램 입니다. 런타임 이란 **"어떤 프로그래밍 언어가 동작할 수 있는 프로그램"**입니다.우리가 JavaScript를 이용해서 코드를 적었으면 코드가 실행이 되어야겠죠? 바로 실행되는 곳이 바로 **런타임**입니다.

우리는 JavaScript를 다루고 있으니 JavaScript 런타임이 무엇이 있는지 살펴보겠습니다.먼저 아까 말씀드렸던 브라우저가 대표적인 JavaScript 런타임입니다. 이전에는 JavaScript 런타임이 브라우저 밖에 없었습니다. 하지만 이제 **node.js**라는 새로운 JavaScript 런타임이 나왔습니다. JavaScript가 브라우저가 아닌곳에서 실행될 수 있으니, 이제 우리는 JavaScript를 이용해서 웹페이지 뿐만 아니라 서버와 같은 다른 프로그램을 만들 수 있습니다.

이제 우리는 우리가 쓴 JavaScript 코드를 브라우저에서 실행시킬수도 있고, **node.js**라는 환경에서 실행시킬수도 있습니다.HTML `<script>` 태그 내에 JavaScript 코드를 작성한다면 우리가 작성한 코드는 브라우저에서 동작합니다.또는`node <file_name>` 명령어를 입력하시면 작성하신 코드가 **node.js**라는 환경에서 실행되게 됩니다. 예제를 하나 더 볼까요?

```jsx
// runnode.js
const testFunction = function(arg){
console.log("Arg is : ", arg);
}

testFunction(20);
```

자 이렇게 `runnode.js`라는 파일을 만들어 위와같이 코드를 작성해 보았습니다. 저 코드를 실행시키려면 어떻게 해야할까요? 저 파일을 브라우저에서 실행시키려면 html 파일을 만들어 그 안에 넣어주시면 됩니다. 이번에는 node에서 한번 실행시켜 보겠습니다. 아래와 같이 명령어를 입력해 보세요.

```jsx
$ node runnode.js
```

그럼 터미널창에`"Arg is : 20"` 이라는 메시지를 확인하실 수 있습니다. 자 이제 우리가 작성한 코드가 어디에서 동작하고 있는지 구분하실 수 있겠죠?!

정리하자면 **런타임**이란 **프로그래밍 언어가 돌아가는 환경**, 그리고 **node.js**는 **JavaScript 런타임**입니다.