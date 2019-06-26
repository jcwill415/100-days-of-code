# #100DaysOfCode Log - Round 1 - [Jenna Williams]

The log of my #100DaysOfCode challenge. Started on [June 16, Sunday, 2019].

## Log

### R1D1 6/16/19
Worked on CSS Basics @treehouse. Basic selectors, common values & units. https://teamtreehouse.com/ 4hrs prework @codelouisville.

### R1D2 6/17/19
AM tutorials #Python #AutomateTheBoringStuffWithPython. CSS text/box shadows & gradients @treehouse. 2hrs prework @codelouisville.

### R1D3 6/18/19
Completed @codelouisville pre-work: #HTML and #CSS. Reviewing a @treehouse #SQL course. Having so much fun! We use a relational database at work using SQL, and I'm excited to improve my #SQL skills and put them to good use. Plan to review some practice exercises in #HTML and #CSS before 6/26.

### R1D4 6/19/19
Still reviewing #SQL @treehouse! w3schools.com/sql/sql_select.asp

Write SELECT statement to query data from relational database
Select specific columns
Searching tables using 'WHERE'
Filter by comparing values

### R1D5 06/20/19
R1D5: Made progress in @treehouse #SQL course, reviewing relational operators. Having fun! Working on basics, then focus on writing better queries.

Also looking at @thew3cx courses on http://edx.org  #HTML5 & #JavaScript soon!

### R1D6 06/21/19
Modifying #SQL @treehouse, review & practice. Practice, practice, practice. 

5hrs to go in SQL Basics -- learning a lot everyday!

### R1D7 06/22/19
@treehouse + modifying data w/ #SQL. Updating Data in a Database badge.

### R1D8 06/23/19
R1D8: Reporting w/ #SQL @treehouse. Working on data handling - ordering, limiting, manipulating text, and aggregation.

SQL Basics Cheatsheet:
https://github.com/treehouse/cheatsheets/blob/master/sql_basics/cheatsheet.md

Reporting w/ SQL Cheatsheet: https://github.com/treehouse/cheatsheets/blob/master/reporting_with_sql/cheatsheet.md

Reporting w/ #SQL @treehouse part 2. Ordering Limiting. Paging Results.

### R1D9 06/24/19
+ Reporting w/ #SQL @treehouse; Functions/CONCAT. About an hr left on this module!

### R1D10 06/25/19
+ #SQL @treehouse - completed 1 hr during lunch!

-aggregate & numeric functions
-moving on to differences b/w databases...after work!

### R1D11 06/26/19
Formatting Dates For Reporting
The dates stored in a database often don't suit a human reader. 

Documentation Links for Formatting Dates

SQLite - https://www.sqlite.org/lang_datefunc.html
MS SQL - https://docs.microsoft.com/en-us/sql/t-sql/functions/date-and-time-data-types-and-functions-transact-sql?view=sql-server-2017#SetorGetSessionFormatFunctions
PostgreSQL - https://www.postgresql.org/docs/9.1/functions-datetime.html
MySQL - https://dev.mysql.com/doc/refman/5.5/en/date-and-time-functions.html
Oracle - https://docs.oracle.com/cd/B28359_01/server.111/b28286/sql_elements004.htm

Cheat Sheets

SQL Basics - https://github.com/treehouse/cheatsheets/blob/master/sql_basics/cheatsheet.md
Reporting with SQL - https://github.com/treehouse/cheatsheets/blob/master/reporting_with_sql/cheatsheet.md

-- DATE(<time string>, <modifiers>)

SELECT COUNT(*) FROM orders WHERE ordered_on
BETWEEN DATE("now", "-7 days") AND DATE("now", "-1 day");

SELECT COUNT(*) FROM orders WHERE ordered_on
BETWEEN DATE("now", "-7 days", "-7 days")
    AND DATE("now", "-1 day", "-7 days");

DATABASE SCHEMA

addresses	  20 Rows
id (PK)	    INTEGER
nickname	  TEXT
street	    TEXT
city	      TEXT
state	      TEXT
zip	        TEXT
country	    TEXT
user_id	    INTEGER

campaigns	9 Rows
id (PK)	    INTEGER
name	      TEXT
sales	      INTEGER

customers	10 Rows
id (PK)	    INTEGER
username	  TEXT
first_name	TEXT
last_name	  TEXT
password	  TEXT
email	      TEXT
phone	      TEXT

orders	294 Rows
id (PK)	    INTEGER
product_id	INTEGER
user_id	    INTEGER
address_id	INTEGER
ordered_on	DATE
status	    TEXT
cost	      DECIMAL(10,2)

products	29 Rows
id (PK)	    INTEGER
name	      TEXT
category	  TEXT
description	TEXT
price	      DECIMAL(10,2)
stock_count	INTEGER

id (PK)
INTEGER	nickname
TEXT	street 
TEXT	city 
TEXT	state 
TEXT	zip 
TEXT	country
TEXT	user_id
INTEGER

addresses

id      nickname  street                city            state             zip       country user_id
(PK)

INTEGER TEXT      TEXT                  TEXT            TEXT              TEXT      TEXT    INTEGER

1	      Home	    2532 2nd ST	          San Diego	      California	      90222	    USA	     1
2	      Work	    2213 5th PL	          Fresno	        CA	              90266	    USA	     1
3	      Home	    3521 24th AVE	        Fresno	        California	      90263	    USA	     2 
4	      Work	    3984 2nd AVE	        San Diego	      California	      90246	    USA	     2
5	      Home	    1271 13th ST	        Fresno	        CA	              90230	    USA	     5
6	      Work	    575 6th ST	          Sacramento	    CA	              90292	    USA	     5
7	      Home	    656 1st PL	          Sacramento	    CA	              90270	    USA	     10
8	      Work	    1190 1st ST	          Fresno	        CA	              90213	    USA	     10
9	      Home	    1405 6th ST	          Fresno	        CA	              90290	    USA	     11
10	    Work	    2493 4th ST	          Los Angeles	    CA	              90223	    USA	     11
11	    Home	    43 Barnetby Road	    Beverley        North Humberside	hu7 3yk	  UK	     12
12	    Work	    16 Chantlands Avenue	Hessle	        East Yorkshire	  hu1 2av	  UK	     12
13	    Home	    14 Richmond Avenue	  Hessle	        East Yorkshire	  HU1 9DS	  UK	     13
14	    Work	    73 Chantlands Avenue	Hessle	        East Yorkshire	  hu1 9wo	  UK	     13
15	    Home	    13 Barnetby Street	  Beverley	      East Yorkshire	  hu13 4lp	UK	     14
16	    Work	    37 Barnetby Avenue	  Beverley	      North Humberside	HU5 3BR	  UK	     14
17	    Home	    64 Barnetby Road	    Anlaby	        North Humberside	HU1 4EG	  UK	     20
18	    Work	    36 Barnetby Street	  Hessle	        East Yorkshire	  HU1 7HX	  UK	     20
19	    Home	    19 Chantlands Street	Anlaby	        North Humberside	HU18 1CR	UK	     21
20	    Work	    20 Chantlands Street	Beverley	      North Humberside	HU14 6FD	UK	     21

campaigns

id      name          sales
(PK)

INTEGER	TEXT          INTEGER
1	      e-mail	      780
2	      television	  8027
3	      banner ads	  8462
4	      google ads	  5017
5	d     irect mail	  3951
6	      blog	        4407
7	      social media  3574
8	      search	      621
9	      affiliate	    7199

customers

id      username        first_name  last_name   password    email phone            
(PK)

INTEGER	TEXT	          TEXT	      TEXT	      TEXT	      TEXT	TEXT

1	      lozzy	          Lauren	    Chalkley	  $2a$10$ym4rN7Q9bi1evayogNd1deS1KBPZ26qiVjMUjCa2o7JBtnHKImbjG	Lauren.Chalkley@example.com	(601)-555-8510
2	      sawmac	        Dave	    McFarland	    $2a$10$Uuc32WcXKiQ7XdqXbUoqweOIUQ.6wJuUH2stw1d.qOXvr9wmm2NPy	Dave.McFarland@example.com	(675)-555-4108
5	      pasanpr	        Pasan		                $2a$10$62UyMdce66RJiEeMjDFUB.y5wsKkh50RLaoI3YeUGW8HPVeE87g0K	pdawg@example.com	(898)-555-3719
10	    chalkers	      Andrew	  Chalkley	    $2a$10$sscRBI/UgjAGzsl5In/pgupzdfFUc2AiWTaQ5VAZl1FtefmDviBv6	Andrew@teamtreehouse.com	(798)-555-8112
11	    rocky	          Rachael	  Hinkley	      $2a$10$DwkYC.Vk.QsFHwCmcJ5N7u1ImdmDVzXOtcy5yK.kFqDOP6.Zruey2	Rachael.Hinkley@example.com	(645)-555-2397
12	    wig_lady	      Lola	    Love	        $2a$10$DOP8wdOdr/mkpdTokCNw5e0/MUGTyAZk0w5vTsnUbc9zNhoB152tq	Lola.Love@example.com	(582)-555-6954
13	    2spooky4me	    Nick	    Pettit	      $2a$10$OyntCZ148P2.0vWNskgNUOSorNZJOVo.8ZHq.a47lSH6qt6O0yTzK	Nick.Pettit@example.com	(784)-555-6107
14	    racing_car	    Cory	    Tepper	      $2a$10$7oZ/wvP1tygyzJIjSD37POgH5If.E/fL8VR9mZTXbhMllidP7pWpi	Cory.Tepper@example.com	(514)-555-7803
20	    beard_man	      Jim	      Hoskins	      $2a$10$ievDxprcJHq14.A5LedqTe4AT9rJrXujwyJJfSgfHZJgdIUF8r1Gm	Jim.Hoskins@example.com	(602)-555-4047
21	    poley_hands	    Michael		              $2a$10$bNetPI81FeQQlbrE.kgv0OUasKYHwNjtDYWclPsvWZC0WYYL3gVVG	michael.poley@example.com	(748)-555-9464

orders

id (PK)
INTEGER	product_id
INTEGER	user_id
INTEGER	address_id
INTEGER	ordered_on
DATE	status 
TEXT	cost 
DECIMAL(10,2)
1	14	1	2	2019-06-22	shipped	10.99
2	17	1	1	2019-06-25	shipped	8.99
3	21	1	2	2019-06-19	placed	6.99
4	13	1	1	2019-06-17	placed	15.99
5	21	1	1	2019-06-21	placed	11.99
6	4	1	2	2019-06-18	placed	11.99
7	26	1	2	2019-06-23	placed	17.99
8	3	1	2	2019-06-24	placed	12.99
9	2	1	2	2019-06-21	shipped	11.99
10	27	1	1	2019-06-23	shipped	14.99
11	12	1	1	2019-06-23	placed	14.99
12	9	1	1	2019-06-21	placed	172.99
13	10	1	2	2019-06-19	placed	8.99
14	10	1	2	2019-06-18	placed	15.99
15	28	1	2	2019-06-25	shipped	11.99
16	23	1	1	2019-06-19	placed	12.99
17	10	1	2	2019-06-16	shipped	8.99
18	1	1	1	2019-06-26	placed	10.99
19	12	1	2	2019-06-26	placed	16.99
20	29	1	1	2019-06-16	placed	13.99
21	2	1	1	2019-06-23	shipped	4.99
22	17	1	1	2019-06-23	shipped	14.99
23	14	1	2	2019-06-21	placed	5.99
24	26	1	1	2019-06-24	shipped	14.99
25	6	1	2	2019-06-24	shipped	10.99
26	17	1	1	2019-06-24	shipped	12.99
27	10	1	2	2019-06-16	shipped	13.99
28	13	1	2	2019-06-18	placed	11.99
29	1	1	1	2019-06-22	shipped	9.99
30	20	1	2	2019-06-19	placed	15.99
31	9	1	2	2019-06-23	placed	164.99
32	1	1	1	2019-06-25	placed	12.99
33	24	1	2	2019-06-20	placed	11.99
34	5	1	1	2019-06-24	shipped	3.99
35	13	1	2	2019-06-26	shipped	16.99
36	29	1	2	2019-06-23	placed	6.99
37	20	1	2	2019-06-18	placed	12.99
38	29	1	1	2019-06-26	placed	9.99
39	17	1	1	2019-06-21	placed	6.99
40	3	1	2	2019-06-22	placed	12.99
41	25	1	1	2019-06-18	shipped	8.99
42	15	1	1	2019-06-26	shipped	7.99
43	5	1	1	2019-06-19	placed	6.99
44	2	1	2	2019-06-22	placed	3.99
45	4	1	1	2019-06-22	shipped	10.99
46	3	1	2	2019-06-19	placed	7.99
47	2	1	1	2019-06-18	shipped	2.99
48	28	1	1	2019-06-19	shipped	10.99
49	26	1	1	2019-06-17	placed	14.99
50	26	1	2	2019-06-16	placed	17.99
51	5	2	3	2019-06-20	shipped	5.99
52	9	2	4	2019-06-26	placed	165.99
53	13	2	3	2019-06-19	shipped	9.99
54	13	2	4	2019-06-19	placed	14.99
55	26	2	3	2019-06-18	shipped	15.99
56	26	2	3	2019-06-26	placed	16.99
57	10	2	3	2019-06-24	placed	14.99
58	21	2	3	2019-06-16	placed	11.99
59	3	2	4	2019-06-22	shipped	7.99
60	27	2	4	2019-06-20	shipped	15.99
61	19	2	3	2019-06-24	placed	9.99
62	17	2	3	2019-06-17	shipped	15.99
63	3	2	4	2019-06-25	placed	3.99
64	4	2	3	2019-06-22	placed	3.99
65	24	2	4	2019-06-24	shipped	11.99
66	21	2	3	2019-06-24	placed	11.99
67	22	2	3	2019-06-22	shipped	14.99
68	15	2	3	2019-06-26	shipped	14.99
69	2	2	3	2019-06-26	placed	8.99
70	4	2	4	2019-06-18	shipped	10.99
71	3	2	4	2019-06-19	shipped	10.99
72	20	2	4	2019-06-17	placed	14.99
73	14	2	3	2019-06-21	placed	10.99
74	15	2	4	2019-06-16	placed	8.99
75	23	2	3	2019-06-21	shipped	16.99
76	6	2	3	2019-06-26	shipped	5.99
77	13	2	3	2019-06-24	shipped	14.99
78	10	2	4	2019-06-18	shipped	10.99
79	3	2	3	2019-06-17	shipped	11.99
80	27	2	4	2019-06-23	placed	11.99
81	26	2	4	2019-06-22	shipped	17.99
82	13	2	3	2019-06-22	shipped	16.99
83	13	2	4	2019-06-19	shipped	10.99
84	18	2	4	2019-06-22	placed	11.99
85	1	2	4	2019-06-16	shipped	4.99
86	5	2	4	2019-06-20	shipped	11.99
87	15	2	4	2019-06-24	placed	11.99
88	9	2	4	2019-06-21	placed	167.99
89	6	2	4	2019-06-16	shipped	2.99
90	2	2	4	2019-06-23	placed	10.99
91	3	5	5	2019-06-26	placed	9.99
92	16	5	6	2019-06-18	shipped	9.99
93	13	5	5	2019-06-21	placed	10.99
94	20	5	5	2019-06-21	shipped	15.99
95	22	5	5	2019-06-19	placed	14.99
96	7	5	5	2019-06-24	placed	295.99
97	26	5	6	2019-06-22	placed	15.99
98	7	5	5	2019-06-16	placed	295.99
99	3	5	6	2019-06-26	placed	9.99
100	2	5	5	2019-06-24	placed	10.99
101	10	5	5	2019-06-21	shipped	9.99
102	5	5	6	2019-06-21	placed	5.99
103	10	5	5	2019-06-16	placed	14.99
104	20	5	6	2019-06-22	shipped	8.99
105	25	5	5	2019-06-26	placed	11.99
106	7	5	5	2019-06-26	shipped	299.99
107	8	5	6	2019-06-24	shipped	343.99
108	1	5	6	2019-06-23	placed	9.99
109	22	5	5	2019-06-22	shipped	6.99
110	25	5	5	2019-06-25	shipped	10.99
111	1	5	6	2019-06-18	shipped	12.99
112	27	5	6	2019-06-18	shipped	13.99
113	16	5	5	2019-06-22	shipped	14.99
114	25	10	7	2019-06-24	placed	9.99
115	21	10	7	2019-06-21	shipped	3.99
116	9	10	7	2019-06-19	shipped	167.99
117	1	10	7	2019-06-22	placed	12.99
118	25	10	8	2019-06-23	placed	6.99
119	2	10	8	2019-06-22	placed	10.99
120	1	10	7	2019-06-16	placed	6.99
121	12	10	8	2019-06-24	shipped	15.99
122	5	10	7	2019-06-23	placed	6.99
123	25	10	7	2019-06-24	placed	4.99
124	24	10	8	2019-06-20	placed	10.99
125	7	10	8	2019-06-16	shipped	297.99
126	7	10	8	2019-06-18	placed	299.99
127	5	10	7	2019-06-25	placed	8.99
128	16	10	8	2019-06-17	placed	15.99
129	21	10	8	2019-06-21	shipped	3.99
130	25	10	8	2019-06-16	placed	11.99
131	6	10	7	2019-06-19	shipped	3.99
132	17	10	8	2019-06-26	placed	15.99
133	9	11	9	2019-06-21	shipped	171.99
134	19	11	9	2019-06-26	placed	11.99
135	6	11	9	2019-06-16	shipped	9.99
136	3	11	9	2019-06-25	placed	7.99
137	18	11	9	2019-06-26	placed	15.99
138	23	11	9	2019-06-24	placed	9.99
139	6	11	10	2019-06-25	placed	9.99
140	19	12	12	2019-06-20	shipped	2.99
141	28	12	12	2019-06-25	placed	11.99
142	16	12	12	2019-06-16	shipped	15.99
143	13	13	13	2019-06-25	placed	16.99
144	11	13	13	2019-06-24	shipped	12.99
145	21	13	13	2019-06-18	shipped	3.99
146	7	13	13	2019-06-17	placed	296.99
147	16	13	14	2019-06-20	placed	15.99
148	9	13	14	2019-06-19	placed	167.99
149	9	13	13	2019-06-17	shipped	164.99
150	29	13	13	2019-06-26	placed	14.99
151	19	13	14	2019-06-25	shipped	10.99
152	1	13	13	2019-06-17	shipped	11.99
153	17	13	14	2019-06-18	shipped	13.99
154	9	13	14	2019-06-26	shipped	169.99
155	21	13	14	2019-06-24	shipped	11.99
156	25	13	13	2019-06-18	placed	11.99
157	20	13	14	2019-06-19	shipped	7.99
158	14	13	14	2019-06-26	shipped	11.99
159	3	13	14	2019-06-26	placed	11.99
160	23	13	13	2019-06-22	placed	10.99
161	2	13	14	2019-06-16	shipped	8.99
162	15	13	14	2019-06-16	placed	5.99
163	12	13	13	2019-06-16	placed	10.99
164	25	13	14	2019-06-24	shipped	10.99
165	16	13	14	2019-06-22	shipped	14.99
166	3	13	13	2019-06-21	placed	12.99
167	4	13	13	2019-06-26	shipped	10.99
168	1	13	13	2019-06-16	placed	10.99
169	20	13	13	2019-06-23	shipped	12.99
170	12	13	14	2019-06-25	shipped	11.99
171	21	13	14	2019-06-22	shipped	6.99
172	16	13	13	2019-06-16	placed	8.99
173	14	13	13	2019-06-26	placed	10.99
174	17	13	13	2019-06-23	shipped	15.99
175	13	13	14	2019-06-22	placed	9.99
176	5	13	14	2019-06-18	placed	11.99
177	12	13	13	2019-06-17	shipped	11.99
178	3	13	13	2019-06-26	shipped	12.99
179	21	13	14	2019-06-26	placed	11.99
180	5	13	14	2019-06-19	shipped	4.99
181	15	13	14	2019-06-24	shipped	14.99
182	6	13	14	2019-06-23	placed	5.99
183	27	13	14	2019-06-23	shipped	10.99
184	14	13	13	2019-06-17	shipped	13.99
185	12	13	13	2019-06-18	shipped	10.99
186	15	14	15	2019-06-25	placed	14.99
187	12	14	16	2019-06-21	shipped	16.99
188	3	14	15	2019-06-26	placed	11.99
189	20	14	16	2019-06-20	shipped	12.99
190	11	14	15	2019-06-17	shipped	8.99
191	8	14	15	2019-06-17	shipped	345.99
192	5	14	16	2019-06-23	placed	4.99
193	15	14	15	2019-06-16	shipped	11.99
194	11	14	15	2019-06-17	placed	10.99
195	25	14	15	2019-06-25	shipped	9.99
196	4	14	15	2019-06-25	placed	12.99
197	25	14	16	2019-06-17	shipped	11.99
198	4	14	16	2019-06-16	placed	9.99
199	1	14	16	2019-06-24	placed	9.99
200	28	14	15	2019-06-22	placed	11.99
201	18	14	16	2019-06-16	placed	11.99
202	12	14	16	2019-06-21	shipped	17.99
203	16	14	16	2019-06-21	shipped	14.99
204	29	14	16	2019-06-16	shipped	15.99
205	11	14	15	2019-06-19	shipped	5.99
206	11	14	15	2019-06-25	shipped	10.99
207	26	14	16	2019-06-26	placed	12.99
208	24	14	15	2019-06-20	shipped	12.99
209	8	14	15	2019-06-24	shipped	352.99
210	3	14	16	2019-06-24	shipped	6.99
211	4	14	16	2019-06-17	shipped	11.99
212	26	14	16	2019-06-20	placed	14.99
213	27	14	16	2019-06-23	shipped	16.99
214	4	14	15	2019-06-21	placed	12.99
215	3	20	17	2019-06-23	shipped	11.99
216	6	20	17	2019-06-22	shipped	9.99
217	27	20	17	2019-06-25	shipped	15.99
218	14	20	17	2019-06-23	placed	11.99
219	11	20	17	2019-06-21	placed	4.99
220	23	20	17	2019-06-21	placed	9.99
221	3	20	18	2019-06-26	shipped	11.99
222	9	20	17	2019-06-23	shipped	171.99
223	19	20	18	2019-06-24	shipped	3.99
224	2	20	18	2019-06-25	shipped	9.99
225	3	20	17	2019-06-24	shipped	11.99
226	4	20	17	2019-06-26	shipped	10.99
227	9	20	17	2019-06-19	shipped	169.99
228	7	20	18	2019-06-22	placed	301.99
229	16	20	17	2019-06-23	shipped	12.99
230	2	20	18	2019-06-26	shipped	9.99
231	10	20	18	2019-06-24	shipped	14.99
232	29	20	17	2019-06-23	shipped	13.99
233	3	20	17	2019-06-24	shipped	12.99
234	8	20	18	2019-06-24	shipped	350.99
235	10	20	18	2019-06-18	shipped	13.99
236	14	20	17	2019-06-21	placed	11.99
237	28	20	17	2019-06-19	placed	13.99
238	14	20	17	2019-06-25	placed	4.99
239	8	20	18	2019-06-25	shipped	347.99
240	11	20	18	2019-06-19	placed	4.99
241	3	20	18	2019-06-25	placed	5.99
242	19	20	18	2019-06-25	shipped	9.99
243	25	20	17	2019-06-16	shipped	9.99
244	7	20	17	2019-06-20	placed	300.99
245	29	20	18	2019-06-25	shipped	12.99
246	16	20	17	2019-06-22	placed	9.99
247	4	20	17	2019-06-25	shipped	6.99
248	2	21	20	2019-06-18	shipped	11.99
249	18	21	20	2019-06-18	placed	8.99
250	5	21	20	2019-06-18	shipped	11.99
251	12	21	19	2019-06-23	placed	14.99
252	6	21	19	2019-06-23	placed	2.99
253	18	21	19	2019-06-17	placed	15.99
254	13	21	19	2019-06-23	placed	11.99
255	17	21	19	2019-06-22	shipped	13.99
256	4	21	19	2019-06-19	shipped	3.99
257	12	21	20	2019-06-16	shipped	16.99
258	8	21	19	2019-06-26	shipped	346.99
259	1	21	20	2019-06-19	placed	10.99
260	18	21	19	2019-06-16	shipped	14.99
261	24	21	19	2019-06-16	placed	13.99
262	29	21	19	2019-06-17	placed	6.99
263	26	21	20	2019-06-18	shipped	14.99
264	5	21	20	2019-06-24	shipped	9.99
265	29	21	19	2019-06-19	shipped	15.99
266	15	21	19	2019-06-23	placed	11.99
267	3	21	20	2019-06-17	shipped	9.99
268	19	21	20	2019-06-20	shipped	8.99
269	28	21	19	2019-06-19	shipped	11.99
270	20	21	19	2019-06-21	shipped	12.99
271	13	21	20	2019-06-17	placed	11.99
272	27	21	20	2019-06-25	placed	11.99
273	4	21	20	2019-06-21	shipped	9.99
274	3	21	20	2019-06-19	shipped	12.99
275	6	21	20	2019-06-22	placed	10.99
276	13	21	19	2019-06-24	placed	17.99
277	16	21	20	2019-06-18	placed	10.99
278	27	21	20	2019-06-25	shipped	15.99
279	25	21	19	2019-06-26	placed	4.99
280	22	21	19	2019-06-20	placed	11.99
281	1	21	19	2019-06-23	placed	12.99
282	17	21	19	2019-06-23	placed	7.99
283	28	21	20	2019-06-19	shipped	5.99
284	18	21	20	2019-06-19	shipped	10.99
285	29	21	20	2019-06-20	placed	14.99
286	4	21	19	2019-06-17	shipped	10.99
287	6	21	20	2019-06-19	placed	10.99
288	9	21	19	2019-06-22	shipped	169.99
289	10	21	19	2019-06-21	placed	7.99
290	20	21	20	2019-06-24	placed	14.99
291	2	21	20	2019-06-22	shipped	9.99
292	3	21	20	2019-06-18	placed	10.99
293	7	21	19	2019-06-18	placed	301.99
294	28	21	19	2019-06-25	placed	8.99

products

id (PK)
INTEGER	name 
TEXT	category 
TEXT	description 
TEXT	price 
DECIMAL(10,2)	stock_count
INTEGER
1	Small Retro T-Shirt	Clothing	Retro T-Shirt is made from 100% cotton. It's available in the following sizes: Small, Medium, Large	10.99	613
2	Medium Retro T-Shirt	Clothing	Retro T-Shirt is made from 100% cotton. It's available in the following sizes: Small, Medium, Large	8.99	419
3	Large Retro T-Shirt	Clothing	Retro T-Shirt is made from 100% cotton. It's available in the following sizes: Small, Medium, Large	8.99	97
4	Small Skinny Jeans	Clothing	Skinny Jeans is made from durable denim. It's available in the following sizes: Small, Large, Extra Large	9.99	530
5	Large Skinny Jeans	Clothing	Skinny Jeans is made from durable denim. It's available in the following sizes: Small, Large, Extra Large	8.99	25
6	Extra Large Skinny Jeans	Clothing	Skinny Jeans is made from durable denim. It's available in the following sizes: Small, Large, Extra Large	8.99	59
7	Xbox One	Electronics	Xbox One is a games console manufactured by Microsoft. It has 500GB of storage.	299.99	45
8	Playstation 4	Electronics	Playstation 4 is a games console manufactured by Sony. It has 500GB of storage.	349.99	657
9	Apple TV 32GB	Electronics	Apple TV 32GB is a streaming device manufactured by Apple. It has 32GB of storage.	169.99	52
10	Harry Potter and the Philosopher's Stone	Books	'Harry Potter and the Philosopher's Stone' was authored by J.K. Rowling. It was first published in 1997. It's one of the best fantasy books of all time.	13.99	872
11	Harry Potter and the Chamber of Secrets	Books	'Harry Potter and the Chamber of Secrets' was authored by J.K. Rowling. It was first published in 1998. It's one of the best fantasy books of all time.	12.99	779
12	Harry Potter and the Prisoner of Azkaban	Books	'Harry Potter and the Prisoner of Azkaban' was authored by J.K. Rowling. It was first published in 1999. It's one of the best fantasy books of all time.	10.99	314
13	Harry Potter and the Goblet of Fire	Books	'Harry Potter and the Goblet of Fire' was authored by J.K. Rowling. It was first published in 2000. It's one of the best fantasy books of all time.	13.99	770
14	Harry Potter and the Order of the Phoenix	Books	'Harry Potter and the Order of the Phoenix' was authored by J.K. Rowling. It was first published in 2003. It's one of the best fantasy books of all time.	6.99	508
15	Harry Potter and the Half-Blood Prince	Books	'Harry Potter and the Half-Blood Prince' was authored by J.K. Rowling. It was first published in 2005. It's one of the best fantasy books of all time.	6.99	796
16	Harry Potter and the Deathly Hallows	Books	'Harry Potter and the Deathly Hallows' was authored by J.K. Rowling. It was first published in 2007. It's one of the best fantasy books of all time.	6.99	389
17	A Brief History of Time	Books	'A Brief History of Time' was authored by Stephen Hawking. It was first published in 1988. It's one of the best non fiction books of all time.	7.99	738
18	The Universe in a Nutshell	Books	'The Universe in a Nutshell' was authored by Stephen Hawking. It was first published in 2001. It's one of the best non fiction books of all time.	11.99	790
19	Frankenstein	Books	'Frankenstein' was authored by Mary Shelley. It was first published in 1818. It's one of the best horror books of all time.	11.99	720
20	The Martian	Books	'The Martian' was authored by Andy Weir. It was first published in 2014. It's one of the best science fiction books of all time.	14.99	831
21	Ready Player One	Books	'Ready Player One' was authored by Ernest Cline. It was first published in 2014. It's one of the best science fiction books of all time.	12.99	793
22	Armada	Books	'Armada' was authored by Ernest Cline. It was first published in 2015. It's one of the best science fiction books of all time.	13.99	563
23	Pride and Prejudice	Books	'Pride and Prejudice' was authored by Jane Austen. It was first published in 1813. It's one of the best classic books of all time.	10.99	221
24	Emma	Books	'Emma' was authored by Jane Austen. It was first published in 1815. It's one of the best classic books of all time.	12.99	653
25	1984	Books	'1984' was authored by George Orwell. It was first published in 1949. It's one of the best fiction books of all time.	10.99	502
26	Dune	Books	'Dune' was authored by Frank Herbert. It was first published in 1965. It's one of the best science fiction books of all time.	14.99	551
27	The Circle	Books	'The Circle' was authored by Dave Eggers. It was first published in 2013. It's one of the best science fiction books of all time.	12.99	547
28	Contact	Books	'Contact' was authored by Carl Sagan. It was first published in 1985. It's one of the best science fiction books of all time.	7.99	394
29	Animal Farm	Books	'Animal Farm' was authored by George Orwell. It was first published in 1945. It's one of the best fiction books of all time.	15.99	644
### R1D12
### R1D13
### R1D14
### R1D15
### R1D16
### R1D17
### R1D18
### R1D19
### R1D20
### R1D21
### R1D22
### R1D23
### R1D24
### R1D25
### R1D26
### R1D27
### R1D28
### R1D29
### R1D30
### R1D31
### R1D32
### R1D33
### R1D34
### R1D35
### R1D36
### R1D37
### R1D38
### R1D39
### R1D40
### R1D41
### R1D42
### R1D43
### R1D44
### R1D45
### R1D46
### R1D47
### R1D48
### R1D49
### R1D50
### R1D51
### R1D52
### R1D53
### R1D54
### R1D55
### R1D56
### R1D57
### R1D58
### R1D59
### R1D60
### R1D61
### R1D62
### R1D63
### R1D64
### R1D65
### R1D66
### R1D67
### R1D68
### R1D69
### R1D70
### R1D71
### R1D72
### R1D73
### R1D74
### R1D75
### R1D76
### R1D77
### R1D78
### R1D79
### R1D80
### R1D81
### R1D82
### R1D83
### R1D84
### R1D85
### R1D86
### R1D87
### R1D88
### R1D89
### R1D90
### R1D91
### R1D92
### R1D93
### R1D94
### R1D95
### R1D86
### R1D97
### R1D98
### R1D99
### R1D100
