# java
static keyword
class usestatic
    {
        static int a=3;
        static float b;
        int c=9;
        static void met1()
        {
            System.out.println("\n outer class static method");
            System.out.println("\n enter the value a:"+a);
            System.out.println("\n enter the value b:"+b);
        }
        static void met2()
        {
            System.out.println("\n outer class non-static method");
            System.out.println("value of c is:");
        }
        static
        {
            System.out.println("in static block");
            b=a*66;
        }
    }
    class Main
        {
            public static void main(String args[])
            {
                usestatic.met1();
                usestatic s=new usestatic();
                s.met2();
            }
        }
    
