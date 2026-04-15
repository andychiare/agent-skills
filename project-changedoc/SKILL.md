---
name: project-changedoc
description: Create a document that describes the code changes needed to transform a project from an initial status to a final status.
user-invocable: true
---


## Preliminary checks

Check if parameters are passed and follow the instructions described in the following subsections accordingly.

### No parameter passed

Make sure that you are in a git repository.

If you are in a git repository, consider the git history of the current branch and use the first commit as the initial project and the final commit as the final project.

Describe the changes following the commits in the history. 

### One parameter passed

Make sure that the parameter passed by the user is the URL to a git repository, for example, the URL to a GitHub repository.

Consider the git history of the main branch or the branch specified by the user. Use the first commit as the initial project and the final commit as the final project.

Describe the changes following the commits in the history. 

### Two parameters passed

Make sure that two parameters are passed.

If the user does not pass exactly two parameters, tell them that you need the path of the folder of the initial project as the first parameter and the path of the folder of the final project as the second parameter.

Make sure that the two parameters passed by the user are relative or absolute folder paths.

You will refer to the first folder as the initial project and to the second folder as the finnal project.

### Otherwise

Stop here and inform the user about what you expect as parameters.

## Instructions

You are a developer that understands the project code.

Consider the code of the initial project and compare it with the code of the final project.

Create a markdown document where you describe step by step how the user can obtain the final project starting from the initial project.

## Content creation rules

Follow the rules in this section to create the content for the document.

### Prerequisites

Summarize the technical prerequisites needed to run the projects you are going to document.

### Change description

Describe each step of the changes explaining why these changes are done.

In addtion to code changes, include configuration changes such as package installations, settings changes, etc.

### Code blocks

In each code block, add the path and file name of the file it refers to as in the following example:

```javascript
// myproject/src/myApp.js

console.log("Ok"):
```

Avoid long code block. Highlights the changes point by point using multiple short code blocks instead.

### Conclusion

Conclude the document with a quick recap of the changes and the instructions to run the final application.
