# Valuable snippets for Exceptions in Dart/Flutter

## Overview

Clear documentation for exceptions is valuable. This repository provides a snippet for documenting potential exceptions that a method or function can throw in Dart.

## How to Use

When defining exceptions in your code, it's essential to document the exceptions that a method or function can throw. these snippet helps in creating structured exceptions and documentation.

### Install the Snippets

1. Copy the snippets provided below.
2. Add it to your editor's snippet configuration. For example, in Visual Studio Code, go to `Preferences > User Snippets` and select your Dart file or create a new snippet file.
3. Paste the following snippet configuration:

```json
"Exception Comment Only": {
  "prefix": "exceptionComment",
  "body": [
    "/// ${1:Method description}",
    "///",
    "/// Throws:",
    "///",
    "/// * [${2:ExceptionName}] - ${3:Reason for the exception}"
  ],
  "description": "Template for documenting exceptions a method can throw"
},
"Custom Exception": {
  "prefix": "customException",
  "body": [
    "class ${1:CustomException} implements Exception {",
    "  ${1:CustomException}(this.message);",
    "",
    "  final String message;",
    "",
    "  @override",
    "  String toString() => '${1:CustomException}: \$message';",
    "}"
  ],
  "description": "Snippet for creating a custom exception class that implements Exception."
}
```
