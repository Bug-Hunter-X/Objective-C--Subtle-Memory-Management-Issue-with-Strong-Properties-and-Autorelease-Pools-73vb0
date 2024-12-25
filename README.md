# Objective-C Memory Management Bug

This repository demonstrates a subtle memory management issue in Objective-C related to strong properties and autorelease pools.  The `bug.m` file contains code that exhibits the problem, while `bugSolution.m` provides a corrected version.

The issue arises from the interaction between the strong property `myString` and the automatic deallocation of objects within an autorelease pool.  This can lead to dangling pointers and unexpected crashes.

The solution involves careful consideration of object ownership and lifetime.  The corrected code ensures proper object deallocation and avoids potential memory-related issues.