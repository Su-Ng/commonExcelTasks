# Common Excel Tasks
In many testing jobs, there are are lots of data needed to be checked for various scenarios. Excel is commonly used for such tasks. 
However its is possible to replace the commonly used Excel functions such as pivot table and vloopUp with python coding. 

# pivot_table

titanic.groupby(['sex', 'class'])['survived'].aggregate('mean').unstack()

is equivalent to

titanic.pivot_table('survived', index='sex', columns='class')

# vLookUp

What is vlookup? Vlookup is essentially combining two different tables using a shared column.

