---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "HR"
date: 2022
published: true
labels:
  - Java
summary: "I created a program that can add/delete employees and add certain information to their ID."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

The Hr program will give you options based off what you want to do such as 1) Add employee 2) Remove employee 3) Print employees that earn a given amount 4) Print all the employees. Based off the option you choose there is a prompt that tells you what to do and it stores the information between each option.

Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
