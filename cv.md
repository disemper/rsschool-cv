## Dmitry Shemyakin

### Contacts:
  * city: _Nizhniy Novgorod_
  * email: _disemper@gmail.com_
  * tel.: _8(908)-151-41-14_
  
### About me
I like programming and I want to develop my skills in this sphere. My goal is to become a senior Frontend Developer  and  to take part in team development. My strengths are responsibility, attentiveness to details, teamwork.
I want to continue learning and realize my potential.

## Skills
I use next technologies: 
* HTML;
* CSS / SCSS;
* Gulp;
* JS, jQuery;
* Bootstrap;
* Figma, Zeplin, Adobe XD;
* GIT, Atlassian Jira.

### Code Examples
An example code from my jQuery plugin for quick work with forms?
_You can see the full plugin code [here](https://github.com/disemper/quick-form/blob/develop/src/js/jquery.quick-form.js)_
```javascript
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
```

### A few projects (Frontend)
* [https://www.mk.metalexpert.pro/](https://www.mk.metalexpert.pro/)
* [http://arkoiltech.nl/en](http://arkoiltech.nl/en)
* [http://aplana.ru/](http://aplana.ru/)

### English
Pre-Intermediate (A2)
