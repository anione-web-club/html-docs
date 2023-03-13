<script>
    import { Badge } from 'sveltestrap/src';
    import { ExampleCode } from '$lib/ui';
</script>

<h1>p</h1>

<p>
    HTML <Badge>{'<a>'}</Badge> 태그(앵커 태그)는 <Badge>href</Badge> 속성을 통해 
    다른 페이지나 같은 페이지의 어느 위치, 파일, 이메일 주소와 그 외 다른 URL로 연결할 수 있는 하이퍼링크를 만듭니다. 
    <Badge>{'<a>'}</Badge> 안의 콘텐츠는 링크의 목적지의 설명을 나타내야 합니다.
</p>

<ExampleCode 
    placeholder='https://www.naver.com'
    codeProcessor={(input) => `<a href="${input}">링크</a>`}
/>