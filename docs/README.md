# Getting Started

[![Build Status](https://travis-ci.org/22digital/FormCat.svg?branch=master)](https://travis-ci.org/22digital/FormCat)

Basic form example:

```html
 <form action="https://form.cat/your@email.com" method="POST">
  <input type="text" name="_gotcha" style="display: none">
  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</form>
```

## Setup

Setting it up is easy and free. You don't even have to register. Here's how:

### 1. Setup the HTML form

Change your form's action-attribute to `https://form.cat/your@email.com` and replace `your@email.com` with your own email.

Form example:

```html
<form action="https://form.cat/kittymagic@gmail.com" method="POST">
```

### 2. Confirm your Email Address

Go to your website and submit the form once. This will send you an email asking you to confirm your email address, so that no one can start sending you spam from random websites.

### 3. All set, Receive Emails

From now on, when someone submits that form, we'll forward you the data as email.
