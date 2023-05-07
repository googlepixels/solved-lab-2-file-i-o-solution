Download Link: https://assignmentchef.com/product/solved-lab-2-file-i-o-solution
<br>
<p class="ui header product-top-header" title="LAB #2 – File I/O Solution">Each lab will begin with a brief demonstration by the TAs for the core concepts examined in this lab. As such, this document will not serve to tell you everything the TAs will in the demo. It is highly encouraged that you ask questions and take notes.As long as you attended lab 1 or received prior permission for missing the lab, then you can receive any number of points back for finishing the lab prior to this lab #2. Make sure you get checked off at the beginning of lab #2 for credit!!!Pair ProgrammingIn this lab, you can choose a partner for pair programming. You must be checked off together. You only need one computer for pair programming. One person will be the driver, who controls the computer and codes, while the other is the navigator, who observes and advises. After 20 minutes, your TA will switch driver and navigator, continuing this pattern until the task is complete. Please read more about pair programming and the benefits: Pair Programming Student Handout(3 pts) DesignIn this lab, you will read and write to a file. You can copy and paste or download this example file, input.txt. The input file provides details for a webpage in the following format:TitleBackground_colorFont_color Font_size Font_faceContents_of_bodyYour program will read specific information from the file and continue reading thecontents of the body from the file until the EOF (end of file) character. You will output the html to a file called index.html in the public_html directory located in your home directory. You can specify the relative or absolute path to this directory. The absolute path is “/nfs/stak/students/u/username/public_html/index.html”, and the relative would be based on where you are. For example, if you are in a labs directory in a cs162 directory in your home directory, then the relative path is “../../public_html/index.html”.HTML background:All html files need to begin and end with &lt;html and &lt;/html tags. Within these tags are the header (&lt;head &lt;/head) and body tags (&lt;body &lt;/body). The head tag contains title information between the title tags (&lt;title &lt;/title),and the head ends before the body begins. The body tag contains background color information, font tags (&lt;font &lt;/font)that allow you to control the color, size, and face of the font in the body, andbreaks (&lt;br) for newlines in the text.o The body tag contains an attribute called bgcolor. For example:&lt;body bgcolor=”red”o The font tag contains attributes called color, size, and face. For example:&lt;font color=”white” size=”5” face=”comic sans ms”o The break tag (&lt;br) is used to insert a newline in html, and you shouldinsert one at the end of each line break in your content for the body.An example output index.html file corresponding to the input.txt file provided would be:&lt;html&lt;head&lt;titleMy first web page&lt;/title&lt;/head&lt;body bgcolor=”red”&lt;font color=”white” size=”5″ face=”comic sans ms”Woohoo! This is my first webpage!&lt;br&lt;br-Jennifer&lt;br&lt;br&lt;/font&lt;/body&lt;/htmlYou will implement the following functions (with the exact parameters) that read the specific information from a file and output the information in html format.void create_header(ifstream &amp;, ofstream &amp;);void create_body(ifstream &amp;, ofstream &amp;);void create_html(ifstream &amp;);Your main function needs to check to make sure the file you open exists beforemoving forward. If the file doesn’t exist, then you need to provide an error message and get a file name that does exist. Write a design for the main function in the driver file, driver.cpp. Write a design for the create_header(), create_body(), and create_html()functions in the implementation file, webpage.cppAfter 30 minutes, STOP!!!! Your TAs will compare some designs and go over pros and cons to design. (7 pts) ImplementationNow, implement the driver.cpp, webpage.cpp, and webpage.h files. Create a Makefile to manage the compilation of all these files.The first time the index.html file is created, you may need to change permissions to view the file in your web browser. To change the permissions use chmod.chmod 664 index.htmlView the index.html file using a web browser! <a href="http://web.engr.oregonstate.edu/~username/" target="_blank" rel="nofollow noopener noreferrer">http://web.engr.oregonstate.edu/~username/</a>Remember, you and your partner will not receive lab credit if you do not getchecked off before leaving each lab. Once you have a zero on a lab, then it cannot be changed because we have no way of know if you were there or not!!!

5/5 - (2 votes)