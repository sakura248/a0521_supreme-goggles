# Lab 1

## Q1: 
> Write a Java program with a method named 'totalSum' that takes in an argument of two integers and return its sum. Call this method from main( ) and print the results.

```
class main {
	public static int totalSum(int a, int b) {
		return a + b;
	}
	public static void main(String[] args) {
	System.out.println(totalSum(3,5));
	}
}

```

## Q2:
> Write a Java program with a method named 'getGrades' that will display grades according to the marks entered into the method call as below:
```
Marks        Grade
91-100         A+
81-90          A-
71-80          B+
61-70          B-
51-60          C+
41-50          D-
<=40          Fail
```

```
class main {
	public static String getRecords(int marks) {
		if (marks >= 91 && marks <= 100) {
			return "A+";
		} else if (marks >= 81) {
			return "A-";
		} else if (marks >= 71) {
			return "B+";
		} else if (marks >= 61) {
			return "B-";
		} else if (marks >= 51) {
			return "C+"; 
		} else if (marks >= 41) {
			return "D-"; 
		} else {
			return "fail";
		}
	}
	public static void main(String[] args) {
	System.out.println(getRecords(76));
	}
}
```

## Q3:
> Write a program to print the factorial of a number by defining a method named 'factorial'. Factorial of any number n is represented by n! and is equal to 1*2*3*....
``` 
4! = 1*2*3*4 = 24
3! = 3*2*1 = 6
2! = 2*1 = 2
Also,
1! = 1
0! = 0
```

```
class main {
	public static int factorial(int n) {
		if (n > 0 ){
			n = n*factorial(n-1);
		}else {
			n = 1; 
		}
		return n;
		}
	public static void main(String[] args) {
		
	System.out.println(factorial(4));
	}
}
```

## Q4
> Write a Java method to create the area of a pentagon.

```
class main {
	public static double pnetagon(int n) {
		return 1.72 * n * n;
	}
	public static void main(String[] args) {
		
		System.out.println(pnetagon(4));
	}
}
```
