# Django : Working with forms 

## Django Forms take a lot of the work out of all these steps, by providing a framework that lets you define forms and their fields programmatically, and then use these objects to both generate the form HTML code and handle much of the validation and user interaction.

### HTML Forms :

#### The form is defined in HTML as a collection of elements inside <form>…</form> tags, containing at least one input element of type="submit".

#### The role of the server is first to render the initial form state — either containing blank fields or pre-populated with initial values. After the user presses the submit button, the server will receive the form data with values from the web browser and must validate the information. If the form contains invalid data, the server should display the form again, this time with user-entered data in "valid" fields and messages to describe the problem for the invalid fields. Once the server gets a request with all valid form data, it can perform an appropriate action (such as: saving the data, returning the result of a search, uploading a file, etc.) and then notify the user.


#### the main things that Django's form handling does are:

#### Display the default form the first time it is requested by the user.
#### The form may contain blank fields if you're creating a new record, or it may be pre-populated with initial values (for example, if you are changing a record, or have useful default initial values).
#### The form is referred to as unbound at this point, because it isn't associated with any user-entered data (though it may have initial values).
#### Receive data from a submit request and bind it to the form.
#### Binding data to the form means that the user-entered data and any errors are available when we need to redisplay the form.
#### Clean and validate the data.
#### Cleaning the data performs sanitization of the input fields, such as removing invalid characters that might be used to #### send malicious content to the server, and converts them into consistent Python types.
#### Validation checks that the values are appropriate for the field (for example, that they are in the right date range, #### aren't too short or too long, etc.)
#### If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem #### fields.
#### If all data is valid, perform required actions (such as save the data, send an email, return the result of a search, #### upload a file, and so on).
#### Once all actions are complete, redirect the user to another page.

#### There are many other types of form fields, which you will largely recognize from their similarity to the equivalent model field classes:

- BooleanField
- CharField
- ChoiceField
- TypedChoiceField
- DateField
- DateTimeField
- DecimalField
- DurationField
- EmailField
- FileField
- FilePathField
- FloatField
- ImageField
- IntegerField
- GenericIPAddressField
- MultipleChoiceField
- TypedMultipleChoiceField
- NullBooleanField
- RegexField
- SlugField
- TimeField
- URLField
- UUIDField
- ComboField
- MultiValueField
- SplitDateTimeField
- ModelMultipleChoiceField
- ModelChoiceField


### The arguments that are common to most fields are listed below (these have sensible default values):

#### required: If True, the field may not be left blank or given a None value. Fields are required by default, so you would set required=False to allow blank values in the form.
#### label: The label to use when rendering the field in HTML. If a label is not specified, Django will create one from the field name by capitalizing the first letter and replacing underscores with spaces (e.g. Renewal date).
#### label_suffix: By default, a colon is displayed after the label (e.g. Renewal date​:). This argument allows you to specify a different suffix containing other character(s).
#### initial: The initial value for the field when the form is displayed.
#### widget: The display widget to use.
#### help_text (as seen in the example above): Additional text that can be displayed in forms to explain how to use the field.
#### error_messages: A list of error messages for the field. You can override these with your own messages if needed.
#### validators: A list of functions that will be called on the field when it is validated.
#### localize: Enables the localization of form data input (see link for more information).
#### disabled: The field is displayed but its value cannot be edited if this is True. The default is False.