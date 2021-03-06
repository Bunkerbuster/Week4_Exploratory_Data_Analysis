<h2>Peer-graded Assignment: Course Project 2<h2>

<h3>Instructions</h3>

<p>Fine particulate matter (PM2.5) is an ambient air pollutant for which there is strong evidence that it is harmful to human health. In the United States, the Environmental Protection Agency (EPA) is 
tasked with setting national ambient air quality standards for fine PM and for tracking the emissions of this pollutant into the atmosphere. Approximatly every 3 years, the EPA releases its database on emissions of PM2.5.
 This database is known as the National Emissions Inventory (NEI). You can read more information about the NEI at the <a href="http://www.epa.gov/ttn/chief/eiinformation.html">EPA National Emissions Inventory web site.</a></p>

<p>For each year and for each type of PM source, the NEI records how many tons of PM2.5 were emitted from that source over the course of the entire year. The data that you will use for this assignment are for 1999, 2002, 2005, and 2008.</p>

<h4>Review criteria</h4>

<p>For each question</P>

<ol>
    <li>Does the plot appear to address the question being asked?</li>
    <li>Is the submitted R code appropriate for construction of the submitted plot?</li>
</ol>


<h4>Data</h4>

<p>The data for this assignment are available from the course web site as a single zip file:</p>

<ul>
    <li>Data for Peer Assessment [29Mb]</li>
</ul>

<p>The zip file contains two files:</p>

<p>PM2.5 Emissions Data (summarySCC_PM25.rds\color{red}{\verb|summarySCC_PM25.rds|}summarySCC_PM25.rds): This file contains a data frame with all of the PM2.5 emissions data for 1999, 2002, 2005, and 2008. For each year, the table contains number of tons of PM2.5 emitted from a specific type of source for the entire year. Here are the first few rows.</p>

[DATA SAMPLE]

<ul>
	<li><b style="color:red" />fips:</b> A five-digit number (represented as a string) indicating the U.S. county</li>
	<li><b style="color:red" />SCC:</b> The name of the source as indicated by a digit string (see source code classification table)</li>
	<li><b style="color:red" />Pollutant:</b> A string indicating the pollutant</li>
	<li><b style="color:red" />Emissions:</b> Amount of PM2.5 emitted, in tons</li>
	<li><b style="color:red" />type:</b> The type of source (point, non-point, on-road, or non-road)</li>
	<li><b style="color:red" />year:</b> The year of emissions recorded</li>
</ul>

<p>Source Classification Code Table (<b style="color:red" />Source_Classification_Code.rds</b>): This table provides a mapping from the SCC digit strings in the Emissions table to the actual name of the PM2.5 source. The sources are categorized in a few different ways from more general to more specific and you may choose to explore whatever categories you think are most useful. For example, source ???10100101??? is known as ???Ext Comb /Electric Gen /Anthracite Coal /Pulverized Coal???.</p>

<p>You can read each of the two files using the <b style="color:red" />readRDS()</b> function in R. For example, reading in each file can be done with the following code:</p>

[DATA SAMPLE]
