# create-t3-turbo

> **Note**
>Haryana Hackathon 2024 Metaverse Car racing game to control drug usage


## Installation

There are two ways of initializing an app using the `create-t3-turbo` starter. You can either use this repository as a template:

or use Turbo's CLI to init your project (use PNPM as package manager):



## About the app
Welcome, racers, to our metaverse car race game! Navigate the city, collecting coins to power up your vehicle for the final race. Beware of drugs on the road – they reduce your speed and control. In the final race, use your collected coins to upgrade your car for a competitive edge. Avoid drugs, as they lead to frequent blackouts, hindering your chances of victory. Skill, strategy, and a keen eye for coins will determine the ultimate champion. Racers, start your engines and race to victory in our thrilling metaverse challenge!


```text
.github
  └─ workflows
        └─ CI with pnpm cache setup
.vscode
  └─ Recommended extensions and settings for VSCode users
apps
  ├─ auth-proxy
  |   ├─ Nitro server to proxy OAuth requests in preview deployments
  |   └─ Uses Auth.js Core
  ├─ expo
  |   ├─ Expo SDK 49
  |   ├─ React Native using React 18 ar/vr technologies to run the game
  |   ├─ Navigation using Expo Router
  |   ├─ Tailwind using Nativewind
  |   └─ Typesafe API calls using tRPC
  └─ next.js
      ├─ Next.js 14 admin side and moderators
      ├─ React 18
      ├─ Tailwind CSS
      └─ E2E Typesafe API Server & Client
packages
  ├─ api
  |   └─ tRPC v10 router definition
  ├─ auth
  |   └─ Authentication using next-auth. **NOTE: Only for Next.js app, not Expo**
  └─ db
      └─ Typesafe db calls using Drizzle & Planetscale
tooling
  ├─ eslint
  |   └─ shared, fine-grained, eslint presets
  ├─ prettier
  |   └─ shared prettier configuration
  ├─ tailwind
  |   └─ shared tailwind configuration
  └─ typescript
      └─ shared tsconfig you can extend from
```

> In this template, we use `@acme` as a placeholder for package names. As a user, you might want to replace it with your own organization or project name. You can use find-and-replace to change all the instances of `@acme` to something like `@my-company` or `@project-name`.

## Quick Start

> **DB**
>  Uses drizzle orm to seamless send data and for concurrency support

To get it running, follow the steps below:

### 1. Setup dependencies

```bash
# Install dependencies
pnpm i

# Configure environment variables
# There is an `.env.example` in the root directory you can use for reference
cp .env.example .env

# Push the Drizzle schema to the database
pnpm db:push
```
