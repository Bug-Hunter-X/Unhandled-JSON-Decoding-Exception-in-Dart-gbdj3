# Unhandled JSON Decoding Exception in Dart

This repository demonstrates a common error in Dart when handling JSON responses from APIs: not properly handling potential `FormatException` exceptions that can occur during JSON decoding using `jsonDecode`.  The `bug.dart` file contains the buggy code, and `bugSolution.dart` provides a robust solution. 

The bug is that the code fails to handle cases where the API returns an invalid JSON response.  This causes the app to crash, resulting in a poor user experience. 

The solution addresses this by adding comprehensive error handling, including checks for non-200 HTTP status codes and appropriate handling of `FormatException` exceptions.