# Multi-steps-form-Website
This is a personal solution to a Frontmentor project.

## Reference Designe

- Desktop: 1440px x 900
- Mobile: 375px x 812 Iph

<img width="549" alt="Reference-designe" src="https://github.com/juanpablobracco/Multi-steps-form-Website/assets/64668332/d8f93862-aa49-4569-ba1b-61144aaf4e1f">

## Deployed
https://multi-steps-form-website.vercel.app/
    
## Research and basic usefull data

### Form client side validation => https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation

- Builtin form validation:
  
  - required: Specifies whether a form field needs to be filled in before the form can be submitted.
  - minlength and maxlength: Specifies the minimum and maximum length of textual data (strings).
  - min and max: Specifies the minimum and maximum values of numerical input types.
  - type: Specifies whether the data needs to be a number, an email address, or some other specific preset type.
  - pattern: Specifies a regular expression that defines a pattern the entered data needs to follow.



### Constraint Validation Api => https://developer.mozilla.org/en-US/docs/Learn/Forms/Form_validation#the_constraint_validation_api

To interact with preset form setting: 

    const email = document.getElementById("mail");

    email.addEventListener("input", (event) => {
      if (email.validity.typeMismatch) {
        email.setCustomValidity("I am expecting an email address!");
      } else {
        email.setCustomValidity("");
      }
    });



### Website security =>
https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Website_security

- Warning: Never trust data passed to your server from the client. Even if your form is validating correctly and preventing malformed input on the client-side, a malicious user can still alter the network request.




