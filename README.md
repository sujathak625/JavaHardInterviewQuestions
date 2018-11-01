# JavaHardInterviewQuestions

This is to give some heads up on the advanced java interview questions. I have given answers for some and left blank for some. Welcome to accept
the mistakes or enhancements in the answers.

Try to be nice when pointing the mistakes.

These questions test not only the programming skill but also the approach, problem solving skill etc. technically and non-technically. 

There are lot of programmers around the world. Nowadays even a kid can program. But what makes a normal developer to stand out uniquely as pexrt
is their apprach to solve a problem.

Let us discuss few aspects. I will be updating as I encounter new topics and questions.

1. What are all the deisgn patterns you have used in your projects till now?

Almost aksed in all interviews. Depends upon your work experience.

2. What are SOLID design principles

SRP – Single Responsibility Principle.
OCP – Open/Closed Principle.
LSP – Liskov Substitution Principle.
ISP – Interface Segregation Principle.
DIP – Dependency Inversion Principle.

3. What are important transaction management aspects?

This is an indrect question. You are expected to answer about ACID properties.

4. Spring or Plain Java, which will be better for the web application development and why?

5. How to handle memory leak ?

This is a general question without specifcally asking about Garbage collections. You can talk about what you did to avoid garbage collection
such as closing of resource objects, using primitive data type than wrapper classes, using StringBuffer or StringBuilder
for dynamic string generation instead of "+" for Strinig concatenation, releasing the object by pointing them to null after its usage etc.

You can also talk about increasing the heap memery size in the JVM.

6. How do you handle delay in a web application? For example, your application is expected to responsd in 300 ms but it takes more time.
How will you debug it?

7. How two java client server application talk with each other without webservices?

8. How can we decide if Angular or Java Web application suitable for our application development needs?

9. Which collection you might consider when you want to maintain insertion order?

LinkedHastSet, LinkedHashMap maintains the insertion order.

10. How you will tune your database SQL query?

11. What is the use of Spring AOP?

12. How will consume REST webservices?


Sometimes we would prepare more in-depth and that we might lose track with most basic concept. 

13. Why String is immutable?

14. Can Static methods be overrided?

15. What are features added in Java 6, Java 7 and Java 8?   Asked in most of the interviews.

16. What is serialization? What are the methods involved in it?

17. Iterator or ListIterator? which will be your choice and why?

18. Why would you use ConcurrentHashMap against hashmap or which one is better?

19. Can non-static members be accessed in static methods?
No. But it can be accessed if a local instance is provided from the static method.

Does not work when,

public class Demo {
int i;

public static void main(String[] args) {
		Demo od = new Demo();
		i =1;		
	}

}

Works when scenario like below,

public class Demo {
int i;

public static void main(String[] args) {
		Demo od = new Demo();
		od.i =1;		
	}
}

20. Can static members be accessed in non-static methods?
Yes

