---
title: Test Form
layout: default
---
## Form Example

The following is an example form that you can test out below.

```html
<form action="https://forms.22digital.tech/hello@22digital.co.za" method="POST">
    <input type="text" name="_gotcha" style="display: none">
    <input type="hidden" name="_subject" value="22 Digital Test Form">
    <input type="hidden" name="_cc" value="hello@22digital.co.za">
    <input type="hidden" name="_format" value="html">
    <input type="hidden" name="_language" value="en">
    <div class="form">
        <div class="row">
            <div class="name">Name:</div>
            <div class="input">
                <input type="text" name="name" value="Type in your Name...">
            </div>
        </div>
        <div class="row">
            <div class="name">Email Address:</div>
            <div class="input">
                <input type="email" name="_replyto" value="Type in your Email Address...">
            </div>
        </div>
        <div class="row">
            <button type="submit">Send</button>
        </div>
    </div>
</form>
```
