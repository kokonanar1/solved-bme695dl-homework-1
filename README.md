Download Link: https://assignmentchef.com/product/solved-bme695dl-homework-1
<br>
The goal of this homework is to improve your understanding of the Python OO code in general, especially with regard to how it is used in PyTorch. This is the only homework you will get on general Python OO programming. Future homework assignments will be specific to using PyTorch classes directly or your own extensions of those classes for creating your DL solutions.

<h1>2             Programming Tasks</h1>

<ol>

 <li>Create a class named People that has three instance variables named:

  <ul>

   <li>first_names</li>

   <li>middle_names</li>

   <li>last_names</li>

  </ul></li>

 <li>Use the Python’s package random to generate an array of 10 random strings of length 5 for each of the aforementioned three variables. Each string consists of 5 randomly generated lowercase alphabet letters. Make sure to initialize the seed of the random number generator to 0 before generating random strings. To generate a single lowercase alphabet letter, you can use the following Python statement (after importing the string and random Python packages):</li>

</ol>

random.choice(string.asciilowercase)

<ol start="3">

 <li>Create an instance of your class and store the three arrays in the three instance variables of the People instance</li>

 <li>Expand your class definition and endow it with an iterator. Iterating through the data stored in the People instance should print out the 10 names, with each name in the following order:</li>

</ol>

first_name second_name third_name

<ol start="5">

 <li>Further expand the definition of the class and endow it with another instance variable that takes one of the following three values:

  <ul>

   <li>first_name_first (<em>i</em>.<em>e</em>., a name should appear in the format “first middle last”)</li>

   <li>last_name_first (<em>i</em>.<em>e</em>., a name should appear in the format “last first middle”)</li>

   <li>last_name_with_comma_first (<em>i</em>.<em>e</em>., a name should appear in the format “last, first middle”)</li>

  </ul></li>

</ol>

Note that the last choice is basically the same as the second choice, except that the last name is followed with a comma (a practice that is used in some countries and in some publications when showing author names).

Now show that you can create an instance of your expanded class with a value for the new instance variable. And also show that when you iterate through the instance, it prints out the names in the chosen format. Illustrate that for the 3 different formats in the order given by the above bullets.

<ol start="6">

 <li>Further expand the definition of the class and make its instances callable. With this new definition for the People class, when you apply the function-call operator ‘()’ to an instance, it should print out a sorted list of just the last names.</li>

 <li>Finally, extend your People class into a subclass named PeopleWithMoney . Endow this class with its own instance variable named wealth. Initialize wealth with 10 randomly generated integer between 0 and 1000. Again create an iterator for this class that gets a part of its work done by the iterator of the parent class. Now demonstrate the following:

  <ul>

   <li>When you iterate through an instance of PeopleWithMoney, that should print each individual’s name (following the order “first middle last”) and the wealth associated with the individual. Also make the instances of the subclass callable. When you call an instance of PeopleWithMoney with the function-call operator ‘()’, that should print out the names of all the individual sorted by the size of their wealth in the ascending order.</li>

  </ul></li>

</ol>

<h1>3             Output Format</h1>

The output of your code, that corresponds to the tasks above, will be evaluated using automated scripts. Thus, it is of particular importance that you follow the suggested output format below <strong>precisely</strong>. Note that there isn’t a

newline character before the first output line nor after the last output line. Each output segment below is separated by a single newline character.

<table width="527">

 <tbody>

  <tr>

   <td width="527">first_name1 middle_name1 last_name1 first_name2 middle_name2 last_name2... first_name10 middle_name10 last_name10last_name1 first_name1 middle_name1 last_name2 first_name2 middle_name2... last_name10 first_name10 middle_name10last_name1, first_name1 middle_name1 last_name2, first_name2 middle_name2... last_name10, first_name10 middle_name10sorted_last_name1 sorted_last_name2 ... sorted_last_name10first_name1 middle_name1 last_name1 wealth_amount1 first_name2 middle_name2 last_name2 wealth_amount2...first_name10 middle_name10 last_name10 wealth_amount10first_name middle_name last_name lowest_wealth_amount first_name middle_name last_name second_lowest_wealth_amount...first_name middle_name last_name highest_wealth_amount</td>

  </tr>

 </tbody>

</table>

1

2

3

4

5

6

7

8

9

10

11

12

13

14

15

16

17

18

19

20

21

22

23

24

25

26

27

28

29

30

31

32

33

34

35

36

37

38

39

40

41