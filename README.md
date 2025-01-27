# React Router DOM Catch-All Route Issue

This repository demonstrates an uncommon issue encountered when using catch-all routes (`/*`) in React Router DOM, specifically when dealing with nested routes.  The catch-all route unexpectedly overrides other routes even when those other routes might have a more specific path.

## Problem Description

The problem occurs when you have a catch-all route defined along with other more specific routes. The catch-all route seems to always be matched, even if there's a more specific route that should be matched.  This breaks the expected routing behavior.

## Solution

The solution involves carefully ordering your routes.  The order in which you define your routes matters.  The most specific routes should be defined before the catch-all route.