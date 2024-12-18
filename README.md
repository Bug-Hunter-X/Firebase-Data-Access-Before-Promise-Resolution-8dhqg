# Firebase Data Access Before Promise Resolution

This repository demonstrates a common error in Firebase development: attempting to access data from a Firestore document before the asynchronous operation completes. The `bug.js` file shows the erroneous code, while `bugSolution.js` provides the corrected version.

The problem arises when developers incorrectly assume that data is instantly available after initiating a query.  This often leads to `undefined` or similar errors. The solution emphasizes the importance of using Promises and `.then()` or `async/await` to ensure data is ready before accessing it.

## Usage:

1.  Ensure you have the Firebase JavaScript SDK installed and configured.
2.  Run `bug.js` to see the error in action.
3.  Run `bugSolution.js` to see the correct implementation.