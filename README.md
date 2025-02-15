# React Router Dom Nested Route Rendering Issue

This repository demonstrates a subtle bug in React Router Dom v6 related to nested routes and the rendering of components within a parent route that only acts as a container for nested routes.

## Problem Description

The issue arises when a nested route is defined within a parent route that does not render any content of its own.  The parent route's component seemingly overrides the nested route, causing only the parent to render. The bug.js file reproduces this problem.

## Solution

The solution involves adding an `Outlet` component to the parent route's component. The `Outlet` component renders the child route. The bugSolution.js file provides a corrected implementation.

## Setup

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `npm start`.
