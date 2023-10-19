import java.util.Scanner;

 class Employee

 {

    String name,address;

    int age,salary;

    long number;

    void print_salary()

   {

     System.out.println(salary+"\n");

   }

}

 class Officer extends Employee

 {

	 String specialization;

  Officer(String name , int age, long number , String address ,int salary , String specialization)

  {

	  this.name=name;

	  this.age=age;

	  this.number=number;

	  this.salary=salary;

	  this.address=address;

    this.specialization=specialization;

  }

 }

 class Manager extends Employee

 {

  String department;

  Manager(String name , int age, long number , String address ,int salary , String department)

  {

	  this.name=name;

	  this.age=age;

	  this.number=number;

	  this.salary=salary;

	  this.address=address;

    this.department=department;

  }

 }

 public class Empl

 {

  public static void main(String[] args)

  {

   Scanner obj= new Scanner(System.in);

   System.out.print("Enter the name of the Officer: ");

   String name=obj.nextLine();

   System.out.print("Enter the age of the Officer: ");

   int age=obj.nextInt();

   System.out.print("Enter the salary of the Officer: ");

   int salary=obj.nextInt();

   obj.nextLine();

   System.out.print("Enter the address of the Officer: ");

   String address=obj.nextLine();

   System.out.print("Enter the phone number of the Officer: ");

   long number=obj.nextLong();

   obj.nextLine();

   System.out.print("Enter the specialization of the Officer: ");

   String specialization=obj.nextLine();

   Officer obj1= new Officer( name ,  age, number ,  address , salary ,specialization);

   System.out.print("\nDetails of the Officer:\nName: "+obj1.name+"\nAge: "+obj1.age+"\nPhone Number: "+obj1.number+"\nSpecialization:"+obj1.specialization+"\nAddress: "+obj1.address+"\nSalary: ");

   obj1.print_salary();

   System.out.print("Enter the name of the Manager: ");

   name=obj.nextLine();

   System.out.print("Enter the age of the Officer: ");

   age=obj.nextInt();

   System.out.print("Enter the salary of the Officer: ");

   salary=obj.nextInt();

   obj.nextLine();

   System.out.print("Enter the address of the Officer: ");

   address=obj.nextLine();

   System.out.print("Enter the phone number of the Officer: ");

   number=obj.nextLong();

   obj.nextLine();

   System.out.print("Enter the department of the Officer: ");

   String department=obj.nextLine();

   Manager obj2=new Manager( name ,  age,  number ,  address , salary , department);

   System.out.print("\nDetails of the Manager:\nName: "+obj2.name+"\nAge: "+obj2.age+"\nPhone Number: "+obj2.number+"\nAddress: "+obj2.address+"\nDepartment:"+department+"\nSalary: ");

   obj2.print_salary();

  }

 }

