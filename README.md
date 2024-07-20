//Compile Time Polymorphism
class Calculator{
    public int add(int a,int b)
    {
        return a+b;
    }
    public double add(double a,double b)
    {
        return a+b;
    }
}
public class Main
{
	public static void main(String[] args) {
		Calculator calc = new Calculator();
		System.out.println(calc.add(2,3));
		System.out.println(calc.add(2.5,3.5));
	}
}
//run time polymorphism
class Bike {
    void run()
    {
        System.out.println("running");
    }
}
class BMW extends Bike
{
    void run()
     {
         System.out.println("running with 100 km/hr");
     }
}
public class Main
{
    
     public static void main(String[] args)
     {
         Bike b = new BMW();
         b.run();
     }
}
