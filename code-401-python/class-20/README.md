# Django Using models:

## What is models :
### The definition of the model is independent of the underlying database — you can choose one of several as part of your project settings.

### When designing your models, it makes sense to have separate models for every "object" (a group of related information)

## what type of relationships does django allow to use ? 
### Once we've decided on our models and field, we need to think about the relationships. Django allows you to define relationships that are one to one (OneToOneField), one to many (ForeignKey) and many to many (ManyToManyField).

## Model definition:
### Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata.

## In the below sections we'll explore each of the features inside the model in detail:

### Fields
- A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables. Each database record (row) will consist of one of each field value.

### COMMON FIELD ARGUMENTS
- The following common arguments can be used when declaring many/most of the different field types
   - help_text.
   - verbose_name.
   - default.
   - null.
   - blank.
   - choices.
   - primary_key.

### COMMON FIELD TYPES
The following list describes some of the more commonly used types of fields.
   - CharField .
   - TextField .
   - IntegerField .
   - DateField and DateTimeField.
   - EmailField.
   - FileField and ImageField.
   - AutoField.
   - ForeignKey.
   - ManyToManyField .

### Metadata
You can declare model-level metadata for your Model by declaring class Meta One of the most useful features of this metadata is to control the default ordering of records returned when you query the model type. You do this by specifying the match order in a list of field names to the ordering attribute 
The ordering will depend on the type of field (character fields are sorted alphabetically, while date fields are sorted in chronological order).

### Methods
Minimally, in every model you should define the standard Python class method __str__() to return a human-readable string for each object. This string is used to represent individual records in the administration site (and anywhere else you need to refer to a model instance). Often this will return a title or name field from the model.

### Model management
Once you've defined your model classes you can use them to create, update, or delete records, and to run queries to get all records or particular subsets of records.

### Creating and modifying records
To create a record you can define an instance of the model and then call save().

### Searching for records
You can search for records that match certain criteria using the model's objects attribute.

## Django admin site :

### Steps to handle admin site and add the models to it :
- Registering models.
- Creating a superuser.
- Logging in and using the site.
- Advanced configuration.
- Register a ModelAdmin class.
- Configure list views.
- Add list filters.
- Organize detail view layout.
