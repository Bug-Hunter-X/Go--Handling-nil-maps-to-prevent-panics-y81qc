# Go: Handling nil maps to prevent panics

This repository demonstrates a common Go error: panics caused by dereferencing nil maps.

The `bug.go` file contains code that will panic if the map is nil.  The `bugSolution.go` file provides a solution that safely handles this case.

## How to reproduce the bug

1. Run `bug.go`.
2. Observe the runtime panic.

## Solution

The solution involves checking for nil before accessing the map.  The provided `bugSolution.go` shows the corrected code.  This prevents the panic and handles the case where the map is nil gracefully.