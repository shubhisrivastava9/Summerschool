# EAZYSCHOOL (THE BEST SUMMER CAMP FOR YOUR KID)

"Eazy School is a full-stack educational web application with separate roles for Admin and Students. Built with AWS RDS and deployed on AWS, it allows admins to manage enrollments and messages, while students can view their enrolled courses in a seamless interface."


![image](https://github.com/user-attachments/assets/1783cc45-494f-47bc-8455-620e9bdc337c)

![image](https://github.com/user-attachments/assets/71ae3999-b08f-4d10-905d-d2cffa258f4e)

![image](https://github.com/user-attachments/assets/8c48d5de-38c8-4682-99b3-e0953a7123e1)



LOGIN AND REGISTER 

BCryptPasswordEncoder (from Spring Security), used here for :

Encodes: It hashes the raw password using the BCrypt hashing algorithm with a random salt, producing a secure, irreversible encrypted string stored in the database.

Matches: During authentication, it takes the raw password entered by the user, hashes it again internally with the same salt, and compares it to the stored hashed password to verify if they match.



Admin and user both can login from here 

![image](https://github.com/user-attachments/assets/cff82207-a906-48da-a4c0-afa7e44bcb20)

Users can register from here 


![image](https://github.com/user-attachments/assets/9de12ea9-acd6-4629-8f8e-e7fab57ff32c)


IF I'M LOGGED IN AS A ADMIN


DASHBOARD

![image](https://github.com/user-attachments/assets/fc2c7ebb-ecf9-4464-aa8e-b2904f15ecc0)


PROFILE

ENTER CONTACT DETAILS

![image](https://github.com/user-attachments/assets/36082ecf-0c0a-4f45-a4db-39b97a2680bc)


MESSAGES

Pagination is implemented using Spring Data's Pageable interface and Page<Contact> return type in methods like findOpenMsgs, allowing fetching of a specific page of messages with size, number, and sorting info.

Sorting is applied via URL query parameters sortField and sortDir, which are passed into the controller and used in PageRequest.of(pageNum - 1, pageSize, Sort.by(...)) to dynamically sort the table columns (e.g., by name, mobile, subject).

![image](https://github.com/user-attachments/assets/5df80b55-e3e9-47b7-b76d-1b2edaa0fcf4)


Course tab

It shows how many courses are availible and we can see how many students are enrolled in each course.

![image](https://github.com/user-attachments/assets/d86276a8-bc29-4196-ae6d-59a8d6304948)

For ex- for physics class 

I can add students in any class.

![image](https://github.com/user-attachments/assets/0ba94805-57d6-4734-9c40-a7b2c0774915)



IF LOGIN AS STUDENT 

DASHBOARD

![image](https://github.com/user-attachments/assets/481c500c-fe58-4ce6-af8c-1bd048caa6bf)


User can see the how many courses he is enrolled in.

![image](https://github.com/user-attachments/assets/a33ca414-61d7-424b-8309-a7abdd2022e0)



