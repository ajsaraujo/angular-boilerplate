# angular-boilerplate

This is a simple boilerplate for Angular applications. It sets up ESLint, Prettier and a pre-commit hook that runs both. ⚙️

This configuration can be replicated with the following steps. It only takes some minutes. 👇

1. Generate a new Angular application with `ng new {{app-name}}`.
2. Install ESLint with `npm i eslint -D`.
3. Create the initial ESLint configuration with `eslint --init`. ESLint will prompt you some questions to generate the config. If you want to have the very same config just copy and paste the contents of `.eslintrc.json`.
4. Install Prettier with `npm i prettier -D`.
5. Create a file called `.prettierrc.json` at the root of the project, containing the object `{ "quote": "single", "semi": false }`.
6. Generate the pre-commit configuration by running `npx mrm@2 lint-staged`. At that point, _lint-staged_ might have generated a weird log file called `6` at the root of your project. If it did, you might want to delete it.
7. Change the `lint-staged` property of `package.json` to: `{ "*.ts": "eslint --cache --fix", "*.{ts,html,css,json}": "prettier --write" }`.

Aaaaand you're good to go. Happy coding! 🥰
