# Excel Medical Dataset 🏥

![](image.jfif)
---
## About the data

We are working with the medical record of students which includes their _age_, _gender_, _weight_, _height_, _BMI_, _Blood type_, _Temperature_, _Heart Rate_, _Blood Pressure_ and _Diabetis_, _Cholesterol_ and _smoking_ records.
---
## Data Cleaning
The dataset needs cleaning as there are a lot of empty cells in the dataset.

![](RawData.png)

- For the _student ID_ column, because the values are unique and in order, I created an _index column_ and replaced the _student ID_ column with it.
- For the _age_, _gender_, _Blood type_, _Temperature_, _eart Rate_, _Blood Pressure_ and _Diabetis_, _Cholesterol_ and _smoking_ columns, I simply **filled up** and **filled down** the values randomly.
- For the _weight_, _height_ and _BMI_ columns, I created a _custom column_ to calculate the _BMI_ using the formula `([Weight]/([Height]*[Height]))*10000`. I then used _conditional column_ to merge the original _BMI_ column and the _custom column_ into one so as to fill the missing cells.
- I repeated the process for the _weight_ column using the formula `([BMI F]*[Height]*[Height])/10000` and the _height_ column using the formula `Number.Sqrt([Weight F]/[BMI F])*100`.
- 
