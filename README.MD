# ESEP Grade Calculator

This library is a simple utility to calculate your grades. You add assignment, exam,
and essay grades, and it gives back a final letter grade.

Runtime requirements:
Golang 1.24+

All the code is in the `grade-calculator/` folder, so run commands from there.

Example:
```go
gc := NewGradeCalculator()
gc.AddGrade("exam 1", 95, Exam)
gc.GetFinalGrade() // returns "A", "B", "C", "D", or "F"
```

Run unit tests:
```
cd grade-calculator/
go test ./...
```

Run unit tests with code coverage:
```
cd grade-calculator/
go test -coverprofile=coverage.txt ./...
```

See coverage by function, or open it in the browser:
```
go tool cover -func=coverage.txt
go tool cover -html=coverage.txt
```
