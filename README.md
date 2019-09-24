# GitHub Actions CI Templates

A repository of templates for GitHub Actions CI configurations.

## The Templates

- [JavaScript](./templates/javascript/)
  - [Node.js Cross-Platform](./templates/javascript/nodejs-cross-platform-ci.yml): 
    - Runs builds on:
      - Ubuntu (Latest),
      - Windows (Latest),
      - macOS (Latest)
    - Using all versions of Node.js that are [currently supported](https://github.com/nodejs/release#release-schedule) by the Node.js project,
    - Using `npm install` and `npm test`.
  - [Node.js Cross-Platform (using Yarn)](./templates/javascript/yarn-nodejs-cross-platform-ci.yml)
    - Runs builds on:
      - Ubuntu (Latest),
      - Windows (Latest),
      - macOS (Latest)
    - Using all versions of Node.js that are [currently supported](https://github.com/nodejs/release#release-schedule) by the Node.js project,
    - Using `yarn install` and `yarn test`.
  - [Node.js Cross-Platform (using pnpm)](./templates/javascript/pnpm-nodejs-cross-platform-ci.yml):
    - Runs builds on:
      - Ubuntu (Latest),
      - Windows (Latest),
      - macOS (Latest)
    - Using all versions of Node.js that are [currently supported](https://github.com/nodejs/release#release-schedule) by the Node.js project.
    - Using `pnpm install` and `pnpm test`.

## How to use the Templates

Add the appropriate YAML to your repository under the `.github/workflows/` path, naming the YAML whatever you'd like to name it. I generally like to follow the `language-platform(s)-ci.yml` pattern, but your mileage may vary.

For example, if you wanted to use the `nodejs-cross-platform-ci.yml` template, you'd add it in:

```bash
- .github/
  - workflows/
    - nodejs-cross-platform-ci.yml # you can rename this whatever you'd like
```

## How to improve the Templates

If you'd like to improve the templates provided, you're more than welcome to submit a PR! If you notice a template that's entirely missing but you'd like to see, feel free to send a Pull Request to add it yourself _or_ create an issue requesting it to be added.
