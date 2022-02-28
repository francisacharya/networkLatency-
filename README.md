# networkLatency-

Selecting 
Dijkstra to traverse a list of all “unoptimized” vertices
There may be other method to do this task 
more research time needed.
At the moment its just the algorithm and some sample data. You can view the code in networklatency.php file

Network Path Test
Imagine that there is a small network with a number of interconnected devices. Each connection has
a latency parameter which is expressed in milliseconds. Your task is to write a program that will
determine whether a signal can travel between two devices in a given amount of time or less.
Implementation Guidelines:
1. The program should be executable from command line and accept one parameter - csv file path.
2. CSV file structure:
Format: Device From, Device To, Latency (milliseconds)
Contents:
A,B,10
A,C,20
B,D,100
C,D,30
D,E,10
E,F,1000
Interpretation:
A connects to B and it takes 10 milliseconds for signal to travel between two devices. A to C and it
takes 20 milliseconds, B to D and it takes 100 milliseconds etc.
3. The program should then continually wait for user input. Format should be [Device From] [Device
To] [Time] (e.g A F 1000 followed by ENTER key). If the signal can travel from A to F in 1000ms or
less then output the signal path and total travel time in milliseconds otherwise print "Path not found".
If user enters QUIT then terminate the program.
4. You are only required to output first path that meets the time constraint. It does not have to be the
shortest path.
Hints:
Think of the best data structure to accommodate devices and connections and write your code
accordingly.
Submission:
Please commit all your code to a Github public repository and send us the URL. We would like to see
your commit history and instructions on how to run the program from command line.
Sample Input / Output (based on above CSV data):
Input: A F 1000
Output: Path not found - cont over page

Subscribe-HR – ABN 86 132 590 277
1300 543 544
info@subscribe-hr.com.au
Input: A F 1200 Output: A => B => D => E => F => 1120
Input: A D 100 Output: A => C => D => 50
Input: E A 400 Output: E => D => B => A => 120
Input: E A 80 Output: E => D => C => A => 60
