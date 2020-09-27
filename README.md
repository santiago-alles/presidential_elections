# presidential_election_19832019
Presidential Elections in Argentina, 1983-2019
==============================================

Last update:
------------------
01-05-2020

</br >The Argentine president is elected for a four-year term and limited to two consecutive terms in office, but she is eligible to run for re-election after a four-year interval. Presidents were elected for a six-year term without reelection until 1994.

Argentina has utilized a modified version of the double complement rule to elect its president, since a constitutional amendment in 1994 supressed the Electoral College. A runoff between the top two presidential candidates from a first round is held unless the plurality candidate either wins 45% +1 of the vote or wins at least 40% of the vote and at the same time has a margin of victory over the second place candidate of more than 10%.

Presidents had been elected by a 600-member Electoral College in 1983 and 1989 elections. College members were elected using D’Hondt formula, and the number of seats by province was allocated by Law 22.847/1983.

Description
-----------

Data contains the results of presidential elections in Argentina, from 1983 to 2019. It includes election results of first and second rounds.

It contains data of dozens presidential candidates, running in nine presidential elections, over the 24 electoral units (provinces). Data is built by political party at the provincial level.

This dataset comprises information of:

(a) presidential and vice presidential candidate, and,<br />
(b) election results, by province.

The source of the data is the national electoral authority, <i>Dirección Nacional Electoral</i>. Available at: <http://www.elecciones.gob.ar/>, accessed: 12/19/2016.

Data Availability
------------------

Data can be directly called from the repository using Hadley Wickham's <a href="https://cran.r-project.org/web/packages/readr/readr.pdf" target="_blank">readr</a> package:

<pre><code>require(readr)
url <- 'https://raw.githubusercontent.com/santiago-alles/presidential_elections/master/'
file <- 'JELS2016_PRESelections_ARG19832019.csv'
read_csv(paste(url, file, sep='/')) -> dat
</code></pre>

Special characters may appear in name and last name variables. Character strings might be converted to <code>UTF-8</code> encoding using <code>iconv</code>:

<pre><code>iconv(x, from = 'latin1', to = 'UTF-8')</code></pre>

Suggested Citation
-------------------

When using this dataset, please cite:

<b>Alles</b>, Santiago, Mark P. <b>Jones</b>, and Carolina <b>Tchintian</b>. 2016. The 2015 Argentine Presidential and Legislative Elections. <i>Electoral Studies</i>, 43: 184-187. http://dx.doi.org/10.1016/j.electstud.2016.05.001

Alternative Sources on Election Data
-------------------

Lupu and Stokes have published more detailed election data, for a larger period of time: their dataset combines department-level electoral results for all available national elections in Argentina from 1912 to 2003, with census data on urbanization, literature, and population.

Differently, their dataset exclusively focuses on major parties: PJ, UCR, Socialists and Conservatives; while this dataset includes complete election results.

(Last time I checked) Lupu & Stokes dataset was available at: <http://www.noamlupu.com/data.html>
