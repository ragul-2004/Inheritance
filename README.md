# Inheritance

## Aim:
 To write a C# program to print some messages using hierarchical inheritance.
## Algorithm:
### Step 1:
Create a base class.
### Step 2:
Create two child class.
### Step 3:
Create a constructor in the base class and print a message.
### Step 4:
Create a function in child class to print a message.
## Program:
```
using System;
namespace Autovechicle
{
    public class tyre
    {
        public tyre()
        {
            Console.WriteLine("Constructor tyre");
        }
        public virtual void Display()
        {
            Console.WriteLine("Tyre");
        }
    }
    public class scooter : tyre
    {
        public scooter()
        {
            Console.WriteLine("Constructor scooter");
        }

        public override void Display()
        {
            base.Display();
            Console.WriteLine("scooter");
        }
    }

    public class car : tyre
    {
        public car()
        {
            Console.WriteLine("Constructor car");
        }
        public override void Display()
        {
            base.Display();
            Console.WriteLine("car");
        }
    }

    public class Program
    {
        public static void Main(string[] args)
        {
            car cd = new car();
            scooter cdd = new scooter();
            cd.Display();
            cdd.Display();
        }
    }
}
```

## Output:
![ou](./1.png)

## Result
Thus to write a C# program to print some messages using hierarchical inheritance is executed successfully.
