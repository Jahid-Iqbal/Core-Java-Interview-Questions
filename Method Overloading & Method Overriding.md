1. Can we overload the main method?
Ans: Yes. But JVM compiles only the main that receives the String array as parameter.

```java
public class ChildPractice extends Practice {

	public static void main(String args) {
		System.out.println("String="+args);
		
	}
	
	public static void main(String[] args) {
		ChildPractice p= new ChildPractice();
		p.main("Hello");    //String=Hello
	}

}
```