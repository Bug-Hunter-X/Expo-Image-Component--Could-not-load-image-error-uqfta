# Expo Image Component Error: Could not load image

This repository demonstrates a common error encountered when using the Expo `Image` component:  `Error: Could not load image: <uri>`. The error arises from providing an invalid or inaccessible image URI to the component. The `bug.js` file shows the problematic code, and `bugSolution.js` provides the corrected version.

## Problem

The `Image` component fails to load the image when given an invalid URI.  This can stem from typos in the URI, using a local file path that is incorrect, or referencing a remote URL that doesn't exist or is inaccessible.  The console will usually output an error message including the problematic URI.

## Solution

The solution involves carefully verifying the image URI. For local files, ensure the path is correct and the file exists. For remote URLs, double-check the URL for typos and confirm that the server is accessible and returns the image correctly.  In addition, you might need to consider adding error handling to gracefully manage cases where the image fails to load.