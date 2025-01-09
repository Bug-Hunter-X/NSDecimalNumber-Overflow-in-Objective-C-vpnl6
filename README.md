# Objective-C NSDecimalNumber Overflow

This repository demonstrates a potential issue in Objective-C involving `NSDecimalNumber` calculations and how to handle them safely to prevent unexpected results or crashes.

## Problem:
When working with very large or very small numbers using `NSDecimalNumber`, the fixed-point representation can lead to overflow or underflow, causing incorrect calculations or program termination. 

## Solution:
The solution involves careful handling of potential overflow/underflow conditions.  Checking for exceptional conditions (like `NSDecimalNumberHandler`'s `exceptionDuringOperation` flag) and employing strategies like scaling numbers down before performing computations can mitigate this risk. The solution also includes the use of `NSDecimalNumberHandler` to customize rounding behavior. 

## How to run:
1. Clone the repository.
2. Open the project in Xcode.
3. Build and run the application.