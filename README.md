# Databases

<h3>Warehouse of books</h3>
<p><strong>Task</strong>:<br />The name of the book, its author, the number of copies in stock and its price are known. All this information can be presented in the form of a table consisting of 4 columns (only 4 records are given, in fact there are much more of them):<br />Название&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Автор&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Цена, руб&nbsp;&nbsp; Количество<br />Мастер и Маргарита&nbsp; Булгаков М.А.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 670.99&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3<br />Белая гвардия&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Булгаков М.А.&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 540.50&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 5<br />Идиот&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Достоевский Ф.М.&nbsp;&nbsp;&nbsp; 460&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 10<br />Братья Карамазовы&nbsp;&nbsp; Достоевский Ф.М.&nbsp;&nbsp;&nbsp; 799.01&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2</p>
<h3>Online book store</h3>
<p><strong>Task</strong>:<br />The online store sells books. Each book has a title, is written by one author, belongs to one genre, has a certain price. There are several copies of each book available in the store. <br />The buyer registers on the website of the online store, sets his first and last name, e-mail and city of residence. He can form one or several orders, write some wishes for each order. Each order includes one or more books, each book can be ordered in several copies. Then the order goes through a series of successive stages (operations): it is paid, packed, transferred to a courier or a transport company for transportation and, finally, delivered to the buyer. The date of each operation is fixed. The average delivery time of books is known for each city.<br />At the same time, the store keeps records of books, their quantity decreases when buying, increases when the goods arrive, when the quantity is exhausted, an order is placed, and so on.</p>
<h3>Testing</h3>
<p><strong>Task</strong>:<br />The university implements on-line testing in several disciplines. Each discipline includes a certain number of questions. The answers to the question are presented in the form of answer options, one of these options is correct.<br />
The student registers in the system by specifying his first name, last name and patronymic. After that, he can be tested in one or more disciplines. The student has several attempts to pass the test (it is necessary to save the date of the attempt). Each student is randomly selected a set of questions on the discipline and an individual test is formed. The student answers the questions by choosing one of the suggested answers.<br />
After the end of testing, the result (in percent) of the attempt is calculated and stored.<br />
Queries for the subject area:<br />
Bring out students who have passed a certain discipline.<br />
Print the number of attempts and the average result for each discipline.<br />
Output the student(s) who scored the highest score during testing.<br />
If a student has made several attempts in the same discipline, then print the difference in days between the first and last attempt.<br />
Print the number of students who have been tested in each discipline.<br />
Randomly select 3 questions on a certain discipline.<br />
Output the questions that a certain student answered in a certain attempt, the student's answer and the result (correct or not).<br />
Calculate the test results for all attempts.<br />
For each question, print the percentage of successful solutions and the total number of answers.</p>
<h3>Entrant</h3>
<p><strong>Task</strong>:<br />The university consists of a set of faculties (schools). Applicants are enrolled in educational programs based on the results of the Unified State Exam (USE). Each educational program belongs to a certain faculty, the USE subjects necessary for admission, the minimum score in these subjects, as well as the recruitment plan (number of places) are determined for it for an educational program.<br />Applicants apply to the admissions committee for an educational program, each applicant can choose several educational programs (but no more than three). The application indicates the applicant's surname, first name, patronymic, as well as his achievements: whether he received a medal for studying at school, whether he has a TRP badge, etc. At the same time, an additional point is determined for each achievement. The applicant provides a certificate with the results of passing the Unified State Exam. If an applicant chooses an educational program, then he must have passed the subjects defined for this program, and the score must be at least the minimum for this subject.<br />Enrollment of applicants is carried out as follows: first, the sum of points in subjects for each educational program is calculated, achievement points are added, then applicants are sorted in descending order of the sum of points and the first ones are selected according to the number of places determined by the recruitment plan.</p>
<h3>Educational analytics for the course</h3>
<p><strong>Task</strong>:<br />The course on the Stepik platform consists of several modules, each module includes several lessons, for each lesson information about its position in the module is stored. Each lesson consists of a sequence of steps. Each step has its own type (it can be text, SQL task, etc.) and also a sequence number in the lesson.<br />Users register for the course, indicate their name. When a user takes a course on the Stepik platform, all his actions leave a "digital footprint": what tasks and when he completed, how many attempts he made, whether he solved the task correctly. All his comments are also stored. If a user takes a course and receives a certificate, the date of its issuance is saved. All this information is primary for educational analytics.<br />Educational analytics is the measurement, collection, analysis and presentation of data about students and their actions on an online platform in order to understand and optimize the educational process and the environment where this process takes place.<br />For this lesson, a database was created with a full description of the course structure. Educational analytics is not fully included in the database, but only for a certain group of users due to the large amount of data. For example, information about the decisions of 17,000 users of our course for six months of its existence contains 534,500 records.<br />We selected the users for the lesson database as follows:</p>
<ul>
<li>&nbsp;&nbsp;&nbsp; we rejected all those who did not complete any tasks (there were 8800 of them);</li>
<li>&nbsp;&nbsp; &nbsp;we grouped the remaining users depending on the number of solved tasks, that's what happened (we believe that those who did not send tasks for more than a month left the course):</li>
</ul>
<p>&nbsp;&nbsp;&nbsp; Всего&nbsp;&nbsp; &nbsp;Закончили обучение или покинули курс&nbsp;&nbsp; &nbsp;Активные пользователи<br />&nbsp;&nbsp; &nbsp;Выполнили все задания&nbsp;&nbsp; &nbsp;116&nbsp;&nbsp; &nbsp;75&nbsp;&nbsp; &nbsp;41<br />&nbsp;&nbsp; &nbsp;Получили сертификат&nbsp;&nbsp; &nbsp;617&nbsp;&nbsp; &nbsp;470&nbsp;&nbsp; &nbsp;147<br />&nbsp;&nbsp; &nbsp;Третий модуль&nbsp;&nbsp; &nbsp;225&nbsp;&nbsp; &nbsp;220&nbsp;&nbsp; &nbsp;5<br />&nbsp;&nbsp; &nbsp;Второй модуль&nbsp;&nbsp; &nbsp;940&nbsp;&nbsp; &nbsp;762&nbsp;&nbsp; &nbsp;178<br />&nbsp;&nbsp; &nbsp;Первый модуль, 5-7 урок&nbsp;&nbsp; &nbsp;1077&nbsp;&nbsp; &nbsp;891&nbsp;&nbsp; &nbsp;186<br />&nbsp;&nbsp; &nbsp;Первый модуль, 4 урок&nbsp;&nbsp; &nbsp;701&nbsp;&nbsp; &nbsp;589&nbsp;&nbsp; &nbsp;112<br />&nbsp;&nbsp; &nbsp;Первый модуль, 3 урок&nbsp;&nbsp; &nbsp;823&nbsp;&nbsp; &nbsp;670&nbsp;&nbsp; &nbsp;153<br />&nbsp;&nbsp; &nbsp;Первый модуль, 2 урок&nbsp;&nbsp; &nbsp;1268&nbsp;&nbsp; &nbsp;1044&nbsp;&nbsp; &nbsp;224<br />&nbsp;&nbsp; &nbsp;Первый модуль, 1 урок&nbsp;&nbsp; &nbsp;2430&nbsp;&nbsp; &nbsp;2020&nbsp;&nbsp; &nbsp;410</p>
<ul>
<li>&nbsp;&nbsp;&nbsp; then the typical representatives of the groups were selected more or less proportionally to the number of each group (the user names, of course, were replaced);</li>
<li>&nbsp;&nbsp;&nbsp; since users sent from 1 to 1000 solutions during the course, only attempts of steps related to lessons 1.2, 2.2 and 2.4 were included in the database.</li>
</ul>
<p>It turned out 64 users and more than 2000 of their attempts.<br />The grouping and sampling of each group usually depends on the goals of the study, for example, if you need to understand when and for what reason users leave the course, then a more "small" division is needed for the initial steps.</p>
<h3>Business trips</h3>
<p><strong>Task</strong>:<br />Trip table, which provides information about the business trips of employees of some organization (the employee's last name, the city where he went, the amount of the daily allowance, the dates of the first and last day of the business trip)</p>
<h3>Traffic violations</h3>
<p><strong>Task</strong>:<br />The fine table provides information on fines accrued to drivers for traffic violations (driver's name, car number, description of the violation, the amount of the fine, the date of the violation and the date of payment of the fine)</p>
<p><strong>Manual</strong>:<br />I started the database in the Ubuntu 20.04 terminal.</p>
<ol>
<li>To work in the system, you need to install postresql in the terminal in this way:
<br />u@uv:~$ sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" &gt; /etc/apt/sources.list.d/pgdg.list'<br />u@uv:~$ wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -<br />u@uv:~$ sudo apt-get update<br />u@uv:~$ apt list | grep postgresql<br />u@uv:~$ sudo apt-get -y install postgresql<br />u@uv:~$ systemctl status postgresql
<li>To start the program, you need to enter the following commands in the terminal:
<br />:~$ sudo mysql -u root<br />mysql&gt; CREATE DATABASE testbdserver;<br />mysql&gt; \q<br />:~$ mysql -u root -p testbdserver &lt; data-dump0.sql
<br />:~$ sudo su - postgres<br />postgres@uv:~$ psql
</li>
</ol>
<p><strong>Tools</strong>:</p>
<ol>
<li>Ubuntu 20.04</li>
<li>mysql</li>
</ol>
<p><strong>Source</strong>:</p>
<ol>
<li><a href="https://www.asozykin.ru/courses/sql" target="_blank">asozykin</a></li>
</ol>