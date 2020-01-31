# lovely-R-shiny-layouts
Trying to clarify the different kinds of R files that shiny can be used in, and to show different dashboard layouts

There are two different file types in R that can use shiny to make features with which users can interact, e.g. dropdown boxes.
Here's a summary:

### 1. R Markdown
To create an R Markdown file in R:  
File > New File > R Markdown

In the 'New R Markdown' window, choose 'Shiny' and then 'Shiny Document'.  Give it a title, click OK and off you go.  RStudio is kind enough to give you a ready-made dummy R Markdown document at this point, showing some text and an example interactive chart.  This can simply be deleted if not of interest.
The file extension for your new Shiny document is **.Rmd**  
You'll notice that in the YAML section at the top of the document, the following line has been inserted: **runtime: shiny**  
This means that your document is ready to use interactive elements from the shiny package.

There are two main ways to structure your interactive R Markdown document:  *(but what about shinydashboard package?!)*

#### 1a. Straightforward RMarkdown with tabs: a 'vertically scrolling web page' type of product

An example of this format would be the Observatory Analytical Team's *Alcohol profile:* https://publichealthwales.shinyapps.io/AlcoholinWales/

If this is your choice of product, then there's nothing more you need to do to set it up - simply start typing in the white space in the document, and this will form the text within your document.  To insert chunks of code, either to manipulate data or insert interactive shiny elements, select 'Insert > R' at the top-right of the code window.
If you would like to insert tabbed pages within the document, see section 3.1.3 in the following guide:
https://bookdown.org/yihui/rmarkdown/html-document.html
 

#### 1b. Flexdashboard: a dashboard built with the flexdashboard package

Flexdashboard is the best tool if you want to build a dashboard as easily as possible in R.
Building a Shiny app might offer more flexibility in layout and design, but requires more advanced coding.
Comprehensive information on the flexdashboard package is available here:
https://rmarkdown.rstudio.com/flexdashboard/index.html


### 2. Shiny app
To create a Shiny app in R:
File > New File > Shiny Web App
