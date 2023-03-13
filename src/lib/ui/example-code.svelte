<script>
    import {
        Card,
        CardBody,
        CardHeader,
        CardTitle,
        Form,
        FormGroup,
        Input,
        CardText,
    } from 'sveltestrap/src';

    let input = ''
    $: code = `<p>${input}</p>` 
</script>

<Card>
    <CardHeader>
        <CardTitle>예제</CardTitle>
    </CardHeader>
    <CardBody>
        <Form>
            <FormGroup floating label='내용 작성'>
                <Input type='text' placeholder='예제' bind:value={input} />
            </FormGroup>
        </Form>
        <CardText>
            코드: {code}
        </CardText>
        <CardText>
            결과: {@html code}
        </CardText>
    </CardBody>
</Card>