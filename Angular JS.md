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


