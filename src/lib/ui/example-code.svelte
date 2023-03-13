<script>
    import {
        Card,
        CardBody,
        CardHeader,
        CardTitle,
        Form,
        FormGroup,
        Input,
    } from 'sveltestrap/src';
</script>

<Card>
    <CardHeader>
        <CardTitle>예제</CardTitle>
    </CardHeader>
    <CardBody>
        <Form>
            <FormGroup floating label='p 태그'>
                <Input placeholder='예제' />
            </FormGroup>
        </Form>
    </CardBody>
</Card>