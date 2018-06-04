# Advance Features

Form inputs can have specially named `name-attributes`, which alter functionality. They are all prefixed with an underscore.

## _replyto

This value is used for the email's Reply-To field. This way you can directly "Reply" to the email to respond to the person who originally submitted the form.

## _next

By default, after submitting a form the user is shown the FormCat "Thank You" page. You can provide an alternative URL for that page.

## _subject

This value is used for the email's subject, so that you can quickly reply to submissions without having to edit the subject line each time.

## _cc

This value is used for the email's CC Field. This lets you send a copy of each submission to another email address. If you want to cc multiple emails, simply make the cc field a list of emails each separated by a comma.

## _gotcha

Add this _honeypot_ field to avoid spam by fooling scrapers. If a value is provided, the submission will be silently ignored. The input should be hidden with CSS.

## Using AJAX

Premium FormCat Lion users can submit forms via AJAX. This even works cross-origin. The trick is to set the Accept header to application/json. If you're using jQuery this can be done like so:

```javascript
$.ajax({
    url: "https://form.cat/FORM_ID",
    method: "POST",
    data: {message: "hello!"},
    dataType: "json"
});
```
