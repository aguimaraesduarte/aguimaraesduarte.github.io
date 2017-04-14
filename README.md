# About myself
Hi! Im Andre, and welcome to my website! I am an aspiring Data Scientist, and am fascinated by the things we can do with data. From machine learning to beautiful interactive visualizations, the analysis of data really helps us understand the world from a different perspective. Here, I will showcase some interesting projects that I've worked on, either for work, for school assignments, or just out of curiosity.

# Projects

## [WorldBank Shiny](https://aguimaraesduarte.github.io/WorldBank-Shiny/)

This is an R Shiny app that I created for my Data Visualization course at [USFCA](https://www.usfca.edu/arts-sciences/graduate-programs/analytics). You can try out the deployed app [here](https://aguimaraesduarte.shinyapps.io/worldbank-visualizer/) (there is some server lag when using the app online. However, running it locally should work pretty seamlessly).

The [World Bank](http://databank.worldbank.org/data/reports.aspx?source=2&series=SP.POP.1564.TO.ZS&country=) provides a lot of data for all countries between 1960 and 2015, such as Life Expectancy, Fertility Rate, Population, and many others. In this project, I chose those three variables in order to build an R Shiny app that plots the Fertility Rate vs Life Expectancy throughout the years. Each country is a single point that moves through the plot with time, and the size of the point is proportional to the total population for that country. My goal was to reproduce [this interactive graph](https://www.google.com/publicdata/explore?ds=d5bncppjof8f9_&ctype=b&strail=false&nselm=s&met_x=sp_dyn_le00_in&scale_x=lin&ind_x=false&met_y=sp_dyn_tfrt_in&scale_y=lin&ind_y=false&met_s=sp_pop_totl&scale_s=lin&ind_s=false&dimp_c=country:region&ifdim=country&iconSize=0.5&uniSize=0.035) from Google. The result is fairly close, and I'm happy how it turned out.

## [Firefox Crash Graphs](https://aguimaraesduarte.github.io/FirefoxCrashGraphs/)

This is a project I worked for while at [Mozilla](https://www.mozilla.org/en-US/). You can take a look at the deployed website [here](https://people-mozilla.org/~sguha/mozilla/crashgraphs/).

Firefox Crash Graphs is a daily (weekdays) report of crash analysis on a representative 1% sample of the population from Firefox’s release channel on desktop. Main, content, and plugin crashes are collected and analyzed for this sample of the population and provide an accurate representation of the state of Firefox experience for desktop users and can be used by developers to improve it.

For this project, data was analyzed in [Spark](http://spark.apache.org/) ([PySpark](https://spark.apache.org/docs/0.9.0/python-programming-guide.html) and [SparkSQL](http://spark.apache.org/sql/)) using [Jupyter Notebook](http://jupyter.org/) on a 16-node [AWS](https://aws.amazon.com/) cluster. The graphs were made using the [metrics-graphics](https://www.metricsgraphicsjs.org/) javascript library.

## [Wiki-Walk](https://github.com/nplevitt/Wiki-Walk)

This is a Python project I worked on for my Data Acquisition course at [USFCA](https://www.usfca.edu/arts-sciences/graduate-programs/analytics) with three other students. The final output is a [Flask](http://flask.pocoo.org/) app that runs locally (although it is easily deployable on a server as well).

This project displays the degrees of separation between topics on Wikipedia. This interactive program allows users to visually see the shortest path between two topics. Users can select a start and end term from a dropdown menu, and the program will take them on the shortest journey between these topics through an automated process that clicks on the relevant Wikipedia links.

Due to data storage limits and potentially long run-times, the program was implemented on a fully connected subset of articles, rather than all of Wikipedia. However, given more resources, the program can be easily scaled up to get the degrees of separation between any two topics on Wikipedia.

Alongside Flask, we used [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) to parse the HTML pages from Wikipedia (obtained through GET requests) and [Selenium](http://www.seleniumhq.org/) to create the visual journey that guides the user through the shortest path between two articles.

## [DAU Calendar](https://aguimaraesduarte.github.io/DAU_Calendar/)

This is a simple [Bokeh](http://bokeh.pydata.org/en/latest/) Python app I created as a proof of concept. DAU stands for Daily Active Users, i.e., how many distinct users are active on your product on a given day. This metrics is widely used throughout companies, and is usually visualized as a time series. This is just another visualization, where a calendar is built with that information and shows DAU (and any other useful information) when the user hovers on any date. In this example, I also colored weekends and holidays to show some possibilities.

Another fun idea that could be built on top of this current version is to have the size of the day (either the number or the entire square block) increase or decrease according to the DAU, so days that saw more users active would immediately stand out from within the calendar.

# Contact info
You can contact me via [email](mailto:aduarte@mozilla.com?Subject=Contacting%20from%20your%20github%20page) or find me on [LinkedIn](https://www.linkedin.com/in/aguimaraesduarte/).
