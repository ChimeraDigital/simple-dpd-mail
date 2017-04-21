# dpd-mail
Simple integration of nodemailer with deployd

# Install 
`npm install dpd-mail --save`

# Usage
Go to your dashboard and create Mail resource and enter the requested info
To send an email just call the post method of the mail resource you have created

```javascript
dpd.mail.post({
 from: 'FROM <no-reply@example>',
    to: 'to@example',
    subject: 'Your subject',
    html: '<b>Html Content</b>',
    text: 'Text Content!'
}, function(result, error) {
  console.log(error); //Delete the log calls if you want
  console.log(result);
});
```
Change *mail* with your resource name

# Support
For any help post an issue or write to gustavo@chimera.digital
