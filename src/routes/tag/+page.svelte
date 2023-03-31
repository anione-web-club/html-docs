<script>
    import { ExampleCode } from '$lib/ui'
</script>

<h1>HTML 태그</h1>

<p>HTML 태그에 대한 기본적인 설명입니다</p>

<h2>주석</h2>

<p>
    주석은 열기({'<!--'})와 닫기({'-->'})로 구성되며, 이 안의 내용들은 무시됩니다.
    주석 처리된 구문은 웹 브라우저 상에서 표현되지 않으나,
    코드를 설명할 때에나 라이센스등의 코드 외적의 정보를 나타낼 때에 사용됩니다.
</p>

<ExampleCode
    placeholder="주석 안의 내용은 무시됩니다."
    codeProcessor={(input) => `<!--${input}-->`}
/>