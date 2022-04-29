# E-Commerce Clone

This project is a clone of [Build and Deploy a Modern Full Stack ECommerce Application with Stripe](https://www.youtube.com/watch?v=4mOkFXyxfsU).

It mainly serves as private notes.

**Tech-Stack**:

- [Next.js](https://nextjs.org/)
- [Sanity](https://www.sanity.io/)
- [Stripe](https://stripe.com/)


## Setup Local Development Environment

OS Manjaro Linux 21.2.3

### Client

```bash
npx create-next-app client
```

Cd into the `client`.

Copy & paste dependencies in `package.json` and run `npm install --legacy-peer-deps`.

```json
"dependencies": {
  "@babel/core": "^7.17.9",
  "@sanity/client": "^3.2.0",
  "@sanity/image-url": "^1.0.1",
  "@stripe/stripe-js": "^1.25.0",
  "canvas-confetti": "^1.5.1",
  "next": "12.1.0",
  "next-sanity-image": "^3.2.1",
  "react": "17.0.2",
  "react-dom": "17.0.2",
  "react-hot-toast": "^2.2.0",
  "react-icons": "^4.3.1",
  "stripe": "^8.209.0"
}
```

Create a `.env.local` file

```bash
NEXT_PUBLIC_SANITY_TOKEN=sanity_token

STRIPE_SECRET_KEY=secret_key
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=stripe_publishable_key
```

### Sanity

Globally install the cli with

```bash
npm install -g @sanity/cli
```

Create a folder `sanity` and run

```bash
sanity init
```

Check the docs with `sanity docs`, manage the project with `sanity manage` and start the local dev server with `sanity start`.

### Stripe

Create a account on [stripe](https://stripe.com/).
