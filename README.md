This is a personalized [Next.js](https://nextjs.org/) starter kit for setting up common quality of life improvements on top of standard create-next-app installation easily.
## Motivation
I love Next.js and Tailwind and create-next-app also provides a really good way to setup tailwind with Next.js. But there are some things missing in the standard next.js installation which I used to setup on my every new Next.js project. 

Generally my standard create-next-app steps goes like this
- Select yes to add Typescript, EsLinst, Tailwind CSS, Src Directory, App router and customize default alias to @/*
- Install [Prettier](https://prettier.io/) and [Tailwind Prettier Plugin](https://tailwindcss.com/blog/automatic-class-sorting-with-prettier) Since the standard installation does not provide automatic class sorting for tailwind classes
- The default Eslint config is not enough for me so I like to extend Eslint configuration using eslint:recommended and also add additional eslint plugins like typescript-eslint, react, react-hooks & typescript-sort-keys
- Also I would like to add automatic import sorting plugin in prettier to sort all the imports alphabetically.
- After watching this [great talk](https://www.youtube.com/watch?v=sSJBeWPIipQ&ab_channel=JSWORLDConference) by [JoshuaKGoldberg](https://github.com/JoshuaKGoldberg/linting-typescript-in-2023), I loved his idea of customizing error display for eslint errors to yellow/warn so we can easily differentiate between typescript error(red/error) and linting error(yellow/warn). So setup the same for vscode project using .vscode/settings.json on project level
- Ask vscode to enable vscode to fix all the fixable linting errors on save. (Same in .vscode/settings.json)
- Also even if you are using absolute imports and use vscode to auto import stuff It may use relative import if it is shorter/closer of the import. So Ask vscode to always prefer absolute/non-relative imports for typescript/tsx files.

This things takes some time to setup everytime I create a new Next.js project so I decided to create a starter-kit to setup my next.js project using all this goodies with a single command
  
## Getting Started

Install it by the following command. This uses pnpm:

```bash
pnpx create-next-app --use-pnpm -e "https://github.com/bhattrajat/nextjs-boilerplate/tree/main/"
```

```bash
cd nextjs-boilerplate
```
Then run
```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

