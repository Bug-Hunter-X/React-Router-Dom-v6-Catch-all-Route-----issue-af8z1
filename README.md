# React Router Dom v6 Catch-all Route '*' issue

This repository demonstrates a common issue encountered when using the catch-all route (`*`) in React Router Dom v6.  The catch-all route is intended to handle any unmatched routes, but in certain scenarios, it might not behave as expected.

## Issue Description

The problem arises when you have other routes defined and these other routes are not matched, this catch-all route does not catch any unmatched routes and the application shows a blank screen.

## Solution

The solution involves ensuring that the catch-all route is placed correctly within the route hierarchy, after all other specific routes.  This guarantees that the catch-all route will only be activated if no other route matches the URL.