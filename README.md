Prompt: As part of the company's efforts to improve employee retention, develop a SQL query that provides an in-depth analysis of employee engagement and satisfaction. The query should offer the following insights:

1. Engagement and Satisfaction Trends: Calculate the average engagement and satisfaction scores for employees grouped by department.
2. High Performers: Identify employees with an engagement score above 90 and a satisfaction score above 85. Provide their names, job titles, and departments.
3. Gender Representation: Determine the proportion of male, female, and non-binary employees in each department. Include department name, gender, and percentages.
Result:
         department_type  avg_engagement  avg_satisfaction first_name  \
0          Admin Offices        2.925000          2.512500       None   
1       Executive Office        3.375000          3.083333       None   
2                  IT/IS        3.025581          3.009302       None   
3      Production               2.906436          3.020792       None   
4                  Sales        2.990937          3.132931       None   
5   Software Engineering        2.973913          3.113043       None   
6          Admin Offices             NaN               NaN       None   
7          Admin Offices             NaN               NaN       None   
8       Executive Office             NaN               NaN       None   
9       Executive Office             NaN               NaN       None   
10                 IT/IS             NaN               NaN       None   
11                 IT/IS             NaN               NaN       None   
12     Production                    NaN               NaN       None   
13     Production                    NaN               NaN       None   
14                 Sales             NaN               NaN       None   
15                 Sales             NaN               NaN       None   
16  Software Engineering             NaN               NaN       None   
17  Software Engineering             NaN               NaN       None   

   last_name title  gender  percentage  
0       None  None    None         NaN  
1       None  None    None         NaN  
2       None  None    None         NaN  
3       None  None    None         NaN  
4       None  None    None         NaN  
5       None  None    None         NaN  
6       None  None  Female   55.000000  
7       None  None    Male   45.000000  
8       None  None  Female    4.166667  
9       None  None    Male   95.833333  
10      None  None  Female   49.069767  
11      None  None    Male   50.930233  
12      None  None  Female   62.475248  
13      None  None    Male   37.524752  
14      None  None  Female   34.743202  
15      None  None    Male   65.256798  
16      None  None  Female   42.608696  
17      None  None    Male   57.391304  

Prompt: To optimize the company's training programs, create a SQL query that identifies key patterns in training data. The query should provide the following insights:

1. Training Completion Rates: Calculate the percentage of employees who have completed their training programs in each business unit.
2. High-Cost Training: Identify training programs that cost more than $5000. Provide their names, duration, and associated trainer.
3. Correlation with Performance: Find employees who completed training in 'Leadership' and have a performance score of 'Excellent'. Provide their names, job titles, and business units.
Result:
  business_unit  completion_rate training_program_name training_duration_days  \
0           BPC        21.452145                  None                   None   
1          CCDR        22.666667                  None                   None   
2            EW        25.827815                  None                   None   
3           MSC        26.351351                  None                   None   
4           NEL        23.026316                  None                   None   
5            PL        24.916944                  None                   None   
6           PYZ        24.080268                  None                   None   
7           SVG        32.236842                  None                   None   
8           TNS        30.639731                  None                   None   
9           WBL        25.510204                  None                   None   

  trainer first_name last_name title  
0    None       None      None  None  
1    None       None      None  None  
2    None       None      None  None  
3    None       None      None  None  
4    None       None      None  None  
5    None       None      None  None  
6    None       None      None  None  
7    None       None      None  None  
8    None       None      None  None  
9    None       None      None  None  

Prompt: To support recruitment strategy improvements, create a SQL query that provides insights into applicant data. The query should include the following:

1. Education Distribution: Group applicants by their highest education level and count the number in each group.
2. Experience Analysis: Calculate the average years of experience for applicants grouped by job title.
3. Geographic Distribution: Count the number of applicants from each state.
Result:
        education_level       count
0     Bachelor's Degree  785.000000
1           High School  738.000000
2       Master's Degree  736.000000
3                   PhD  741.000000
4    Academic librarian   16.166667
..                  ...         ...
694                  VT   36.000000
695                  WA   58.000000
696                  WI   53.000000
697                  WV   54.000000
698                  WY   60.000000

[699 rows x 2 columns]

Prompt: As part of the company's workforce analysis, create a SQL query to explore the distribution and performance of employees. The query should include the following insights:
                    1. Performance Distribution: Calculate the average performance score for each employee type (Full-time, Part-time, Contract).
                    2. Termination Analysis: Identify the number of employees terminated by each termination type.
                    3. Regional Performance: Determine the average performance score of employees grouped by state.
Result:
   employee_type  avg_performance
0       Contract              0.0
1      Full-Time              0.0
2      Part-Time              0.0
3    Involuntary            388.0
4    Resignation            380.0
5     Retirement            377.0
6            Unk           1467.0
7      Voluntary            388.0
8             AL              0.0
9             AZ              0.0
10            CA              0.0
11            CO              0.0
12            CT              0.0
13            FL              0.0
14            GA              0.0
15            ID              0.0
16            IN              0.0
17            KY              0.0
18            MA              0.0
19            ME              0.0
20            MT              0.0
21            NC              0.0
22            ND              0.0
23            NH              0.0
24            NV              0.0
25            NY              0.0
26            OH              0.0
27            OR              0.0
28            PA              0.0
29            RI              0.0
30            TN              0.0
31            TX              0.0
32            UT              0.0
33            VA              0.0
34            VT              0.0
35            WA              0.0

Prompt: To assist in evaluating training investments, generate a SQL query that examines the effectiveness and cost distribution of training programs. Include the following:
                1. Training Effectiveness: Calculate the percentage of employees who completed their training programs by training type.
                2. Costly Programs: Identify training programs that exceeded a cost threshold of $7000. Include program name, cost, and trainer.
                3. Departmental Training: Determine the total training cost for each department.
Result:
  training_type  completion_rate training_program_name training_cost trainer  \
0      External        24.077800                  None          None    None   
1      Internal        27.236581                  None          None    None   
2          None              NaN                  None          None    None   
3          None              NaN                  None          None    None   
4          None              NaN                  None          None    None   
5          None              NaN                  None          None    None   
6          None              NaN                  None          None    None   
7          None              NaN                  None          None    None   

        department_type  total_cost  
0                  None         NaN  
1                  None         NaN  
2         Admin Offices    43004.40  
3      Executive Office    14051.27  
4                 IT/IS   242359.86  
5     Production         1130181.05  
6                 Sales   177667.88  
7  Software Engineering    68621.63  

Prompt: To improve work-life balance strategies, generate a SQL query that analyzes survey data. Include the following:
                1. Work-Life Balance Trends: Calculate the average work-life balance score for employees in each business unit.
                2. High Satisfaction Employees: Identify employees with a satisfaction score above 90. Provide their names, job titles, and business units.
                3. Correlation Analysis: Compare the average engagement score of employees with a work-life balance score below 50 versus those above 80.
Result:
   business_unit  avg_balance first_name last_name title balance_group  \
0            BPC     2.854785       None      None  None          None   
1           CCDR     2.896667       None      None  None          None   
2             EW     3.155629       None      None  None          None   
3            MSC     3.033784       None      None  None          None   
4            NEL     2.934211       None      None  None          None   
5             PL     3.023256       None      None  None          None   
6            PYZ     3.006689       None      None  None          None   
7            SVG     3.085526       None      None  None          None   
8            TNS     2.895623       None      None  None          None   
9            WBL     3.003401       None      None  None          None   
10          None          NaN       None      None  None           Low   

    avg_engagement  
0              NaN  
1              NaN  
2              NaN  
3              NaN  
4              NaN  
5              NaN  
6              NaN  
7              NaN  
8              NaN  
9              NaN  
10        2.939667  

Prompt: To streamline recruitment efforts, create a SQL query that evaluates applicant trends and preferences. Include the following:
                1. Application Trends: Count the number of applications received each month in the last year.
                2. Preferred Roles: Identify the top 5 job titles with the highest number of applicants. Include the count of applicants for each.
                3. Education Insights: Calculate the average years of experience for applicants grouped by their highest education level.
Result:
                           application_month        count
0                                       None  1047.000000
1                                   Best boy    13.000000
2                                 Translator    12.000000
3                     Race relations officer    12.000000
4                   Therapeutic radiographer    11.000000
5  Sound technician, broadcasting/film/video    11.000000
6                          Bachelor's Degree     9.908280
7                                High School    10.021680
8                            Master's Degree    10.020380
9                                        PhD     9.912281

Prompt: To evaluate employee engagement in different business units, create a SQL query that provides the following insights:
            1. Engagement by Unit: Calculate the average engagement score for each business unit.
            2. Top Performers: Identify employees with engagement scores in the top 10% across all business units. Include their names and job titles.
            3. Unit Satisfaction: Determine the average satisfaction score for employees in each business unit.
Error: Execution failed on sql 'WITH EngagementByUnit AS (
    SELECT business_unit, AVG(engagement_score) AS avg_engagement
    FROM employee_engagement_survey_data e
    JOIN employee_data d ON e.employee_id = d.employee_id
    GROUP BY business_unit
    ),
    TopPerformers AS (
        SELECT d.first_name, d.last_name, d.title
        FROM employee_engagement_survey_data e
        JOIN employee_data d ON e.employee_id = d.employee_id
        WHERE e.engagement_score > (SELECT PERCENTILE_CONT(0.9) WITHIN GROUP (ORDER BY engagement_score) FROM employee_engagement_survey_data)
    ),
    UnitSatisfaction AS (
        SELECT business_unit, AVG(satisfaction_score) AS avg_satisfaction
        FROM employee_engagement_survey_data e
        JOIN employee_data d ON e.employee_id = d.employee_id
        GROUP BY business_unit
    )
    SELECT * FROM EngagementByUnit
    UNION ALL
    SELECT * FROM TopPerformers
    UNION ALL
    SELECT * FROM UnitSatisfaction;': near "(": syntax error

Prompt: To enhance training program evaluation, create a SQL query that provides insights into training outcomes. Include the following:
            1. Completion Rates by Program: Calculate the completion rate for each training program.
            2. High-Cost Trainings: Identify training programs that exceed $10,000 in total cost. Include their names and the number of attendees.
            3. Impactful Trainings: Find employees who completed the 'Advanced Technical Skills' training and achieved an engagement score above 85. Include their names and job titles.
Error: Execution failed on sql 'WITH CompletionRatesByProgram AS (
            SELECT training_program_name, COUNT(CASE WHEN training_outcome = 'Completed' THEN 1 END) * 100.0 / COUNT(*) AS completion_rate
            FROM training_and_development_data
            GROUP BY training_program_name
            ),
            HighCostTrainings AS (
                SELECT training_program_name, SUM(training_cost) AS total_cost, COUNT(employee_id) AS attendees
                FROM training_and_development_data
                WHERE training_cost > 10000
                GROUP BY training_program_name
            ),
            ImpactfulTrainings AS (
                SELECT d.first_name, d.last_name, d.title
                FROM training_and_development_data t
                JOIN employee_data d ON t.employee_id = d.employee_id
                JOIN employee_engagement_survey_data e ON d.employee_id = e.employee_id
                WHERE t.training_program_name = 'Advanced Technical Skills' AND e.engagement_score > 85
            )
            SELECT * FROM CompletionRatesByProgram
            UNION ALL
            SELECT * FROM HighCostTrainings
            UNION ALL
            SELECT * FROM ImpactfulTrainings;': SELECTs to the left and right of UNION ALL do not have the same number of result columns

Prompt: To analyze employee performance and retention, create a SQL query to identify key patterns. Include the following insights:
            1. Retention Rates: Calculate the percentage of employees retained over the last three years.
            2. Top Performers by Department: Identify the top 3 employees with the highest performance scores in each department. Include their names and scores.
            3. Exit Trends: Count the number of employees who exited the company each year.
Error: Execution failed on sql 'WITH RetentionRates AS (
            SELECT strftime('%Y', start_date) AS start_year,
                   COUNT(CASE WHEN exit_date IS NULL THEN 1 END) * 100.0 / COUNT(*) AS retention_rate
            FROM employee_data
            WHERE strftime('%Y', start_date) >= strftime('%Y', 'now', '-3 years')
            GROUP BY start_year
            ),
            TopPerformers AS (
                SELECT department_type, first_name, last_name, performance_score
                FROM (
                    SELECT d.department_type, d.first_name, d.last_name, d.performance_score,
                           RANK() OVER (PARTITION BY d.department_type ORDER BY d.performance_score DESC) AS rank
                    FROM employee_data d
                )
                WHERE rank <= 3
            ),
            ExitTrends AS (
                SELECT strftime('%Y', exit_date) AS exit_year, COUNT(*) AS exit_count
                FROM employee_data
                WHERE exit_date IS NOT NULL
                GROUP BY exit_year
            )
            SELECT * FROM RetentionRates
            UNION ALL
            SELECT * FROM TopPerformers
            UNION ALL
            SELECT * FROM ExitTrends;': SELECTs to the left and right of UNION ALL do not have the same number of result columns

Prompt: To evaluate diversity initiatives, create a SQL query that analyzes employee demographics. Include the following:
        1. Gender Distribution: Calculate the percentage of employees by gender in each department.
        2. Ethnicity Representation: Count the number of employees from each ethnicity in each business unit.
        3. Salary Averages: Determine the average pay zone for employees grouped by gender and ethnicity.
Result:
     department_type    gender  percentage
0      Admin Offices    Female   55.000000
1      Admin Offices      Male   45.000000
2   Executive Office    Female    4.166667
3   Executive Office      Male   95.833333
4              IT/IS    Female   49.069767
..               ...       ...         ...
67              Male     Asian    0.000000
68              Male     Black    0.000000
69              Male  Hispanic    0.000000
70              Male     Other    0.000000
71              Male     White    0.000000

[72 rows x 3 columns]

Prompt: To monitor employee growth, create a SQL query that tracks changes in performance scores over time. Include the following:
            1. Yearly Performance Growth: Calculate the average performance score for each year across all employees.
            2. Top 5 Improving Employees: Identify the top 5 employees with the largest improvement in performance score from the previous year. Include their names and scores.
            3. Department Growth Trends: Determine the yearly average performance score for each department.
Error: Execution failed on sql 'WITH YearlyPerformanceGrowth AS (
            SELECT strftime('%Y', start_date) AS year, AVG(performance_score) AS avg_performance
            FROM employee_data
            GROUP BY year
            ),
            TopImprovingEmployees AS (
                SELECT d.first_name, d.last_name,
                       (e.performance_score - LAG(e.performance_score) OVER (PARTITION BY e.employee_id ORDER BY e.survey_date)) AS improvement
                FROM employee_engagement_survey_data e
                JOIN employee_data d ON e.employee_id = d.employee_id
                ORDER BY improvement DESC
                LIMIT 5
            ),
            DepartmentGrowthTrends AS (
                SELECT d.department_type, strftime('%Y', start_date) AS year, AVG(e.performance_score) AS avg_score
                FROM employee_engagement_survey_data e
                JOIN employee_data d ON e.employee_id = d.employee_id
                GROUP BY d.department_type, year
            )
            SELECT * FROM YearlyPerformanceGrowth
            UNION ALL
            SELECT * FROM TopImprovingEmployees
            UNION ALL
            SELECT * FROM DepartmentGrowthTrends;': no such column: e.performance_score

Prompt: To evaluate employee attendance in training programs, create a SQL query that provides insights into training participation. Include the following:
            1. Training Attendance: Count the number of employees who attended each training program.
            2. Department Participation: Calculate the percentage of employees in each department who have attended at least one training program.
            3. High Attendance Programs: Identify training programs with more than 50 attendees. Include the program name and number of attendees.
Result:
     training_program_name  attendee_count
0     Communication Skills           673.0
1         Customer Service           565.0
2   Leadership Development           574.0
3       Project Management           609.0
4         Technical Skills           579.0
5            Admin Offices           100.0
6         Executive Office           100.0
7                    IT/IS           100.0
8        Production                  100.0
9                    Sales           100.0
10    Software Engineering           100.0
11    Communication Skills           673.0
12        Customer Service           565.0
13  Leadership Development           574.0
14      Project Management           609.0
15        Technical Skills           579.0

Prompt: To identify active employees, write a SQL query that lists all employees currently employed. Include their names and job titles.
Result:
     first_name   last_name                    title
0         Uriah     Bridges  Production Technician I
1         Paula       Small  Production Technician I
2        Edward        Buck       Area Sales Manager
3       Michael     Riordan       Area Sales Manager
4       Jasmine       Onque       Area Sales Manager
...         ...         ...                      ...
2453    Stanley       Reyes  Production Technician I
2454       Levi      Hayden  Production Technician I
2455    Brenden       Leach  Production Technician I
2456     Adyson  Strickland  Production Technician I
2457      Chace        Kerr  Production Technician I

[2458 rows x 3 columns]

Prompt: To evaluate training participation, write a SQL query that counts the number of employees who completed training programs.
Result:
   completed_trainings
0                  770

Prompt: To understand recruitment trends, write a SQL query that calculates the number of applications received for each job title.
Result:
                            job_title  application_count
0                  Academic librarian                  6
1               Accommodation manager                  6
2               Accountant, chartered                  3
3     Accountant, chartered certified                  5
4    Accountant, chartered management                  3
..                                ...                ...
631           Water quality scientist                  4
632                      Web designer                  8
633                Wellsite geologist                  4
634                            Writer                  4
635                      Youth worker                  3

[636 rows x 2 columns]

Prompt: To analyze diversity, write a SQL query that calculates the percentage of employees by gender.
Result:
   gender  percentage
0  Female   56.066667
1    Male   43.933333

Prompt: To evaluate engagement scores, write a SQL query that finds the average engagement score for each department.
Result:
        department_type  avg_engagement
0         Admin Offices        2.925000
1      Executive Office        3.375000
2                 IT/IS        3.025581
3     Production               2.906436
4                 Sales        2.990937
5  Software Engineering        2.973913

Prompt: To track employee growth, write a SQL query that lists employees who have been with the company for over 5 years. Include their names and start dates.
Result:
Empty DataFrame
Columns: [first_name, last_name, start_date]
Index: []

Prompt: To improve satisfaction strategies, write a SQL query that lists employees with a satisfaction score above 80. Include their names and departments.
Result:
Empty DataFrame
Columns: [first_name, last_name, department_type]
Index: []

Prompt: To evaluate training costs, write a SQL query that calculates the total cost of training programs for each department.
Result:
        department_type  total_training_cost
0         Admin Offices             43004.40
1      Executive Office             14051.27
2                 IT/IS            242359.86
3     Production                  1130181.05
4                 Sales            177667.88
5  Software Engineering             68621.63

Prompt: To analyze recruitment success, write a SQL query that counts the number of applicants selected for each job title.
Result:
Empty DataFrame
Columns: [job_title, selected_count]
Index: []

Prompt: To track work-life balance, write a SQL query that finds the average work-life balance score for employees in each business unit.
Result:
  business_unit  avg_balance
0           BPC     2.854785
1          CCDR     2.896667
2            EW     3.155629
3           MSC     3.033784
4           NEL     2.934211
5            PL     3.023256
6           PYZ     3.006689
7           SVG     3.085526
8           TNS     2.895623
9           WBL     3.003401

Prompt: To monitor exit trends, write a SQL query that counts the number of employees who exited the company each year.
Result:
  exit_year  exit_count
0      None        1533

Prompt: To analyze performance, write a SQL query that identifies the top 3 employees with the highest performance scores in each department.
Result:
          department_type first_name last_name performance_score
0           Admin Offices     Hadley   Barrett               PIP
1           Admin Offices     Konnor     Rivas               PIP
2           Admin Offices      Karla   Farrell               PIP
3           Admin Offices   Anderson   Meadows               PIP
4           Admin Offices     Nathan     Kline               PIP
..                    ...        ...       ...               ...
217  Software Engineering       Coby     Giles       Fully Meets
218  Software Engineering      Jalen  Jennings       Fully Meets
219  Software Engineering      Maeve    Gordon       Fully Meets
220  Software Engineering  Monserrat  Ferguson       Fully Meets
221  Software Engineering  Elisabeth   Bradley       Fully Meets

[222 rows x 4 columns]

Prompt: To analyze department retention, write a SQL query that calculates the retention rate for each department.
Result:
        department_type  retention_rate
0         Admin Offices       97.500000
1      Executive Office      100.000000
2                 IT/IS       87.209302
3     Production              78.613861
4                 Sales       90.936556
5  Software Engineering       80.000000

Prompt: To understand salary distribution, write a SQL query that calculates the average pay zone for each job title.
Result:
                           title  avg_pay_zone
0                   Accountant I           0.0
1       Administrative Assistant           0.0
2             Area Sales Manager           0.0
3                   BI Developer           0.0
4                    BI Director           0.0
5                            CIO           0.0
6                   Data Analyst           0.0
7                  Data Analyst            0.0
8                 Data Architect           0.0
9         Database Administrator           0.0
10        Director of Operations           0.0
11             Director of Sales           0.0
12          Enterprise Architect           0.0
13                   IT Director           0.0
14               IT Manager - DB           0.0
15            IT Manager - Infra           0.0
16          IT Manager - Support           0.0
17                    IT Support           0.0
18              Network Engineer           0.0
19               President & CEO           0.0
20      Principal Data Architect           0.0
21            Production Manager           0.0
22       Production Technician I           0.0
23      Production Technician II           0.0
24                 Sales Manager           0.0
25           Senior BI Developer           0.0
26       Shared Services Manager           0.0
27             Software Engineer           0.0
28  Software Engineering Manager           0.0
29                Sr. Accountant           0.0
30                       Sr. DBA           0.0
31          Sr. Network Engineer           0.0

Prompt: To find inactive employees, write a SQL query that lists employees who are no longer employed. Include their names and termination types.
Result:
Empty DataFrame
Columns: [first_name, last_name, termination_type]
Index: []

Prompt: To assess training impact, write a SQL query that lists employees who completed 'Leadership' training and their current performance scores.
Result:
Empty DataFrame
Columns: [first_name, last_name, performance_score]
Index: []

Prompt: To analyze job function diversity, write a SQL query that counts the number of employees in each job function.
Result:
            job_function  employee_count
0             Accountant               2
1             Accounting               9
2         Administration              23
3         Administrative              56
4          Administrator              50
..                   ...             ...
78                    Vp              37
79             Warehouse               2
80     Warehouse Manager               1
81  Warehouse Technician               3
82                Welder               5

[83 rows x 2 columns]

Prompt: To evaluate applicant experience, write a SQL query that calculates the average years of experience for applicants grouped by state.
Result:
   state  avg_experience
0     AK        9.131148
1     AL        8.959184
2     AR       11.638889
3     AS       10.795455
4     AZ       10.061224
5     CA        8.869565
6     CO       10.545455
7     CT       10.448980
8     DC       11.200000
9     DE        8.686275
10    FL        9.982456
11    FM        9.465517
12    GA       10.411765
13    GU        9.943396
14    HI        9.178571
15    IA        9.796296
16    ID       10.000000
17    IL       11.145455
18    IN        9.338710
19    KS       10.760870
20    KY       11.765957
21    LA        8.866667
22    MA       10.042553
23    MD       10.040816
24    ME       10.807692
25    MH        8.365854
26    MI       10.333333
27    MN        9.139535
28    MO       10.157895
29    MP       10.600000
30    MS       10.360000
31    MT       12.155556
32    NC        9.437500
33    ND        9.347826
34    NE        9.019231
35    NH       11.049180
36    NJ       10.130435
37    NM       10.346939
38    NV        8.725490
39    NY        9.220339
40    OH       10.803922
41    OK       10.307692
42    OR        9.985294
43    PA        9.537037
44    PR       10.065217
45    PW       10.915254
46    RI       10.016949
47    SC       10.711864
48    SD        9.739130
49    TN        9.979167
50    TX       10.289474
51    UT        9.980392
52    VA        8.733333
53    VI        9.660714
54    VT       10.166667
55    WA        9.706897
56    WI        9.094340
57    WV        9.777778
58    WY        9.350000

Prompt: To understand gender representation in management, write a SQL query that calculates the percentage of male and female employees in management roles.
Result:
   gender  percentage
0  Female   40.900901
1    Male   59.099099

Prompt: To analyze employee engagement trends, write a SQL query that calculates the average engagement score for each department over the last two years.
Result:
        department_type  avg_engagement
0         Admin Offices        2.576923
1      Executive Office        3.400000
2                 IT/IS        3.050633
3     Production               2.898161
4                 Sales        2.755725
5  Software Engineering        3.222222

Prompt: To evaluate training program outcomes, write a SQL query that calculates the completion rate and average cost of training programs grouped by training type.
Result:
  training_type  completion_rate    avg_cost
0      External        24.077800  556.818008
1      Internal        27.236581  560.417787

Prompt: To understand recruitment efficiency, write a SQL query that calculates the average time to hire for selected applicants grouped by job title.
Error: Execution failed on sql 'SELECT job_title, 
           AVG(julianday(selection_date) - julianday(application_date)) AS avg_time_to_hire
FROM recruitment_data
WHERE status = 'Selected'
GROUP BY job_title;': no such column: selection_date

Prompt: To assess employee distribution, write a SQL query that calculates the number of employees in each business unit and their average years of service.
Result:
  business_unit  employee_count avg_years_of_service
0           BPC             303                 None
1          CCDR             300                 None
2            EW             302                 None
3           MSC             296                 None
4           NEL             304                 None
5            PL             301                 None
6           PYZ             299                 None
7           SVG             304                 None
8           TNS             297                 None
9           WBL             294                 None

Prompt: To analyze performance trends, write a SQL query that calculates the average performance score for each department and filters for departments with an average score above 85.
Result:
Empty DataFrame
Columns: [department_type, avg_performance]
Index: []

Prompt: To understand training participation, write a SQL query that calculates the percentage of employees in each department who attended at least one training program.
Result:
        department_type  participation_rate
0         Admin Offices               100.0
1      Executive Office               100.0
2                 IT/IS               100.0
3     Production                      100.0
4                 Sales               100.0
5  Software Engineering               100.0

Prompt: To analyze hiring trends, write a SQL query that calculates the number of applications received monthly for each job title over the past year.
Result:
    application_month                         job_title  application_count
0                None                Academic librarian                  3
1                None             Accommodation manager                  1
2                None             Accountant, chartered                  1
3                None   Accountant, chartered certified                  1
4                None  Accountant, chartered management                  1
..                ...                               ...                ...
512              None           Water quality scientist                  3
513              None                      Web designer                  4
514              None                Wellsite geologist                  2
515              None                            Writer                  1
516              None                      Youth worker                  1

[517 rows x 3 columns]

Prompt: To evaluate gender diversity in management roles, write a SQL query that calculates the percentage of male and female employees in managerial positions.
Result:
   gender  percentage
0  Female   40.900901
1    Male   59.099099

Prompt: To assess training cost efficiency, write a SQL query that calculates the total cost and average cost per attendee for each training program.
Result:
    training_program_name  total_cost  avg_cost_per_attendee
0    Communication Skills   365023.24             542.382229
1        Customer Service   320575.04             567.389451
2  Leadership Development   323902.03             564.289251
3      Project Management   343313.17             563.732627
4        Technical Skills   323072.61             557.983782

Prompt: To update the department of employees based on recent role changes, write a SQL query that updates the department of employees with the title 'Team Lead'.
Error: 'NoneType' object is not iterable

Prompt: To clean up records, write a SQL query that deletes employees who have been inactive for more than 3 years.
Error: 'NoneType' object is not iterable

Prompt: To reward outstanding employees, write a SQL query that inserts a bonus record for employees with performance scores greater than 90.
Error: Execution failed on sql 'INSERT INTO bonuses (employee_id, bonus_amount, bonus_date)
SELECT employee_id, 1000, date('now')
FROM employee_data
WHERE performance_score > 90;': no such table: bonuses

Prompt: To update training records, write a SQL query that updates the training status of employees who have completed their programs.
Error: 'NoneType' object is not iterable

Prompt: To remove duplicate recruitment entries, write a SQL query that deletes duplicate applicants based on email and job title.
Error: 'NoneType' object is not iterable

Prompt: To add training feedback records, write a SQL query that inserts feedback for employees who completed the 'Leadership Skills' training.
Error: Execution failed on sql 'INSERT INTO training_feedback (employee_id, training_program_name, feedback_date, feedback_score)
SELECT employee_id, training_program_name, date('now'), NULL
FROM training_and_development_data
WHERE training_program_name = 'Leadership Skills' AND training_outcome = 'Completed';': no such table: training_feedback

Prompt: To update job titles for accuracy, write a SQL query that appends 'Junior' to the title of employees hired less than 2 years ago.
Error: 'NoneType' object is not iterable

Prompt: To manage training schedules, write a SQL query that deletes training records older than 5 years.
Error: 'NoneType' object is not iterable

Prompt: To insert new hires into the employee database, write a SQL query that adds employees from a temporary table who are not already in the main table.
Error: Execution failed on sql 'INSERT INTO employee_data (employee_id, first_name, last_name, title, start_date)
SELECT temp_id, temp_first_name, temp_last_name, temp_title, temp_start_date
FROM temp_employees
WHERE temp_id NOT IN (SELECT employee_id FROM employee_data);': no such table: temp_employees

Prompt: To update salary bands, write a SQL query that increases the pay zone by one level for employees in management roles.
Error: 'NoneType' object is not iterable

Prompt: To clear outdated survey data, write a SQL query that deletes survey responses older than 3 years.
Error: 'NoneType' object is not iterable

Prompt: To reward employees who completed high-cost training programs, write a SQL query that inserts reward records into a table for those programs over $5000.
Error: Execution failed on sql 'INSERT INTO training_rewards (employee_id, training_program_name, reward_date)
SELECT employee_id, training_program_name, date('now')
FROM training_and_development_data
WHERE training_cost > 5000 AND training_outcome = 'Completed';': no such table: training_rewards

Prompt: To standardize job titles, write a SQL query that replaces 'Software Engineer' with 'Developer' across all records.
Error: 'NoneType' object is not iterable

Prompt: To clean up terminated employees' training data, write a SQL query that deletes training records for employees no longer active.
Error: 'NoneType' object is not iterable

Prompt: To promote employees with exceptional performance, write a SQL query that updates their title to 'Senior' followed by their current title.
Error: 'NoneType' object is not iterable

Prompt: To insert performance review data, write a SQL query that adds a review for employees with no existing reviews in the current year.
Error: Execution failed on sql 'INSERT INTO performance_reviews (employee_id, review_date, review_score)
SELECT employee_id, date('now'), NULL
FROM employee_data
WHERE employee_id NOT IN (
    SELECT employee_id
    FROM performance_reviews
    WHERE strftime('%Y', review_date) = strftime('%Y', 'now')
);': no such table: performance_reviews

Prompt: To manage outdated job postings, write a SQL query that deletes recruitment entries for positions unfilled for over a year.
Error: 'NoneType' object is not iterable

Prompt: To update department types for reorganization, write a SQL query that sets all 'Operations' departments to 'Business Operations'.
Error: 'NoneType' object is not iterable

Prompt: To insert feedback for employees attending safety training, write a SQL query that adds records to the feedback table.
Error: Execution failed on sql 'INSERT INTO feedback (employee_id, feedback_type, feedback_date)
SELECT employee_id, 'Safety Training', date('now')
FROM training_and_development_data
WHERE training_program_name = 'Safety' AND training_outcome = 'Completed';': no such table: feedback

Prompt: To clean up duplicates, write a SQL query that deletes duplicate employee entries based on email and start date.
Error: 'NoneType' object is not iterable

Prompt: To recognize employee achievements, write a SQL query that inserts award records for employees with a satisfaction score above 90.
Error: Execution failed on sql 'INSERT INTO awards (employee_id, award_date, award_type)
SELECT employee_id, date('now'), 'High Satisfaction'
FROM employee_engagement_survey_data
WHERE satisfaction_score > 90;': no such table: awards

Prompt: To adjust salary ranges, write a SQL query that updates the pay zone for employees in the 'Development' department to one level higher.
Error: 'NoneType' object is not iterable

Prompt: To insert survey reminders, write a SQL query that adds reminder records for employees who have not completed a survey this year.
Error: Execution failed on sql 'INSERT INTO reminders (employee_id, reminder_date, reminder_type)
SELECT employee_id, date('now'), 'Survey Reminder'
FROM employee_data
WHERE employee_id NOT IN (
    SELECT employee_id
    FROM employee_engagement_survey_data
    WHERE strftime('%Y', survey_date) = strftime('%Y', 'now')
);': no such table: reminders

Prompt: To standardize department names, write a SQL query that updates all instances of 'HR' to 'Human Resources'.
Error: 'NoneType' object is not iterable

Prompt: To remove inactive applicants, write a SQL query that deletes recruitment records for applicants whose status is 'Rejected' for over a year.
Error: 'NoneType' object is not iterable

Prompt: To promote long-term employees, write a SQL query that updates their titles to 'Senior' followed by their current title for employees with over 10 years of service.
Error: 'NoneType' object is not iterable

Prompt: To recognize exceptional trainers, write a SQL query that inserts trainer awards for those conducting training programs with an average score above 4.5.
Error: Execution failed on sql 'CREATE TABLE IF NOT EXISTS trainer_awards (
    trainer_name TEXT,
    award_date DATE,
    award_type TEXT
);

INSERT INTO trainer_awards (trainer_name, award_date, award_type)
SELECT trainer, date('now'), 'Excellence Award'
FROM training_and_development_data
WHERE training_program_name IN (
    SELECT training_program_name
    FROM training_feedback
    GROUP BY training_program_name
    HAVING AVG(feedback_score) > 4.5
);
': You can only execute one statement at a time.

Prompt: To assess high-performing employees, write a SQL query that identifies the top 5 employees with the highest engagement scores in each business unit.
Result:
    business_unit first_name  last_name  engagement_score
0             BPC     Judith   Carabbio                 5
1             BPC     Alexis       Moss                 5
2             BPC       Kody    Jimenez                 5
3             BPC     Samuel  MacLennan                 5
4             BPC      Colby      Wolfe                 5
..            ...        ...        ...               ...
579           WBL    Timothy   Sullivan                 5
580           WBL     Jayden      Mckee                 5
581           WBL      Brady      Yoder                 5
582           WBL     Alayna       Hess                 5
583           WBL      Caleb  Schneider                 5

[584 rows x 4 columns]

Prompt: To evaluate work-life balance, write a SQL query that calculates the average work-life balance score for each state.
Result:
   state  avg_balance
0     AL     2.363636
1     AZ     2.967742
2     CA     3.500000
3     CO     3.333333
4     CT     3.200000
5     FL     3.000000
6     GA     3.333333
7     ID     2.903226
8     IN     2.928571
9     KY     2.814815
10    MA     2.983025
11    ME     4.000000
12    MT     1.000000
13    NC     2.800000
14    ND     3.000000
15    NH     4.000000
16    NV     5.000000
17    NY     3.090909
18    OH     5.000000
19    OR     3.666667
20    PA     3.000000
21    RI     3.000000
22    TN     3.000000
23    TX     2.942308
24    UT     3.500000
25    VA     2.500000
26    VT     3.500000
27    WA     2.800000