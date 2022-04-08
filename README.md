# c-sharp

	Write a c# code to show even numbers between 1 to 10:
using System;
namespace looping
{
    class Program
    {
        static void Main(string[] args)
            
        {
            int i = 1;
            for (i = 1; i <= 10; i++)
            {
                if (i % 2 == 0)
                {
                    Console.WriteLine(i);
                }
            }
            Console.ReadLine();
        }
    }
}

using System;
namespace looping
{
    class Program
    {
        static void Main(string[] args)
            
        {
            int i = 1, a;
            Console.WriteLine("Enter the last integer upto the even numbers you want: ");
            a=int.Parse(Console.ReadLine());
            for (i = 1; i <= a; i++)
            {
                if (i % 2 == 0)
                {
                    Console.WriteLine(i);
                }
            }
            Console.ReadLine();
        }
    }
}

	Using break:
using System;
namespace looping
{
    class Program
    {
        static void Main(string[] args)
            
        {
            int i = 1, a;
            Console.WriteLine("Enter the last integer upto the even numbers you want: ");
            a=int.Parse(Console.ReadLine());
            for (i = 1; i <= a; i++)
            {
                if (i % 2 == 0)
                {
                    if (i > 6)
                    {
                        break;
                    }
                    Console.WriteLine(i);
                }
            }
            Console.ReadLine();
        }
    }
}

	Continue:
using System;
namespace looping
{
    class Program
    {
        static void Main(string[] args)
            
        {
            int i = 1, a;
            Console.WriteLine("Enter the last integer upto the even numbers you want: ");
            a=int.Parse(Console.ReadLine());
            for (i = 1; i <= a; i++)
            {
                if (i % 2 == 0)
                {
                    if (i <= 6)
                    {
                        continue;
                    }
                    Console.WriteLine(i);
                }
            }
            Console.ReadLine();
        }
    }
}

	Break in while loop:
using System;
namespace whileloop
{
    class Program
    {
        static void Main(string[] args)
        {
            int i = 1, a;
            Console.WriteLine("Enter the last integer upto the even numbers you want: ");
            a = int.Parse(Console.ReadLine());
            while (i <= a)
            {
                if (i % 2 == 0)
                {
                    if (i > 6)
                    {
                        break;
                    }
                    Console.WriteLine(i);
                }
                i++;
            }
            Console.ReadLine();
        }
    }
}


	Class and object:
using System;
namespace functionarr
{
    class Program
    {
        void show()
        {
            Console.WriteLine("new function is invoked!");
            Console.ReadLine();
        }
        static void Main(string[] args)
        {
            Program msg = new Program();
            msg.show();
        }
    }
}

	Array:
using System;
namespace functionarr
{
    class Program
    {
        void show()
        {
            int[] a = {1,2,3,4,5};
            Console.WriteLine("new function is invoked!");
            Console.WriteLine(a[3]);
            Console.ReadLine();
        }
        static void Main(string[] args)
        {
            Program msg = new Program();
            msg.show();
        }
    }
}



Addition of Array Elements:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace function
{
    class Program
    {
           int i,sum;

        void print()
        {
         
            int[] a = { 12,23,65,45};
     
            for ( i = 0; i < 4; i++)
            {
               sum= sum + a[i];
            }
            Console.WriteLine(sum);
            Console.ReadLine();
        }

        static void Main(string[] args)
        {
            Program m1 = new Program();
            m1.print();
        }
    }
}

Check Maximum Number from Array 

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
namespace function
{
    class Program
    {
           int i,sum,temp, j, greater;
           int[] a = { 12, 23, 65, 45 };
           void print()
           {
              for (i = 0; i < 4; i++)
               {
                   sum = sum + a[i];
               }
               Console.WriteLine(sum);
           }
           void max()
           {
               for (i = 0; i < 4; i++)
               {
                   if (a[i] > greater)
                   {
                       greater = a[i];
                   }
                   else
                   {
                       Console.WriteLine(greater);
                   }
               }
           }

        static void Main(string[] args)
        {
            Program m1 = new Program();
            m1.print();
            m1.max();
            Console.ReadLine();
        }
    }
}

Default Constructor

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace constructor
{
    class defconstructor
    {
        defconstructor()
        {
            Console.WriteLine("Cunstructor called.");
        }
        static void Main(string[] args)
        {
            defconstructor d1 = new defconstructor();
            Console.ReadLine();
        }
    }
}
Parameteraise Constructor

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace constructor
{
    class defconstructor
    {
        defconstructor( int a, int b)
        {
            int c = a + b; ;
            Console.WriteLine(c);
           
        }
        static void Main(string[] args)
        {
            defconstructor d1 = new defconstructor(12,12);
            Console.ReadLine();
        }
    }
}

Or

Parameterise Constructor at Runtime:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace constructor
{
    class parconstructor
    {
        int c;
        parconstructor(int a, int b)
        {
            c = a + b;
        }
        static void Main(string[] args)
        {
            parconstructor d1 = new parconstructor(12, 12);
            Console.WriteLine(d1.c);
            Console.ReadLine();
        }
    }
}

Destructor:
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace constructor
{
    class defconstructor
    {
        defconstructor()
        {
            Console.WriteLine("Cunstructor called.");
        }
      ~defdistructor()
        {
           Console.WriteLine(“Destructor called”);
           Console.ReadLine();
        }
        static void Main(string[] args)
        {
            defconstructor d1 = new defconstructor();
            
        }
    }
}

	Write a C#.Net Program to accept user Define Number and print table of given number. Value should be accept as early class objects created
(It means Using parameterize Constructor).

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace constructorexample
{
    class table
    {
       
        table(int a)
        {
          
       
            Console.WriteLine("table of  "+a+ " is:");
            for (int i = 1; i <= 10; i++)
            {
               
                Console.WriteLine( a * i);

            }
        }
        static void Main(string[] args)
        {
            int num;
              Console.WriteLine("Enter the number: ");
            num = int.Parse(Console.ReadLine());
            table t1 = new table(num);
            Console.ReadLine();
        }
    }
}

	Write a C#.Net Program to accept user Define Number and print table of given number. Value should be accept as early class objects created 
(It means Using parameterize Constructor)
and Object should free memory spaces after program execution completed(It means Using Destructor).

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
namespace table
{
    class table
    {
        int num;
        table(int a)
        {
            Console.WriteLine("table of "+a+" is: \n");
            for (int i = 1; i <= 10; i++)
            {
                Console.WriteLine(a*i);
            }
            Console.ReadLine();
        }
        ~table()
        {
            Console.WriteLine("Destructor called.");
            Console.ReadLine();
        }
        static void Main(string[] args)
        {
            int num;
            Console.WriteLine("Enter a number to print it's table: ");
            num = int.Parse(Console.ReadLine());
            table t1 = new table(num);    
        }
    }
}


	Single Inheritance
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace inheritance
{
    public class stud
    {
        public string name = "chetan";

        public string class1 = "sybca";
    }
        class exam : stud
        {
            public string sub = "math";
           public void display()
            {
                Console.WriteLine(" Name= " + name + " class= " + class1 + " subject " + sub);
                Console.ReadLine();
            }
        }
        class program
        {
            static void Main(string[] args)
            {
                exam s1 = new exam();
                //  s1.show();
                s1.display();
            }
        }
    }


	Demonstration Multilevel Inheritance:

using System;
namespace inheritance
{
    public class stud
    {
        public string name="Manish";
        public string class1="SYBCA";
        public void showinfo()
        {
            Console.WriteLine("Name= " + name + " Class= " + class1);
  
        }
    }
    public class exam: stud
    {
        public void showsub()
        {
        string sub="C#.Net";
        Console.WriteLine("Subject= "+sub);
        }
    }
    public class mark : exam
    {
        public void showmarks()
        {
            int marks = 50;
            Console.WriteLine("Marks= " + marks);
            Console.ReadLine();
        }
    }

    class Program
    {
        static void Main(string[] args)
        { 
            mark mk=new mark();
            mk.showinfo();
            mk.showsub();
            mk.showmarks();
        }
    }
}


	Demonstration of Interface:

using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace @interface
{
    class student
    {
        public string name;
        public string class1;
        public void showinfo() 
        {
            name = "Chetan";
            class1 = "SYBCA";
            Console.WriteLine("Student Name: " + name);
            Console.WriteLine("Class:" + class1);
        }
    }
    interface exam
    {
        
        void showsub();
    }
    class result:student,exam
    {
         
        
        public void showsub()
        {
            
            Console.WriteLine("C#.net");
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            result r1 = new result();
            r1.showinfo();
            r1.showsub();
            Console.ReadLine();
        }
    }
}

Demonstration Method Overloading:
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace methodoverloading
{
    class demo
    {
        public int c, d;

        public void sum(int a, int b)
        {
            c = a + b;
            Console.WriteLine(c);
        }
        public void sum(int a, int b, int e)
        {
            d = a + b + e;
            Console.WriteLine(d);
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            demo d1 = new demo();
            d1.sum(2,4,6);
            d1.sum(5,10);
            Console.ReadLine();
        }
    }
}

Demonstration of Method Overriding:
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;

namespace methooverriding
{
    class demo
    {
        public void display()
        {
            Console.WriteLine("Hundai i20");
        }
    }
    class demo2 : demo
    {
        public void display()
        {
            Console.WriteLine("Mahendra Scorpio");
        }
    }
    class Program
    {
        static void Main(string[] args)
        {
            demo2 d = new demo2();
            d.display();
            Console.ReadLine();
        }
    }
}

