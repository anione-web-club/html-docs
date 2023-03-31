<script>
    import { Badge } from 'sveltestrap/src';
    import { ExampleCode } from '$lib/ui';
</script>

<h1>h1~h6</h1>
<hr>

<p>
    HTML <Badge>{'h1'}</Badge>~<Badge>{'h6'}</Badge> (heading) 태그는
    6단계로 강조되는 제목을 나타냅니다. 
    <br>
    강조 단계는 <Badge>{'h1'}</Badge>이 가장 높고 <Badge>{'h6'}</Badge>이 가장 낮습니다.
</p>

<ExampleCode 
    placeholder='야수선배'
    codeProcessor={(input) => `
        <h1>${input}</h1>
        <h2>${input}</h2>
        <h3>${input}</h3>
        <h4>${input}</h4>
        <h5>${input}</h5>
        <h6>${input}</h6>
    `}
/>