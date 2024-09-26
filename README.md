Turborepo starter with shadcn/ui
Static Badge

This is Turborepo starter with shadcn/ui pre-configured.

Note

This example uses pnpm as package manager.

npm version

Using this example
Clone the repository:

git clone https://github.com/dan5py/turborepo-shadcn-ui.git
Install dependencies:

cd turborepo-shadcn-ui
pnpm install
Add ui components
Use the pre-made script:

pnpm ui add <component-name>
This works just like the shadcn/ui CLI.

Add a new app
Turborepo offer a simple command to add a new app:

pnpm turbo gen workspace --name <app-name>
This will create a new empty app in the apps directory.

If you want, you can copy an existing app with:

pnpm turbo gen workspace --name <app-name> --copy
Note

Remember to run pnpm install after copying an app.

What's inside?
This Turborepo includes the following packages/apps:

Apps and Packages
docs: a Next.js app
@repo/ui: a stub React component library (🚀 powered by shadcn/ui)
@repo/eslint-config: eslint configurations (includes eslint-config-next and eslint-config-prettier)
@repo/typescript-config: tsconfig.jsons used throughout the monorepo
Each package/app is 100% TypeScript.

Utilities
This Turborepo has some additional tools already setup for you:

TypeScript for static type checking
ESLint for code linting
Prettier for code formatting
Build
To build all apps and packages, run the following command:

cd turborepo-shadcn-ui
pnpm build
Develop
To develop all apps and packages, run the following command:

cd turborepo-shadcn-ui
pnpm dev
Remote Caching
Turborepo can use a technique known as Remote Caching to share cache artifacts across machines, enabling you to share build caches with your team and CI/CD pipelines.

By default, Turborepo will cache locally. To enable Remote Caching you will need an account with Vercel. If you don't have an account you can create one, then enter the following commands:

cd turborepo-shadcn-ui
npx turbo login
This will authenticate the Turborepo CLI with your Vercel account.

Next, you can link your Turborepo to your Remote Cache by running the following command from the root of your Turborepo:

npx turbo link
Useful Links
Learn more about the power of Turborepo:

Tasks
Caching
Remote Caching
Filtering
Configuration Options
CLI Usage
Learn more about shadcn/ui:

Documentation
