# Work-with-Strings-in-Python

<h2>Introduction</h2>

Security analysts work with a lot of string data. For example, some security analysts work on creating and updating IDs such as employee IDs and device IDs, which are commonly represented as strings. As another example, certain network activity will be stored as string data. Becoming comfortable working with strings in Python is essential for the work of a security analyst.

In this lab, I'll practice creating Python code and working with strings. I'll work with an employee ID, a device ID, and a URL, all represented as string data.

<h2>Scenario</h2>

I'm working as a security analyst, and I am responsible for writing programs in Python to automate updating employee IDs, extracting characters from a device ID, and extracting components from a URL.

<h2>Task 1</h2>

In my organization, employee IDs are currently either four digits or five digits in length. In this task, I'm given a four-digit numeric employee ID stored in a variable called employee_id. Convert this to a string format and store the result in the same variable. Later, I'll update this employee ID string so that it complies with a new standardized format.

<h2>Task 2</h2>

Imagine that I have just been informed of a new criteria for employee IDs. They must all be five digits long for standardization purposes.

In this task, I will write a conditional statement that displays a message if the length of the employee ID is less than five digits.

<h2>Task 3</h2>

In this task, I'll build upon the previous code. If an employee ID is only four digits, I'll use concatenation to create a five-digit employee ID number.

Concatenation is a process that allows me to merge strings together. The addition operator (+) in Python allows me to concatenate two strings.

Write an if statement that evaluates whether the length of employee_id is less than 5. When the condition evaluates to True, reassign employee_id by concatenating "E" in front of the four-digit employee ID to create a five character employee ID. Then, display employee_id again.

<h2>Task 4</h2>

Now I'll move on to the next part of my task. Imagine that the characters in a device ID convey technical information about the device. I'll need to extract characters in specific positions from the device ID. Start off by extracting the fourth character.

The variable device_id represents a device ID containing alphanumeric characters; it's already stored as a string.

<h2>Task 5</h2>

Now I will also need to extract the first through the third characters in the device ID. So take a slice of the device ID. I can achieve this using bracket notation in Python. Then, display the slice to examine the result.

<h2>Task 6</h2>

I'll now proceed to the last part of my task. This involves extracting components of a URL.

I'll work with string indices to display various components of a URL that's stored in the URL variable. First, I'll extract and display the protocol of the URL and the :// characters that follow it using string slicing. Consider that the protocol is in the secure format of https when determining the indices for my slice.

<h2>Task 7</h2>

Later in this lab, I'll extract the domain extension. To prepare for this, use the .index() method to identify the index where the domain extension .com is located in the given URL.

<h2>Task 8</h2>

It's a good idea to save important data in variables when programming. This allows for quick and easy tracking and reuse of information.

Store the output of the .index() method in a variable called ind, which is short for index. This index represents the position where the domain extension ".com" starts in the url.

Note that running this cell will not produce an output.

<h2>Task 9</h2>

I can use string slicing to also extract the domain extension of a URL. To do so, I can create a slice. The starting index should be the ind variable. This contains the index where the domain extension begins. The ending index should be ind + 4 (since ".com" is four characters long). Sometimes, like in this situation, it's easier to express the ending index to the starting index. Examine the following code, run it as is, and observe the output.

<h2>Task 10</h2>

Finally, extract the website name from the given URL using string slicing and the ind variable that I defined earlier. In the given URL, the website name is "exampleURL1".

<h2>Conclusion</h2>

What are the key takeaways from this lab?

- Strings are instrumental in storing important, security-related data, such as device IDs and URLs.
- String concatenation allows me to easily combine the information in a string with the information stored in another string.
- String slicing is a powerful technique that enables me to extract any subsection of a string.
- Python has many functions and methods that help analysts work with string values, as well as data that they want to convert to string format.
  - The ```type()``` function returns the data type of its input.
  - The ```str()``` function converts the input object into a string. For example, when called on an integer, ```str()``` returns that integer value converted to a string.
  - The ```len()``` function returns the number of elements in an object. When called on a string, ```len()``` returns the number of characters in that string.
  - The ```.index()``` method finds the first occurrence of the input in a string and returns its location. It provides the index where the substring begins.

