# FileReader and Template Classes

## [FileReader Class](./docs/FileReader.md)

The FileReader class is a part of the package `org.noahspoling.Models` and is an implementation of the IFileReader interface. The main purpose of this class is to read from text files, generate templates from them, and create files from those templates.

### Key Methods:

- `readFromTxt(String filename)`: Reads from a text file and generates templates from the lines in the file.
- `generateTemplate(String[] entries)`: Generates a template based on the entries provided.
- `createFiles(List<Template> templates)`: Creates files from the provided list of templates.
- `outputFromTemplate(Template template, String filetype)`: Creates a file of the specified filetype from the provided template.
- `replaceText(String replaceText, List<String> entries)`: Replaces placeholders in the text with the provided entries.

---

## [TemplateA Class](./docs/Template.md)

The TemplateA class extends the Template class and is also a part of the `org.noahspoling.Models` package. This class serves as a concrete implementation of the abstract Template class. It has additional attributes specific to the "TemplateA" type, including `name`, `item`, `replacedItem`, and `priceDifference`.

### Key Methods:

- `getEntries()`: Returns a list of all the entries in the template, which includes the values of all the fields of this class.




## [TemplateB Class](./docs/Template.md)


The TemplateB class extends the Template class and is a part of the `org.noahspoling.Models` package. This class serves as a concrete implementation of the abstract Template class. It has additional attributes specific to the "TemplateB" type, including `name`, `item`, `date`, `reward`, and `numOfWinners`.

### Key Methods:

- `getEntries()`: Returns a list of all the entries in the template, which includes the values of all the fields of this class.

## How to Use:

### TemplateB Class:

1. Instantiate a new TemplateB with the necessary parameters.
2. Use `getEntries` to get a list of all the entries in the template.

---

## How to Use:

### FileReader Class:

1. Instantiate a new FileReader with a text file name or a list of templates.
2. Use `readFromTxt` to read the contents of a text file.
3. Use `createFiles` to create files from the templates.

### TemplateA Class:

1. Instantiate a new TemplateA with the necessary parameters.
2. Use `getEntries` to get a list of all the entries in the template.

Please note that you'll need to adjust paths and inputs to fit your specific use case. It's also worth noting that this project includes exception handling to ensure that errors are dealt with appropriately. 

### TemplateA Class:

1. Instantiate a new TemplateA with the necessary parameters.
2. Use `getEntries` to get a list of all the entries in the template.

**Note**: The FileReader's constructor will automatically call `readFromTxt` to read the contents of the text file and generate templates. These templates will be stored in the `templates` list which is a member of the FileReader class.

---

## Template Child TemplateA

This template child extends the abstract Template class and specializes it to the "TemplateA" type. Its attributes include `name`, `item`, `replacedItem`, and `priceDifference`. It also overrides the `getEntries` method from the parent class to return a list of the values of its fields. This list can then be used to fill in placeholders in a document.