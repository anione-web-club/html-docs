<script>
    import { ExampleCode } from '$lib/ui';
</script>

<h1>HTML 태그 구조</h1>
<hr>

<p>
    HTML은 HyperText Markup Language의 약자입니다 <br />
    웹 페이지는 HTML 문서라고도 불리며, HTML 태그들로 구성됩니다 <br />
    각각의 HTML 태그는 웹 페이지의 디자인이나 기능을 결정하는데 사용됩니다 <br />
</p>

<h3>태그란</h3>
<p>
    HTML 태그는 태그 이름을 꺾쇠 괄호({'< >'})로 감싸서 표현합니다. <br />
    HTML 태그는 시작 태그와 종료 태그로 구성되며, 
    시작 태그와 종료 태그는 태그 이름 사이에 슬래시(/)를 넣어서 표현합니다 <br />
    그러나 일부 태그는 시작 태그만 있고 종료 태그가 없는 단일 태그로 구성됩니다 <br />
</p>

<ExampleCode 
    placeholder='tag'
    codeProcessor={(input) => `<${input}>내용</${input}>`}
/>

<p>
    HTML 태그는 대소문자를 구분하지 않습니다
</p>

<p>
    HTML 요소(element)는 여러 속성을 가질 수 있으며, <br>
    이러한 속성(attribute)은 해당 요소에 대한 추가적인 정보를 제공합니다 <br />
    속성은 HTML 요소 중에서도 언제나 시작 태그 내에서만 정의되며, <br>
     속성 이름과 속성값(value)으로 표현됩니다
</p>

<ExampleCode 
    placeholder='https://www.naver.com'
    codeProcessor={(input) => `<a href=${input}>내용</a>`}
/>
