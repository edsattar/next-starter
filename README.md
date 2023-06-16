## dependencies

```bash
npm i prisma @prisma/client
```

## structure

```ts
src
 ├────────────────────────────────────┐
 ├\app─<RootLayout> (1)               ├lib
 │  │   ├<Navbar> (3)                 └auth.js
 │  │   └<Toaster> (7)
 │  └─<RootPage> (2)
 │
 ├\api
 │ └\auth\[...nextauth]
 │             └─route.ts
 ├(auth)\sign-in
 │ └<SignInPage> (4)
 │   └<SignIn> (5)
 │     └<UserAuthForm-C> (6)
```

## >lib

#### >prisma.ts

Prisma Client instance plus additional logic to avoid instantiating Multiple instances in development.
