##Dmitry Shemyakin
###Contacts:
  * city: _Nizhniy Novgorod_
  * email: _disemper@gmail.com_
  * tel.: _8(908)-151-41-14_
  
###About me
I like programming and I want to develop my skills in this sphere.
I want to continue learning and realize my potential.

###Skills
I use next technologies: 
* HTML;
* CSS / SCSS;
* Gulp;
* JS, jQuery;
* Bootstrap;
* Figma, Zeplin, Adobe XD;
* GIT, Atlassian Jira.

###Code Examples
An example code from my jQuery plugin for quick work with forms?  
_You can see the full plugin code [here](https://gitlab.com/disemper)_
```javascript
function validation(form) {
  let errors = false;
  const values = {};

  form.find('input:not([type="hidden"], [type="checkbox"], [type="radio"]), textarea').each(function () {
    const field = $(this);
    const value = field.val();
    const fieldName = field.attr('name');
    values[fieldName] = value;

    if (isRequired(field) && isEmpty(field)) {
      setErrorField(field);
      errors = true;
      return;
    }
    if (!isEmpty(field) && isMin(field)) {
      const reg = /\{\w+\}/;
      newMessageMin = messageMin.replace(reg, field.attr('minlength'));

      setErrorField(field, newMessageMin);

      errors = true;
      return;
    }
    if (validators) {

      if (validators[fieldName]) {
        for (const method in validators[fieldName]) {
          const func = validators[fieldName][method];
          if (func(value)) {
            setErrorField(field, func(value));
            errors = true;
            return;
          }
        }
      }
    }

  });

  const validateResult = validate(values);

  if (validateResult) {
    for (fieldName in validateResult) {
      const field = form.find('[name="'+ fieldName +'"]');
      setErrorField(field, validateResult[fieldName]);
    }
    errors = true;
  };

  return !errors;
}
```

###A few projects (Frontend)
* https://www.mk.metalexpert.pro/
* http://arkoiltech.nl/en
* http://aplana.ru/

###English
Pre-Intermediate
