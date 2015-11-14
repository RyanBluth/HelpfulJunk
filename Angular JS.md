## Built in Directives - Summarry ##

### ng-if ###
If the expression passed to ng-if evaluates to true then the element will be included in the DOM. Otherwise it will be removed from the DOM

### ng-show ###
Similar to ng-if in that ng-show expects and expression which evaluates to true or false. The difference is that if the expression evaluates to false then the element will be hidden using CSS as opposed to being removed from the DOM

### ng-hide ###
The same as ng-show except that the element is hidden if the expression is true and shown if the expression is false

## Basic Form Validation ##
**Requires the ngMessages module - This comes from angular-messages in bower**

```html
<form name="testForm">
  <input type="text" ng-model="field" name="testField" required minlength="5"/>
  <div ng-messages="testForm.testField.$error">
    <div ng-message="required">You did not enter a field</div>
    <div ng-message="minlength">The value entered is too short</div>
  </div>
</form>
```


