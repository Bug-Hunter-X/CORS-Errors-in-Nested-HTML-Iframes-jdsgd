# CORS Errors in Nested HTML Iframes

This repository demonstrates a relatively uncommon HTML bug related to Cross-Origin Resource Sharing (CORS) issues that can arise when using nested iframes.  Accessing resources between iframes hosted on different origins can lead to unexpected errors and behavior.

The `bug.html` file showcases the problem, while `solution.html` provides a potential solution using techniques like `postMessage` for secure inter-iframe communication.

## Problem

Nested iframes from different origins often lead to CORS errors when attempting data sharing, even if both iframes appear to be correctly implemented.

## Solution

The preferred method is to use the `postMessage` API for secure communication between iframes irrespective of their origins. This method ensures data transfer is controlled and avoids CORS violations.