<script>
    import { Badge } from 'sveltestrap/src';
    import { ExampleCode } from '$lib/ui';
</script>

<h1>p</h1>
<hr>

<p>
    HTML <Badge>{'<p>'}</Badge> (paragraph) 태그는 하나의 문단을 나타냅니다. 
    시각적인 매체에서, 문단은 보통 인접 블록과의 여백과 첫 줄의 들여쓰기로 구분하지만, 
    HTML에서 문단은 이미지나 입력 폼 등 서로 관련있는 콘텐츠 무엇이나 될 수 있습니다.
    <br>
    문단은 블록 레벨 요소이며, 자신의 닫는 태그(<Badge>{'</p>'}</Badge>) 이전에 다른 블록 레벨 태그가 분석되면 자동으로 닫힙니다. 
</p>

<ExampleCode 
    placeholder='코코아는 역시 반호텐'
    codeProcessor={(input) => `<p>${input}</p>`}
/>