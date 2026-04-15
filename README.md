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
  
  Create a markdown document that describes the code changes needed to transform a project from an initial status to a final status.
  
  If you don't pass any parameter, it inspects the git history of the current branch and describes the changes starting from the initial commit to the last one.
  
  Otherwise, you can pass two parameters: the first parameters is the path to the initial project's folder; the second parameter is the path to the final project's folder.

## License

[MIT](LICENSE)