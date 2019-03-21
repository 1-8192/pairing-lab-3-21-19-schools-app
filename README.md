In this project you'll be creating a rails app to keep track of a school's students and teachers.


1. Create a new rails app called SchoolTracker.

2. Create three models: Student, Teacher, and School.

  - A school has many students and many teachers.
  
  - A teacher has many students, a student can have only one teacher.
  
  - A student can belong to only one teacher, and only belongs to one school.
  
3. Create a migration for each Model.

  Attributes:

  - school: name:string , location:string , year started:integer 
  
  - teacher: name:string, subject:string, years_teaching:integer
  
  - student: name:string, learning_method:string, age:integer, teacher_id:integer
  
4. Migrate your changes.

5. Create the relationships between your models (provided in Step 2).

6. Seed your database with data.

7. Make your controller actions & routes:

   - Create index, show, new, create, edit, update, and destroy actions for School.

   - Create index, show, new, create, and destroy actions for Teacher.
   
   - Create a new, create, destroy action for student.


8. Make your view pages.

- Have link to a teacher's view page in the school show page
- Have button within a teacher’s show page to delete or create a student
- Have link within teacher and school index page to create a new instance of a student or a teacher.
- Use a .collection_select to select the teacher instead of inputting a teacher’s name when creating a new student
   
   
9. Make validations for your models.

- teacher cannot have the same subject
- students cannot have the same name
- cannot have multiple schools with the same name, cannot have multiple schools with the same location
