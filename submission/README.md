# Project 2

### Introduction

In this project, we would like to answer questions about the enrollment of engineering programs. We generate 4 visualizations exploring different features of the enrollment data. Detailed features can be found in [Proj2Note.ipynb](https://github.com/INFO-4602-5602/project-2-ncwit-team-3/blob/master/Proj2Note.ipynb).

**1. How do female and male students perform before and after going into engineer programs?**

We visualized the correlation of college GPA and High school grades (SAT, ACT Math, and High school GPA) in both female and male students. We thought this is interesting because grades might be potential reasons that students want to stay in the program if their work is successful. Therefore, it might influence university student retention.

We used **scatterplot** with a linear regression line to show the correlation between GPA and high school grades because the slope of. Also, we built selectors to query from genders and high school grades for comparison. After that, you could click on comparing button to draw the regression line of the opposite gender. However, showing the linear regression in different scatterplot is hard to compare, and sometimes it is hard to say which line has larger slope. Because of that, we tried other visualization way to show the correlation. Beside the scatterplot, we drew two circles representing college GPA and high school score. The overlapping area emphasizes the difference of each correlation.

**2. How is the race distribution in these institutions?**


The dataset has lots of fields of population of different races. The distribution may be not related to the NCWIT, but it's still very interesting to see how the distribution looks like in these institutions, especially in these majors. And by separating the data by the school year, we are also able to see how the distribution changes over these years.

We used **pie chart** to visualize the data because it fits for visualizing the distribution best. We first have a pie chart which shows the number of students each school year. It's mainly used to navigate through data on different years, by clicking on any arcs on the pie chart, another pie chart showing the race distribution on the corresponding year will pop up on the left. Though the distributions are not exactly the same, we can easily see that the biggest part is white then Asian. But Asians are increasing year by year.

**3. How does student retention rate go from year to year?**

Student retention rate is one of the most important thing that every university cares about. Plotting the retention rate of every year can evaluate the programs/schools policy on retaining students. We calculated the retention ratio by subtracting the total student number in this year from that in the next year, and then average the difference among 4 years.

Since it is a temporal data, we chose **line chart** to visualize this trend so that we can see the change of the retention rate. We can see that in average, female students have lower retention rate than male students. The interesting thing is that, after 2008, female's retention rate grows largely and close to male's retention rate. To show more details, we visualize the details by clicking on the dots. You can know retention rate of Freshman, Sophomores and others, under the condition of different time that major has been selected.

**4. How well does Extension Service help with students GPA?**

Since NCWIT provides Extension Service to help institution on student retention, we would like to know the relationship of student GPA in an institution that is with or without the extension service. Suppose that GPA is a feature that impact students' willingness of staying, we want to explore how well female and male students perform on their studies in institutions with Extension Service support, comparing to those without ES support.

We used **bar chart** to visualize the data because it could easily tell the difference between two condition by the height difference. We encountered some difficulty in visualizing this concept due to the lack of dataset. The y axis is the difference between female GPA and male GPA. According to the result, students have lower GPA difference and it is positive, which means most of female students GPA are high, in the institution with Extension Service consulting.

---

**Team Members:**

Yijun Zhang, Yuhan Lin, Chih-Wei Lin

**Contribution:**

Three of us explored the dataset and discussed the idea together.

Yijun is responsible for all the data preprocessing work and deal with missing value.

Yuhan works on the visualization using D3 and create the basic graph and logics.

Chih-Wei adds the animation and interaction on top of Yuhan's work to perform interactive views.

---

### How to run it?

- Under the submission directory, start a local server using python 3:

    ```bash
    $ python3 -m http.server <port number>
    ```

    Default should be port 8000.

    Please install python3 if you don't have it.

    Mac OS:
    ```
    $ brew python3
    ```

    Linux:
    ```
    $ sudo apt-get python3
    ```

- Open the browser and go to:

    ```
    http://localhost:<port number>
    ```
