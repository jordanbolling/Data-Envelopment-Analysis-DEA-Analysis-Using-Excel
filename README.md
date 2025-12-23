<h1>Data Envelopment Analysis DEA Analysis Using Excel</h1>

<h2>Description</h2>
This project involved conducting a **comparative efficiency analysis** for a board of four fictional elementary schools (Alton, Beeks, Carey, and Delancey), which are the decision-making units (DMUs) in this case. The objective was to evaluate the **relative performance** of these schools and **identify areas for improvement** in resource utilisation and academic outcomes. Using Data Envelopment Analysis (DEA) and spreadsheet-based linear programming, the study measured the efficiency of each school by **balancing inputs** such as teacher-to-student ratios, supplementary funding, and parental education levels against **outputs** like standardised test scores in reading, math, and history. The findings identified Delancey as relatively inefficient, enabling the development of **targeted recommendations** for resource reallocation and syllabus adjustments to enhance institutional performance. The project was developed as part of an Operations Analytics coursework assignment and demonstrates practical application of mathematical optimisation methods to strategic decision-making in the public sector.
<br />

<h2>Languages and Utilities Used</h2>

- Excel (Spreadsheet Modeling, Linear Programming (LP))
<br />

[Project Excel File](https://github.com/jordanbolling/Data-Envelopment-Analysis-DEA-Analysis-Using-Excel/blob/main/DEA%20Excel.xlsx)

#### **Project Workflow**

A linear equation can be constructed from the objective. For example, Delancey’s maximum relative efficiency (MRE) can be found through identifying the decision variables and implementing an objective function.
<br />

**Objective Function**

Considering the 6 measures which were stated above, they can be divided into the inputs and outputs of the models. The inputs are as follows.

o	Teacher-to-student ratio: This would the total number of teachers divided by the total number of students and can represent each school’s ability to give each student personalised attention.
o	Supplementary funds/student: This represents the school’s ability to provide students with improved resources such as smartboards, additional materials like textbooks, the technology to online learning like meetings and resource dashboards, better learning environments and even new buildings and classrooms.
o	Average educational level of parents: This represents the calibre of background that the student comes from which is essentially their platform for learning.

The decision variables linked to inputs are the weights attributed to each input and are X1,X2,X3 for each respective measure.
The outputs of the model are the average SOL scores for the following.
o	Reading
o	Math
o	History

The decision variables linked to outputs are the weights attributed to each output and are X4, X5 ,X6 for each respective measure.
These are considered by the board as the inputs and outputs as the relative efficiency of each school is measured on how the most critical factors that can potentially affect the SOL scores of young kids, and how well the school can convert their resources and manage these factors to produce the best SOL scores possible. 

The following objective function to find Delancey’s MRE.

Maximize Z = 81X4 + 73X5 + 69X6

These values are used because the board ultimately considers the outputs SOLs for Delancey.

This scenario is linear problem because the constraints can be written as linear inequalities or equations.

*Delancey’s objective is subject to*, 
0.06X1 + 260X2 + 11.3X3 >= 86X4 + 75X5 + 71X6
0.05X1 + 320X2 + 10.5X3 >= 82X4 + 72X5 + 67X6
0.08X1 + 340X2 + 12X3 >= 81X4 + 79X5 + 80X6
0.06X1 + 460X2 + 13.1X3 >= 81X4 + 73X5 + 69X6
This states that the value of each schools’ inputs is greater or equal than its outputs.
This is because it is impossible for school’s efficiency to be greater than 100%. Therefore, a schools’ MRE is less than or equal to 1. Efficiency is equal to sum of outputs divided by the sum of inputs. Therefore, this generates the following inequality.

<p align="center">
<img src="https://i.ibb.co/RwLZ4m5/Screenshot-2025-12-23-at-09-04-39.png"/>
<br/>
</p>

The above constraints are essentially a re-arrangement of this inequality for each school.

*Constraints on the weights*
0.06X1 + 460X2 + 13.1X3 = 1
The weights of a regression model in mathematics generally sum to 1. Additionally, this forces the efficiency score to be less than 1, which is ideal. 
All values are non-negative.

Finally, in order for this problem to be solved through LP, the resources involved must be finite and the objective must be quantifiable (Basumallick,2022), which is correct in this scenario.

This function would yield the following results through spreadsheet modelling.
<br/>

**Spreadsheet Modelling**

<p align="center">
<img src="https://i.ibb.co/5gXvDk08/Screenshot-2025-12-23-at-09-07-18.png"/>
<br/>
<img src="https://i.ibb.co/99PkbMvF/Screenshot-2025-12-23-at-09-07-40.png"/>
</p>

This indicates that Delancey’s MRE is 0.8582.
This is repeated for the schools.

<p align="center">
Alton: <br/>
<img src="https://i.ibb.co/HDHcDBVL/Screenshot-2025-12-23-at-09-10-17.png"/>
  Alton’s MRE is 1
<br/>
Beeks: <br/>
<img src="https://i.ibb.co/N2Ghdkg4/Screenshot-2025-12-23-at-09-10-29.png"/>
  Beeks' MRE is 1
<br/>
Carey: <br/>
<img src="https://i.ibb.co/8gZ8DTBS/Screenshot-2025-12-23-at-09-10-40.png"/>
  Finally, Carey’s MRE is 1
</p>
<br/>

**Conclusion**

It can be concluded that although an MRE of approximately 0.8 seems high at first, when compared to the other schools, Delancey is relatively inefficient. Considering the efficiency formula given above, this means that the school isn’t utilising its inputs as effectively as the other school (approximately 20% less effectively). 
To evaluate, this result doesn’t mean that Delancey isn’t performing well as it is relative.
Additionally, an efficiency score of 1 for the other schools doesn’t mean that they’re perfectly run for the same reason. It is also important to remember that managing a set of schools is harder than owning just 1 school, for example. A board has a set of resources, and they must allocate them effectively and it is extremely difficult to be perfect in this regard.
<br/>

**Recommendations for Delancey**

•	The average education level of parents is the highest and therefore, many of them are college graduates. This might indicate that these parents are encouraging the following.
•	Children to focus on STEM related subjects by acting as role models in this regard even when the children are young (Gülhan,2023). This is alluded to by the school’s below average performance in History.
•	Research suggests that children from wealthier backgrounds tend to take up more extracurricular activities such as music lessons (Social Mobility Commission,2019). This might shift the focus of younger kids slightly away from their studies and alludes to Delancey’s below average SOLs. 

Delancey must invest its well-above average available funds in creating an enivronment that encourages an interest in history and learning in general and even alter the syllabus so it highlights the importance of learning history. They can also invest these funds in AI-powered virtual classrooms that better tailor to a student’s needs as it analyzes each student’s characteristics, which is especially useful in special needs education, and can make recommendations for curriculums, which optimizes an education system (fintelics,2023).
<br/>

**Recommendations for the board**

A comparison between a board’s own schools is critical to effectively manage a set of resources. The next step would be to conduct a similar project but externally, with well-established school boards that own a set of schools or with schools around the areas of Alton, Beeks, Carey and Delancey. This might give the board an idea of where to invest and grow, which potentially attract more students’ applicants and more skilled employees who could increase the efficiency of a school’s services.

