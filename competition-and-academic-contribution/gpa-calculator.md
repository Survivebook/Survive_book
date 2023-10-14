# GPA Calculator

[_Find your GPA_](https://gpa.ssbs.club/)

## SSBS GPA Calculator

This is a tool that helps you estimate your GPA score at SSBS.

The source code of this tool is contained in this repository. Feel free to check it out and contribute!

### Suggestions & Issues

You can report suggestions and issues by:

* opening an [issue](https://github.com/JettChenT/GPA/issues) in this repository.
* contacting `JettChenT` in wechat

### Privacy

Our server does not store any information/statistics regarding your GPA score.

When you share your GPA score with others via an `https://gpa.ssbs.club/#<data>` URL, all information related to your grade data is represented in the `<data>` string, hence why the shared URL is so long. Furthermore, `<data>` is completely hidden from our server and would not be logged.

To estimate how much should be spent maintaining this, we keep track of the number of visitors to our website.

You can view the analytics [here](https://analytics.ssbs.club/share/xcOczTBw/GPA). Now you have as much information as we do :)

### Mobile version

The mobile version(a mini program on WeChat) is coming soon!

### Calculation

#### Step 1: Overall grade for each course

Weights:

| Part       | Weight |
| ---------- | ------ |
| Term Score | 0.3    |
| Midterm    | 0.3    |
| Finals     | 0.4    |

The overall score is then calculated as the [weighted average](https://en.wikipedia.org/wiki/Weighted\_arithmetic\_mean) of the entered Term Score, Midterm, and Finals.

For example, if you only entered your Midterms and Finals, respectively, 84 and 89, your overall grade would be $\frac{84\times 0.3+89\times 0.3}{0.3+0.4} = 86.857$

#### Step 2: GPA for each course

This tool will calculate your GPA for each course based on your overall grade and the course level, as shown below.&#x20;

For example, you have an overall grade of $86.857$ in an AP course. Since $86.857>86.5$, the grade would be rounded up to $87$ and considered as `A-`, which means a GPA of $4.7$ for an AP level course.

#### Step 3: Calculating the final GPA

The overall GPA is calculated as the the weighted average of the GPAs for each course, in which the weight for each class is the number of periods there is each week.

For example, for 10th graders, Geography would weigh 0.5

Example:

| course     | weight | gpa |
| ---------- | ------ | --- |
| Math       | 5      | 4.2 |
| Literature | 5      | 4.4 |
| Elective   | 3      | 3.5 |
| Politics   | 0.5    | 3.3 |

Your final GPA will be calculated as follows:

$$\frac{4.2\times5+4.4\times5+3.5\times3+3.3\times0.5}{5+5+3+0.5} = 4.085$$



Original URL: [https://github.com/JettChenT/GPA/blob/main/README.md](https://github.com/JettChenT/GPA/blob/main/README.md)
