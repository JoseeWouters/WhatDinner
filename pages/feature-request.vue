<template>
    <div class="container">
        <h1 class="title">Feature request</h1>
        <p>Do you have a request for a feature that's not yet in the app?</p>
        <p>Fill out this form and I'll see what I can do!</p>
        <form class="form" name="request" action="/thanks" method="POST" netlify-honeypot="bot-field" data-netlify="true">
            <input type="hidden" name="form-name" value="request" />
            <fieldset class="hidden">
                <label for="bot-field">Don't fill this in if you're human</label>
                <input name="bot-field">
            </fieldset>
            
            <fieldset class="top">
                <label for="Name">
                    <span>Your name</span>
                    <input type="text" name="name">
                </label>
                <label>
                    <span>Your Email</span>
                    <input type="email" name="email" />
                </label>
            </fieldset>

            <label for="message">
                <span>Your request</span>
                <textarea name="message" rows="1"></textarea>
            </label>
            <button type="submit">Submit</button>
        </form>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.form {
    display: flex;
    flex-direction: column;
    background-color: $support;
    box-shadow: 0px 3px 15px rgba(0,0,0,0.1);
    margin: 1em;

    .hidden {
        display: none;
    }

    * {
        outline: 0;
        border: 0;
        font-family: inherit;
        font-size: inherit;
        color: inherit;

        &:focus {
            outline: 2px solid $primary;
            border-bottom-color: transparent;
        }
    }

    label {
        margin: 1em;

        span {
            display: block;
            margin-bottom: .5em;
        }
    }

    input, textarea {
        border-bottom: 2px solid $primary;
        padding-top: .5em;
        padding-bottom: .5em;
    }

    textarea {
        width: 100%;
    }

    .top {
        display: flex;
        justify-content: space-between;
    }

    button {
        background-color: $primary;
        color: $support;
        padding: .5em;
        margin-top: .5em;

        &:focus {
            outline: 0;
        }
    }
}
</style>
