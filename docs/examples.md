# Examples

## Basic Form

The below, basic form are the suggested minimum items you require to begin using FormCat.

While the `_gotcha` input below isn't required (we use ReCAPTCHA to validate humans), it is still good practice to ensure you avoid getting spam.

```html
 <form action="https://form.cat/your@email.com" method="POST">
  <input type="text" name="_gotcha" style="display: none">
  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</form>
```

## All Available Features

The following example form contains all the available, advanced features.

```html
<form action="https://form.cat/your@email.com" method="POST">
    <input type="text" name="_gotcha" style="display: none">
    <input type="hidden" name="_subject" value="FormCat Example Form">
    <input type="hidden" name="_cc" value="tiger@form.cat,leopard@form.cat">
    <input type="hidden" name="_format" value="text">
    <input type="hidden" name="_language" value="en">
    <input type="hidden" name="_next" value="https://support.form.cat">
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
            <input type="submit" value="Submit Form">
        </div>
    </div>
</form>
```

## AJAX

Premium FormCat Lion users can submit forms via AJAX. This even works cross-origin. The trick is to set the Accept header to application/json. If you're using jQuery this can be done like so:

```javascript
$.ajax({
    url: "https://form.cat/FORM_ID",
    method: "POST",
    data: {message: "hello!"},
    dataType: "json"
});
```
