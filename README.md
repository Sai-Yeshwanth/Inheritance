class A{
	String name="Amazon";
	float area = 10000;
	public void nam()
	{
		System.out.println("Name of forest is "+ name);
	}
	public void size()
	{
		System.out.println("Size of forest is " + area);
	}
	public void info()
	{
		System.out.println("Many Trees grow here....");
	}
}
class B extends A{
	String name="Coconut";
	int ht = 5;
	public void name()
	{
		System.out.println("Name of tree is "+ name);
	}
	public void height()
	{
		System.out.println("Height of tree is " + ht);
	}
	public void info()
	{
		System.out.println("Many coconuts grow here....");
	}
}
class C extends A{
	String name="Pond";
	double lt = 1500;
	public void names()
	{
		System.out.println("Name of liquid body is "+ name);
	}
	public void capacity()
	{
		System.out.println("No. of litres is " + lt);
	}
	public void info()
	{
		System.out.println("The water here is fresh....");
	}
}

public class Jala {

	public static void main(String[] args) {
		A a = new A();
		a.nam();
		a.size();
		a.info();
		
		B b = new B();
		b.name();
		b.height();
		b.info();   //overridden
		
		C c = new C();
		c.names();
		c.capacity();
		c.info();   //overridden
		
		c.nam();   //function of class A called from object c
		
		
	}
}

