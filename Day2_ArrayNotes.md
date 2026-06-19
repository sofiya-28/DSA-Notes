# ARRAY-The Memmory Box
What will we learn?
In this chapter , we will understand:
* what is an Array?
* Why do we need Array?
* Array Index!
* Array length!
* Accessing Elements!
* Traversing an Array!

# -->A PROBLEM BEFORE ARRAY<--
Imagine you want to store marks of 5 students.
* WITHOUT ARRAY
Java:
int marks1 =85;
int marks2 =90;
int marks3 =78;
int marks4 =95;
int marks5 =87;

looks fine.
but what if there are 1000 students?
Creating 1000 variable is not practical.

# Array
Collection of same/similar  type of data store in a one veriable.
An Array is a container that store multiple value of the same type.
Array is a mutable becouse array changed the value of after declaration.
Java:
 >   int [] marks={ 85,90,78,95,87};
Now one variable store many values.
* >NOTE < without array hume har value ke liye alag se variable banana padta tha  par ab hum        array ka use kar ke ek he varible me sab value ko store kar sakte hai >

# why we need array ?
lets Suppose class ke 100 student ke marks store karne h to ye without array ye data store karna muskil h pr array ka use kar ke hum ye easily manage kar sakte h.
>    int[]arr= new int[100];

# Real Life Example!
Think of an Array as a school bag.
    [book1][book2][book3][book4]
Each space store one item.
Similarly:
[85][90][78][95][87]
Each position store one value.

# Characterstics of Array
*  Store same type of data.
*  fixed size.
*  Index Start from 0.
*  fast access using Index.

# Array index & Memory reprsentation.
Every element has a position.

* Array: 85 90 78 95 87 
* Value: 0  1  2  3  4 
* > NOTE< Array elements memory me continous (contiguous) locatio par store hote hain.>


> Important Rule 
* Array index always start from 0.
* last index of (Length-1).

# Creating an Array
* method 1
 >          int[]arr = {20, 30, 40 ,50};
* method 2
 >          int[]arr = new int[4];
output:
 >          [0][0][0][0]
      java automatically fills integer array with 0.(Default value of int 0)
      
# Accessing Array Elements
using Java:
>          int[] marks={10,70,50,68,40};
>          System.out.println(marks[2]);// what is 2 , it is a array index 
>          System.out.println(marks[4]);
>          System.out.println(marks[0]);//0 is always starting index

OUTPUT:
>      50
>      40
>      10

# Length of Array
>          System.out.println(marks.length);
OUTPUT:
>      5
# Updating Element 
>      marks[2]= 100;
OUTPUT:   
>      10
>      100
>      50
>      68
>      40

# Traversing an Array
Traversing means visiting every element one by one .
Java:
>          int[]arr={20,50,40,30,10};
>          for(int i=0; i<=arr.length;i++){
>              System.out.println(arr[i]);
           }

OUTPUT:
>      20
>      50
>      40
>      30
>      10

# Taking  input
>      Scanner sc=new Scanner(System.in);
>      int[]arr =new int[5];
>      for(int i=0;i<arr.length;i++){
>      arr[i]=sc.nextInt();
>      }
#  Time Complexity
* operation              Complexity
* Access                 O(1)
* Update                 O(1)
* Search                 O(n)
* Traversal              O(n)

>NOTE < Why access is O(1)  : Because array store elements continously and index directly points to memory location >

# why are Arrays Important?
Array are the foundation of DSA.
Many problem are based on Arrays:
* Searching
* Sorting
* Finding Largest
* Finding Smallest Element
* Sum of Element
