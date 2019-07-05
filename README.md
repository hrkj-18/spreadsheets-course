# Spreadsheets Course

### Basics
=121+21
142

### Mathematics
+
-
*
/
^

### Percentages
= 2 * 21%

### Comparison Operators
<, >: smaller/greater than
<=, >=: smaller/greater than or equal to
=, <>: equal/not equal to

### Text
'23 = 23 in text

### Formatting
Format > Number > More formats

### Absolute references
$A$12

### What IS*() the data type?
=ISTEXT()
=ISNUMBER()
=ISDATE()
=ISLOGICAL()
=ISURL()
=ISFORMULA()
=ISBLANK()

### Coversion
=N()
=TO_PERCENT()

=SUM()
=AVERAGE()
=CONVERT(A2, "sec", "min")

### Logarthmic Transformations
=LOG10()
=LN()

### Exponential transformations
=EXP()
=POW(2,CELL)

### Square and square root transformations
=SQRT()

### Min and Max
=MIN(Range)
=MAX(Range)

### Mean and Median
=SUM(Range)
=AVERAGE(Range)
=MEDIAN(Range)

### Rank
=RANK(value, Range, [is_ascending])

### Right and Left
=RIGHT(Beauty and the Beast (2017),4) = 017)
=LEFT(Star Wars: The Last Jedi,3) = Sta

### Length and Search
=LEN()
=SEARCH(" ", cell)

### Concatenate
=CONCATENATE(value1, value2, value3, ....)

### Weekday
=WEEKDAY(date, [type]): evaluates to the day of the week of a date. type is 1, 2 or 3.
type = 1: Sunday is day 1 and Saturday is day 7 (default)
type = 2: Monday is day 1 and Sunday is day 7
type = 3: Monday is day 0 and Sunday is day 6

=DATEDIF(start_date, end_date, unit)
"Y": the number of years between two dates
"M": the number of months between two dates
"D": the number of days between two dates

### Rounding numbers
ROUND(x, n) rounds x to the nearest n decimal places.
CEILING(x, y) rounds x up to the nearest multiple of y.
FLOOR(x, y) rounds x down to the nearest multiple of y.
=ROUND(0.746, 1) = 0.7
=ROUND(325, -2) = 300

=FLOOR(1.0985) = 1
=FLOOR(1.0985, 0.01) = 1.09

=CEILING(0.7461, 0.1) = 0.8

FLOOR(-1.5) is -2 and CEILING(-1.5) is -1

Google Sheets has two related functions called FLOOR.MATH() and CEILING.MATH(). When given one or two arguments, they behave in the same way as FLOOR() and CEILING() respectively. However, you can pass the value 1 to a third argument to make them round towards or away from zero.

That is, FLOOR.MATH(-1.5, , 1) is -1 and CEILING.MATH(-1.5, , 1) is -2

### Random Numbers
=RAND()
=RANDBETWEEN(lo, hi)
=NORMINV(RAND(), 3, 2) mean 3 and standard deviation 2

### Logical Operations
=NOT()
=AND()
=OR()

### Flow Control
=IF(condition, this op if condition true, else this op)
=IFS(condition1, op1, condition2, op2, .....conditionN, opN)
=SWITCH(Range, "value1", opValue1, "value2", opValue2, ....)

### Blanks, missing values, & errors
Error	Cause
#DIV/0!	Dividing by zero.
#VALUE!	Nonsense data in a calculation.
#REF!	Referencing a cell that has been deleted.
#NAME?	Forgetting to quote a string.
#NUM!	Numbers being out of range.
#N/A	Missing value.
#ERROR!	Syntax problem in a formula.

=ISBLANK()
=COUNTBLANK(Range)
=NA() = #N/A
=ISERROR()
=ISERR()

### Cell Addresses
=ROW()
=COLUMN()
=ADDRESS(H5, I5) Absolute
=ADDRESS(H5, I5, 4) Relative
=INDIRECT()
=OFFSET(cell_reference, offset_rows, offset_columns, [height], [width])
=INDEX(Range, row, column)

### Lookups & matching
=VLOOKUP(search_key, range, index, [is_sorted])
=SORT(range, sort_column, is_ascending, [sort_column2, ...], [is_ascending2, ...])
=MATCH(search_key, range, [search_type])

=UNIQUE(Range)
=COUNTIF(Range,value)
=COUNTIFS(Range1, value1, Range2, value2...)
=SUMIF(Range1, value1 in Range1, Range2) = Sum of values coresponding to value1 in Range2
=AVERAGEIF(Range1, value1 in Range1, Range2) = Average of values coresponding to value1 in Range2
