# Agent Skills

This is a personal collection of agent skills I created and use.

## Installation

Use [skills CLI](https://www.npmjs.com/package/skills) to install the skills (recommended).

To install all the skills:

```bash
npx skills add andychiare/agent-skills
```

Install specific skill:
```bash
npx skills add andychiare/skills --skill project-changedoc
```



## Skill List

- `project-changedoc` 
  
  It creates a markdown document that describes the code changes needed to transform a project from an initial status to a final status (*changelog --> changedoc*).
  
  **Usage**:
  
  ```
  /changedoc
  /changedoc https://github.com/owner/repo
  /changedoc path/to/initial-project path/to/final-project
  ```
  
  **Options**:
  
  You can use it with the following options:
  
  - **No paramaters**. It inspects the git history of the current branch and describes the changes starting from the initial commit to the last one.
  - **GitHub repo URL (one parameter)**. It inspects the git history of the main branch of the remote repo and describes the changes starting from the initial commit to the last one.
  - **Initial project, final project (two parameters)**. The first parameters is the path to the initial project's folder; the second parameter is the path to the final project's folder. It compares the two projects and documents the changes from the initial to the final project.
  
  The resulting document contains all the steps to obtain the final status of the project starting from the initial status, including prerequisites, code blocks, explanation of the changes, and instructions to run the final project.

## License

[MIT](LICENSE)