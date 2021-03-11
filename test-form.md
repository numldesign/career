Create a light wrappers around Form (nu-form) and Form.Field (nu-field) and then create Form.Check (nu-check) element that can accept assert property and assign it directly to the nu-check element as a property via ref. It will allow to create custom validation for forms. Most of the time user can use built-in validators but we need a way to provide customization here.
Vanilla-numl example of form with check - https://numl.design/storybook/complex/login-form
In HTML there is no way to provide a function. But using JS it will look like:
```
const check = document.querySelector('nu-check');
check.assert = (val) => val && typeof val === 'string' && val.match(/^[a-z]{6}$/i); // value should be a string with length 6 and contain a-z characters, case insensitive.
```
So we need a React-way of doing so.

After completing the test you can create a public repo in your profile for review and share it with your correspondent Numl Team member.

Thanks!
