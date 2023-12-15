---
layout: project
type: project
image: img/download.jpg
title: "HR"
date: 2022
published: false
labels:
  - Java
summary: "I created a program that can add/delete employees and add certain information to their ID."
---

<div class="text-center p-4">

</div>

The Hr program will give you options based off what you want to do such as 1) Add employee 2) Remove employee 3) Print employees that earn a given amount 4) Print all the employees. Based off the option you choose there is a prompt that tells you what to do and it stores the information between each option.

Here is some code that shows how to remove an employee:

   public static Employee[] removeEmployee(Employee [] employeeArray) {  
      Scanner input = new Scanner(System.in);       
      int enumb = 0;
      System.out.println("Please enter the employee number you want to remove");
      try{
         enumb = input.nextInt();
      }  
      catch(InputMismatchException ime){
         System.out.println("Please enter the valid credentials");     
         return employeeArray;    
      }
      for(int i = 0; i < employeeArray.length; i++) {
         if(employeeArray[i] != null){
            if(employeeArray[i].getEnumb() == enumb){
               employeeArray[i] = null;
             
               System.out.println("You have removed the employee");                                               
            } 
         }
      }   
      return employeeArray;
