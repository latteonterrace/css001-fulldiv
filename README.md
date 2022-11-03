# div 전체화면 설정

width와 height를 100%로 설정하면 전체화면이 될 것만 같지만 그렇지 않습니다. 
* %는 부모 요소 길이의 몇%를 차지할 것인지 나타내기 때문에
* 먼저는 부모 요소의 길이가 설정되어 있어야 합니다.

다음과 같이 마크업을 작성합니다. 

```html
<div class="main">
    main
</div>
```

css를 다음과 같이 작성하여 높이와 널이를 모두 100%로 설정하면 전체화면이 될 것으로 생각할 것입니다. 

```css
.main {
    background-color: rgb(190, 123, 219);
    height: 100%; 
    width: 100%;
}
```

main의 부모 요소인 body와 html의 width, height를 지정해줘야 합니다. 

```css
html, body { 
    margin: 0px;
    background-color: yellow;
    height: 100%;  
    width: 100%;  
}
```

이제 전체 화면으로 보일 것입니다. 