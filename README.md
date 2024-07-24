# DAX-Commands-For-Power-BI

### Power BI

**Power BI** is a business analytics service provided by Microsoft that enables users to visualize and analyze data with greater speed, efficiency, and understanding. It provides tools for aggregating, analyzing, visualizing, and sharing data. Power BI's capabilities include:

- **Data Integration:** Combine data from various sources, including databases, web services, and files.
- **Data Transformation:** Clean, reshape, and transform data to prepare it for analysis.
- **Data Visualization:** Create interactive reports and dashboards with various visualization types like charts, graphs, maps, and tables.
- **Real-Time Analytics:** Monitor data in real time and get instant insights.
- **Collaboration:** Share reports and dashboards with others and collaborate on data-driven decisions.
- **Accessibility:** Access data and reports on multiple devices, including desktops, tablets, and smartphones.

### Data Analysis Expressions (DAX)

**Data Analysis Expressions (DAX)** is a formula language used in Power BI, Power Pivot, and Analysis Services. DAX is designed to work with relational data and perform complex calculations and aggregations. 
Here are some commonly used DAX functions along with their formats:

| **Category**             | **Formula**        | **Description**                                                                                       | **Format**                                   |
|--------------------------|--------------------|-------------------------------------------------------------------------------------------------------|----------------------------------------------|
| **Aggregation**          | `SUM`              | Adds all the numbers in a column.                                                                     | `SUM(<column>)`                              |
|                          | `AVERAGE`          | Returns the average of the numbers in a column.                                                       | `AVERAGE(<column>)`                          |
|                          | `COUNT`            | Counts the number of values in a column.                                                              | `COUNT(<column>)`                            |
|                          | `MAX`              | Returns the largest value in a column.                                                                | `MAX(<column>)`                              |
|                          | `MIN`              | Returns the smallest value in a column.                                                               | `MIN(<column>)`                              |
| **Logical**              | `IF`               | Checks a condition and returns one value if true and another if false.                                | `IF(<condition>, <true_result>, <false_result>)` |
|                          | `AND`              | Checks if all arguments are true, returns true if all are true.                                       | `AND(<logical1>, <logical2>, ...)`           |
|                          | `OR`               | Checks if any arguments are true, returns true if any are true.                                       | `OR(<logical1>, <logical2>, ...)`            |
|                          | `NOT`              | Changes false to true or true to false.                                                               | `NOT(<logical>)`                             |
| **Date and Time**        | `TODAY`            | Returns the current date.                                                                             | `TODAY()`                                    |
|                          | `NOW`              | Returns the current date and time.                                                                    | `NOW()`                                      |
|                          | `YEAR`             | Returns the year of a date.                                                                           | `YEAR(<date>)`                               |
|                          | `MONTH`            | Returns the month of a date.                                                                          | `MONTH(<date>)`                              |
|                          | `DAY`              | Returns the day of a date.                                                                            | `DAY(<date>)`                                |
|                          | `DATE`             | Returns the specified date in datetime format.                                                        | `DATE(<year>, <month>, <day>)`               |
| **Text**                 | `CONCATENATE`      | Joins two or more text strings into one.                                                              | `CONCATENATE(<text1>, <text2>)`              |
|                          | `LEFT`             | Returns the specified number of characters from the start of a text string.                           | `LEFT(<text>, <num_chars>)`                  |
|                          | `RIGHT`            | Returns the specified number of characters from the end of a text string.                             | `RIGHT(<text>, <num_chars>)`                 |
|                          | `MID`              | Returns a specific number of characters from a text string starting at the position you specify.       | `MID(<text>, <start_num>, <num_chars>)`      |
|                          | `LEN`              | Returns the number of characters in a text string.                                                    | `LEN(<text>)`                                |
| **Mathematical**         | `ABS`              | Returns the absolute value of a number.                                                               | `ABS(<number>)`                              |
|                          | `ROUND`            | Rounds a number to the specified number of digits.                                                    | `ROUND(<number>, <num_digits>)`              |
|                          | `CEILING`          | Rounds a number up to the nearest integer or to the nearest multiple of significance.                 | `CEILING(<number>, <significance>)`          |
|                          | `FLOOR`            | Rounds a number down to the nearest integer or to the nearest multiple of significance.               | `FLOOR(<number>, <significance>)`            |
| **Statistical**          | `MEDIAN`           | Returns the median of the numbers in a column.                                                        | `MEDIAN(<column>)`                           |
|                          | `VAR`              | Returns the variance of the numbers in a column.                                                      | `VAR(<column>)`                              |
|                          | `STDEV`            | Returns the standard deviation of the numbers in a column.                                            | `STDEV(<column>)`                            |
| **Filter**               | `FILTER`           | Returns a table that represents a subset of another table or expression.                              | `FILTER(<table>, <expression>)`              |
|                          | `ALL`              | Returns all the rows in a table or all the values in a column, ignoring any filters that might have been applied. | `ALL(<table> or <column>)`                  |
|                          | `CALCULATE`        | Evaluates an expression in a context modified by the specified filters.                                | `CALCULATE(<expression>, <filter1>, <filter2>, ...)` |
|                          | `RELATED`          | Returns a related value from another table.                                                           | `RELATED(<column>)`                          |
|                          | `EARLIER`          | Returns the current value of the specified column in an outer evaluation pass of the row context.      | `EARLIER(<column>, <num_passes>)`            |
| **Time Intelligence**    | `DATESYTD`         | Returns a table that contains a column of the dates for the year to date, given a column of dates.     | `DATESYTD(<dates_column>)`                   |
|                          | `TOTALYTD`         | Evaluates the year-to-date value of the expression in the current context.                             | `TOTALYTD(<expression>, <dates_column>)`     |
|                          | `SAMEPERIODLASTYEAR` | Returns a table that contains a column of dates shifted one year back in time from the dates in the specified column. | `SAMEPERIODLASTYEAR(<dates_column>)` |
|                          | `PARALLELPERIOD`   | Returns a table that contains a column of dates shifted by the specified number of intervals.          | `PARALLELPERIOD(<dates_column>, <interval>, <interval_type>)` |
|                          | `PREVIOUSMONTH`    | Returns a table that contains a column of all the dates in the previous month.                         | `PREVIOUSMONTH(<dates_column>)`              |

