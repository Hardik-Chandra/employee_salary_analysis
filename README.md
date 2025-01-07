# employee_salary_analysis

## Steps to run the project
- Create table salaries1
- Import the data from salary.csv.

## Query Description

```bash
  SELECT * FROM salaries1;
```
![image](https://github.com/user-attachments/assets/7a347d6d-87a1-4007-9f01-a9f174cfc0ca)

```bash
  SELECT EmployeeName,JobTitle from salaries1;
```
![image](https://github.com/user-attachments/assets/e00603f0-d905-4623-98df-0214f63986e5)

```bash
  SELECT count(Id) from salaries1;
```
![image](https://github.com/user-attachments/assets/a902d844-277b-48e0-9fbb-942e1c4e640b)

```bash
  SELECT distinct(JobTitle) from salaries1;
```
![image](https://github.com/user-attachments/assets/fa9f9349-982d-4f4a-bf36-02bc67bcb68c)

```bash
  SELECT JobTitle,OvertimePay from salaries1 where OvertimePay > 50000;
```
![image](https://github.com/user-attachments/assets/75f46ef1-1df3-4faf-8674-c48c78f36bf9)

```bash
  SELECT avg(BasePay) from salaries1;
```
![image](https://github.com/user-attachments/assets/bb224860-ff8f-4140-aaa8-159d5a44924a)

```bash
  SELECT TotalPay from salaries1 order by 'TotalPay' Desc limit 10;
```
![image](https://github.com/user-attachments/assets/e254659b-5407-48d0-b1fa-85e90fe55b7d)

```bash
  SELECT avg(BasePay),avg(OvertimePay),avg(OtherPay) from salaries1;
```
![image](https://github.com/user-attachments/assets/d8518184-e75e-4df7-bd11-990ede2bc685)

```bash
  SELECT EmployeeName,JobTitle from salaries1 where JobTitle like '%Manager%';
```
![image](https://github.com/user-attachments/assets/aceaf8bd-9ae4-43f8-a83a-cbdf50c99f2e)

```bash
  SELECT EmployeeName,JobTitle from salaries1 where JobTitle not like '%Manager%';
```
![image](https://github.com/user-attachments/assets/54c059a8-6ca0-4c1c-a1de-9015509eb447)

```bash
  SELECT EmployeeName from salaries1 where TotalPay between 50000 and 750000;
```
![image](https://github.com/user-attachments/assets/1f77d35a-2f3b-408a-9be6-865d9878d83e)

```bash
SELECT EmployeeName from salaries1 where BasePay < 50000 or TotalPay > 100000;
```
![image](https://github.com/user-attachments/assets/d860e854-67e8-4a1d-a511-8294f78b5773)

```bash
  SELECT EmployeeName,TotalPayBenefits from salaries1 where TotalPayBenefits between 125000 and 150000 and JobTitle like '%Director%';
```
![image](https://github.com/user-attachments/assets/20d110c4-eafb-420a-a7b1-ead1898241d4)

```bash
  SELECT EmployeeName from salaries1 order by TotalPayBenefits Desc;
```
![image](https://github.com/user-attachments/assets/c90136df-a8ee-4f5b-989a-8a156bdb8a1b)

```bash
  SELECT JobTitle,avg(BasePay) from salaries1 group by JobTitle having avg(BasePay) >= 100000 order by avg(BasePay) Desc;
```
![image](https://github.com/user-attachments/assets/92fc7ece-4e8d-439c-972f-b86efaf2e8e8)
