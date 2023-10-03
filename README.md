# { name } resume

## Data

- GitHub Pages
  - [ja](https://YOUR_ACCOUNT.github.io/resume)
  - [en](https://YOUR_ACCOUNT.github.io/resume/en)
- PDF
  - [ja](https://github.com/YOUR_ACCOUNT/resume/releases/latest/download/resume.pdf)
  - [en](https://github.com/YOUR_ACCOUNT/resume/releases/latest/download/resume-en.pdf)
- File
  - [ja](https://github.com/YOUR_ACCOUNT/resume/blob/master/docs/README.md)
  - [en](https://github.com/YOUR_ACCOUNT/resume/blob/master/docs/en/README.md)

## Features

### 💅 Lint text

Automatic proofreading with [textlint](https://github.com/textlint/textlint).

```node
npm run lint --fix
```

It is also automatically executed when pre-commit by [husky](https://github.com/typicode/husky).  
proofreading rules are set with `.textlintrc`.

### 📝 Convert MD to PDF

You can generate PDF with [md-to-pdf](https://www.npmjs.com/package/md-to-pdf).

```node
npm run build:pdf
```

The output PDF can be styled as you like with CSS. Edit the `pdf-configs/style.css`.  

### :label: Versioning Semantically by label

versioning semantically by applying labels that `major`, `minor`, `patch`.
If no label is applied, the default version will be incremented as `patch`.
If you want to explicitly increase a version other than `patch`, Attach either `major` or `minor` label to PR

### 📆 Remind update

Automatically generate issues every three months with GitHub Actions Schedules triggers to prompt you to update your resume.

To change the duration or stop the job, edit `.github/workflows/create-issue.yml`.  
To change the issue contents, edit `.github/ISSUE_TEMPLATE.md`.
