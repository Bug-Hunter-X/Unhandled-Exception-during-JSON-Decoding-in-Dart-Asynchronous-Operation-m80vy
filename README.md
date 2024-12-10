# Unhandled Exception during JSON Decoding in Dart

This repository demonstrates a common error in Dart: neglecting to handle exceptions that can occur during JSON decoding within asynchronous functions. The `bug.dart` file showcases this issue, while `bugSolution.dart` presents a corrected version with improved error handling.

## Problem

The original code lacks specific error handling for JSON decoding.  If the API response isn't valid JSON, a `FormatException` is thrown, but is only caught generically, obscuring the actual cause of the failure. 

## Solution

The solution improves exception handling by specifically catching `FormatException` and providing more informative error messages. It also includes more robust error handling around the HTTP request and response status.