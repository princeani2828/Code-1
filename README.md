import java.util.Scanner;
class Employee
{
	String name;
	int age;
	long number;
	String address;
	int salary;
	void print_salary()
	{
		System.out.println(salary+"\n");
	}
}
class Officer extends Employee
{
	String specialization;
}
class Manager extends Employee
{
	String department;
}
public class Main
{
	public static void main(String[] args)
	{
		Scanner obj= new Scanner(System.in);
		Officer obj1= new Officer();
		Manager obj2 = new Manager();
		System.out.print("Enter the name of the Officer: ");
		obj1.name=obj.nextLine();
		System.out.print("Enter the age of the Officer: ");
		obj1.age=obj.nextInt();
		System.out.print("Enter the salary of the Officer: ");
		obj1.salary=obj.nextInt();
		obj.nextLine();
		System.out.print("Enter the address of the Officer: ");
		obj1.address=obj.nextLine();
		System.out.print("Enter the phone number of the Officer: ");
		obj1.number=obj.nextLong();
		System.out.print("\nDetails of the Officer:\nName: "+obj1.name+"\nAge: "+obj1.age+"\nPhone Number: "+obj1.number+"\nAddress: "+obj1.address+"\nSalary: ");
		obj1.print_salary();
		obj.nextLine();
		System.out.print("Enter the name of the Manager: ");
		obj2.name=obj.nextLine();
		System.out.print("Enter the age of the Officer: ");
		obj2.age=obj.nextInt();
		System.out.print("Enter the salary of the Officer: ");
		obj2.salary=obj.nextInt();
		obj.nextLine();
		System.out.print("Enter the address of the Officer: ");
		obj2.address=obj.nextLine();
		System.out.print("Enter the phone number of the Officer: ");
		obj2.number=obj.nextLong();
		System.out.print("\nDetails of the Manager:\nName: "+obj2.name+"\nAge: "+obj2.age+"\nPhone Number: "+obj2.number+"\nAddress: "+obj2.address+"\nSalary: ");
		obj2.print_salary();
	}
}
