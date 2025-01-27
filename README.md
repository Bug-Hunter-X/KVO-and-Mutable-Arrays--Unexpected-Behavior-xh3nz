# Objective-C KVO and Mutable Arrays Bug

This repository demonstrates a subtle bug that can occur when using Key-Value Observing (KVO) with mutable arrays in Objective-C.  Directly modifying the array (adding or removing objects) can lead to incorrect KVO notifications, causing unexpected behavior or crashes.

The `mutableArrayKVOBug.m` file shows the problematic code. The `mutableArrayKVOBugSolution.m` file provides a corrected version that uses appropriate methods to ensure correct KVO notification.

## How to Reproduce

1. Clone this repository.
2. Compile and run `mutableArrayKVOBug.m`.
3. Observe the inconsistent behavior or potential crash.
4. Compile and run `mutableArrayKVOBugSolution.m` to see the corrected behavior.