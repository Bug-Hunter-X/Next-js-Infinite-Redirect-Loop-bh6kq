# Next.js Infinite Redirect Loop

This repository demonstrates a common bug in Next.js applications: an infinite redirect loop. This occurs when you use the `useRouter` hook's `push` method to navigate to a route that is already active.  The solution involves checking the current route before attempting the redirect.

## Bug
The `bug.js` file contains a component that attempts to redirect to the same route using `router.push()`, creating the infinite loop.

## Solution
The `bugSolution.js` file provides a corrected implementation. It checks the current route before executing the redirect, preventing the infinite loop.