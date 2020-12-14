# stack

package com;

public class day2
{
	public static void main(String []args)
	{
		day2 obj=new day2();
		obj.push(1);
		obj.push(2);
		obj.push(3);
		obj.push(4);
		obj.push(5);
		obj.pop();
		obj.push(100);
		
		obj.display();
	}
	 int size=6;
	 int[] arr=new int[size];
	 int rear=-1;
	 int front=-1;
	 void push(int ele)
	 {
		 if(rear==size-1)
		 {
			 System.out.println("stack is full");
		 }
		 else
		 {
			 rear++;
			 arr[rear]=ele;
		 }
	 }
	 void pop()
	 {
		 if(rear==-1)
		 {
			 System.out.println("stack is empty");
		 }
		 else
		 {
			 rear--;
		 }
		 
	 }
	 void display()
	 {
		 for(int i=0;i<=rear;i++)
		 {
			 System.out.println(arr[i]);
		 }
	 }
}
