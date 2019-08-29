# Dzen
using System;
 
namespace ConsoleApplication2
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("a=");
            int a= Convert.ToInt32(Console.ReadLine());
 
            Console.WriteLine("b=");
            int b= Convert.ToInt32(Console.ReadLine());
 
            Console.WriteLine("c=");
            int c= Convert.ToInt32(Console.ReadLine());
           
            int d=Math.Pow(b,2)-4*a*c;
            
            if(d<0) Console.WriteLine("Корней нет.");
            else
            {
                  int x1=-(b-Math.Sqrt(d))/2;
                  int x2=-(b+Math.Sqrt(d))/2;
                  if(x1=x2) Console.WriteLine("Один корень: x={0}",x1);
                  else Console.WriteLine("Два корня: x1={0}; x2={1}",x1,x2);
             }
        }
    }
}
