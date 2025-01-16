# Clean Exception Comments

## Overview

Clear documentation for exceptions is valuable. This repository provides a snippet for documenting potential exceptions that a method or function can throw in Dart.

## How to Use

When defining exceptions in your code, it's essential to document the exceptions that a method or function can throw. This snippet helps in creating structured exception documentation.

### Step 1: Install the Snippet

1. Copy the snippet provided below.
2. Add it to your editor's snippet configuration. For example, in Visual Studio Code, go to `Preferences > User Snippets` and select your Dart file or create a new snippet file.
3. Paste the following snippet configuration:

```json
"Exception Comment Only": {
  "prefix": "exceptioncomment",
  "body": [
    "/// ${1:Method description}",
    "///",
    "/// Throws:",
    "///",
    "/// * [${2:ExceptionName}] - ${3:Reason for the exception}"
  ],
  "description": "Template for documenting exceptions a method can throw"
}
