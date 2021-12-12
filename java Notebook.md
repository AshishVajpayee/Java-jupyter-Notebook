### Hello World First Java program


```Java
System.out.println("Hello World !!");
```

    Hello World !!


### Printing Multiple print Statements


```Java
System.out.println("Good Morning !!");
System.out.println("Have a nice day");
```

    Good Morning !!
    Have a nice day
    

### Using Variable to store data/value and printing value using variable.


```Java
String name = "Ashish"; // Here var name holds string datatype i.e, Ashish
System.out.println("My Name is "+name); //prints the value stored in var name
```

    My Name is Ashish



```Java
String name = "Ashish";
int age = 22;
System.out.println("My name is " +name+ ", I am " +age+ " years old");
```

    My name is Ashish, I am 22 years old


### Comments in Java


```Java
/* text ignored with in the this */
/** Documentation **/
// Single Line Comment
System.out.println("Comment example");
```

    Comment example


### Data Types in java


```Java
byte a = 1; //Byte datatype
short s = 10000; //short datatype
String name = "Ashish"; //String datatype
int age = 22; // Integer datatype
char sex = 'M'; // character datatype
long phone = 1234567890; 
float salary = 500000.866f; // Float datatype
boolean isStudent = true; // Boolean datatype
System.out.println(a);
System.out.println(s);
System.out.println(name);
System.out.println(age);
System.out.println(sex);
System.out.println(phone);
System.out.println(salary);
System.out.println(isStudent);

```

    1
    10000
    Ashish
    22
    M
    1234567890
    500000.88
    true
    

### Types of Variable


```Java
{
    //instance vairable
    int data = 50;
    System.out.println("instance Var: "+data);
    
    //static varibale
    int m = 100;
    
    System.out.println("Static Var: "+m);


}
void Method()
    {
        //local variable
        int n = 90;
        System.out.println("Local Variable"+n);
    }//end of class
```

    instance Var: 50
    Static Var: 100
    

### Decision Making


```Java
// if statement consists of a boolean expression followed by one more statements
{
    int i = 5;
    if(i<10)
    {
        System.out.println("This is if Statement");  // when ever condition is true the code with in the if block gets executed
    }
    
}
```

    This is if Statement



```Java
/** Here if condition is true, the code which is written inside if block gets executed.
Else if the condition is false, the code inside if block gets executed **/

{
    int test = 10;
    
    if(test > 5)
    {
        System.out.println("Success");
    }
    else
    {
       System.out.println("Failure"); 
    }
    
    System.out.println("Executed Successfully");
}
```

    Success
    Executed Successfully
    


```Java
// IfElseLadder 

{
    
    int test;
    Scanner sc = new Scanner(System.in);
    System.out.println("Enter the number 1/2/3: ");
    test = sc.nextInt();
    if(test == 1)
    {
        System.out.println("Hello");
    }
    else if(test == 2)
    {
       System.out.println("Welcome"); 
    }
    else if(test == 3)
    {
       System.out.println(":D"); 
    }
    else
    {
    System.out.println("No Match Found");
    }
}
```

    Enter the number 1/2/3: 
    2
    Welcome
    


```Java
int x = 60;
int y = 40;
if(x == 60)
{
    if(y == 40)
    {
        System.out.println("X = 60 and Y = 40");
    }
}// if both the if condition are true then this block prints 
```

    X = 60 and Y = 40


### Switch Statement


```Java
Scanner input = new Scanner(System.in);
System.out.println("Menu");
System.out.println("1. Start");
System.out.println("2. Resume");
System.out.println("3. Load \n4. Exit");

int choice = input.nextInt();

switch(choice)
{
    case 1:
        System.out.println("Starting the Game for you..");
        break;
    
    case 2:
        System.out.println("Resuming game..");
        break;
        
    case 3:
        System.out.println("Loading the Game for you..");
        break;
        
    case 4:
        System.exit(0);
        break;
        
    default:
        System.out.println("Invalid Input!!");
        break;
}

```

    Menu
    1. Start
    2. Resume
    3. Load 
    4. Exit
    1
    Starting the Game for you..
    

### Loops


```Java
/** There may be a situation when we need to execute a block of code several number of times, and is often
refered to as loop **/
// The code within a while loop will execute while specified condition is true

int num = 0;

while(num < 10)
{
    num = num + 2;
    System.out.print(num + " "); // Once value of num is greater than 10, the loop will stop executing
}
```

    2 4 6 8 10 


```Java
// do while loop
int num = 5;
do {
    num = num + 2;
    System.out.print(num + " ");
}
while(num < 20);
```

    7 9 11 13 15 17 19 21 


```Java
// for Loop

for(int a = 1; a < 11; a++) //var a is dec with val of 1, a<11 states as long as the var a is less than 11, the loop shld keep running,  a++ states that for every iteration of the loop a shld increase by 1.
{
    System.out.print(a + " "); //to print in a single line instead of multiple line remove ln from print statement
}
```

    1 2 3 4 5 6 7 8 9 10 


```Java
// enhanced for loop
int [] numbers = {10, 20, 30, 40};

for(int x: numbers)
{
    System.out.print(x);
    System.out.print(",");
}
System.out.print("\n");

String [] names = {"James", "Larry", "Tom", "John"};

for(String name: names)
{
    System.out.print(name);
    System.out.print(",");
}
```

    10,20,30,40,
    James,Larry,Tom,John,

## Arrays
#### Array is a data-structure, which stores a fixed-size sequential collection of elements of the same type. 
<ul> <li> Each item in an array is called an element, and each element is accessed by its numerical index. </li>
    <li> First element of the array is stored at 0 index.
  </ul>
<p> Array declaration has two parts: </p>
<ol>
    <li><b>Array's type</b></li>
    <li><b>Array's name</b></li>
</ol>
<ul>
    <li><b>Array's type</b> is written as type[], where type is data type of the contained elements, the brackets are special symbols indicating that this variable holds an array.</li>
    <li><b>Array's name</b> can be anything you want</li>
</ul>


```Java
// Array Examples

//declares an array of integers
int[] anArray;

//allocates memory for 5 integers
anArray = new int[5];

//init first element
anArray[0] = 100;

//init second element
anArray[1] = 200;

//and so on
anArray[2] = 300;
anArray[3] = 400;
anArray[4] = 500;

System.out.println("Element at index 0: "+ anArray[0]);
System.out.println("Element at index 1: "+ anArray[1]);
System.out.println("Element at index 2: "+ anArray[2]);
System.out.println("Element at index 3: "+ anArray[3]);
System.out.println("Element at index 4: "+ anArray[4]);
```

    Element at index 0: 100
    Element at index 1: 200
    Element at index 2: 300
    Element at index 3: 400
    Element at index 4: 500
    


```Java
//Multi-Dimensional Arrays

String[][] names = {
    //first list
    {"Mr. ", "Mrs. ", "Ms. "},
    //second list
    {"walker", "granger"}
};
// Mr. walker
System.out.println(names[0][0] + names[1][0]);
// Ms. granger
System.out.println(names[0][2] + names[1][1]);



```

    Mr. walker
    Ms. granger
    

### Armstrong Number


```Java
int number, result = 0, q, rem;

Scanner input = new Scanner(System.in);
System.out.println("Enter a Number to check if it is an Armstrong number: ");
number = input.nextInt();

q = number;

while(q != 0)
{
    rem = q%10;
    result = result + rem*rem*rem;
    q = q/10;
}

if(number == result)
{
    System.out.println("Entered number is an armstrong number.");
}
else
{
    System.out.println("Entered number is not an armstrong number.");
}
```

    Enter a Number to check if it is an Armstrong number: 
    371
    Entered number is an armstrong number.
    

### Check whether Number is Prime


```Java
int number, res;
boolean flag = true;
Scanner input = new Scanner(System.in);
System.out.println("Please Enter a Number: ");

number = input.nextInt();
for(int i = 2; i <= number/2; i++)
{
    res = number%i;
    if(res == 0)
    {
        flag = false;
        break;
    }
}

if(flag)
    System.out.println(number+ " is Prime Number");
else
    System.out.println(number+ " is Not Prime Number");
```

    Please Enter a Number: 
    5
    5 is Prime Number
    

### Factorial Number


```Java
int fact=1;
int number = 0;

Scanner in = new Scanner(System.in);
System.out.println("Enter the Number: ");
number = in.nextInt();

for(int i = 1; i <= number; i++)
{
    fact = i*fact;
}

System.out.println("The factorial of "+number+ " is " +fact);
```

    Enter the Number: 
    6
    The factorial of 6 is 720
    

### SquareRoot of a Number


```Java
int n;
Scanner in = new Scanner(System.in);
System.out.println("Enter Number: ");
n = in.nextInt();
System.out.println(Math.sqrt(n));
```

    Enter Number: 
    49
    7.0
    

### Binary To Decimal


```Java
BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
System.out.print("Enter Binary no. to convert in Decimal: ");
String number = br.readLine();

int decimalNumber = Integer.parseInt(number, 2);
System.out.println("Binary number converted to decimal number");
System.out.println("Decimal number is: "+decimalNumber);
```

    Enter Binary no. to convert in Decimal: 1010
    Binary number converted to decimal number
    Decimal number is: 10
    


```Java

```
