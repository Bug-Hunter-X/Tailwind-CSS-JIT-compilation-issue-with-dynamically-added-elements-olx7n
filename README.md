# Tailwind CSS JIT Compilation Issue with Dynamically Added Elements

This repository demonstrates a common issue when using Tailwind CSS with frameworks like Next.js or Nuxt.js:  Tailwind classes not being applied to elements added to the DOM after the initial render.  The `bug.js` file showcases the problem, while `bugSolution.js` presents a solution.

## Problem
The core issue is that Tailwind's Just-In-Time (JIT) mode might not detect dynamically added elements.  Consequently, the Tailwind classes associated with these elements fail to apply.

## Solution
The solution involves forcing Tailwind to re-evaluate the styles after the elements are dynamically added to the DOM. This can be achieved using techniques like `forceUpdate` (React) or by re-rendering the component.

## Setup
1. Clone this repository.
2. Make sure you have Node.js and npm (or yarn) installed.
3. Install dependencies: `npm install` or `yarn install`.
4. Run the application (depending on the example used).