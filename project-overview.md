# Project Overview

Project Name: BuggyHelloWorld

Description: A minimal "Hello World" Next.js project designed to showcase error detection capabilities. The project includes a single page (`pages/index.tsx`) that intentionally contains a TypeScript type error.

Features:

*   Basic Next.js setup.
*   A `pages/index.tsx` component that attempts to render a number as a string, causing a type mismatch error.

Target Audience: Developers testing error detection and validation tools.

Technology Stack:

*   Cloudflare next-on-pages framework (NextJS).

pages/index.tsx (Example with intentional error):

```typescript
const HomePage = () => {
  const message: string = 123; // Intentional type error: assigning a number to a string
  return <h1>{message}</h1>;
};

export default HomePage;
```

(Note: The intentional type error is the assignment of the number `123` to the string variable `message`.)