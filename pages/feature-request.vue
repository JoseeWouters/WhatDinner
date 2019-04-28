<template>
    <main class="main">
        <h1 class="title">Feature request</h1>
        <form name="request" action="/thanks" method="POST" netlify-honeypot="bot-field" data-netlify="true">
            <input type="hidden" name="form-name" value="request" />
            <fieldset class="hidden">
                <label for="bot-field">Don't fill this in if you're human</label>
                <input name="bot-field">
            </fieldset>
            
            <label for="Name">
                Your name:
            </label>
            <input type="text" name="name">

            <label>
                Your Email: 
            </label>
            <input type="email" name="email" />

            <label for="message">
                Your request:
            </label>
            <textarea name="message"></textarea>

            <button type="submit">Submit</button>
        </form>
    </main>
</template>

<script>
export default {
    
}
</script>
