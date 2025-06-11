# cs3241-lab-1-solved
**TO GET THIS SOLUTION VISIT:** [CS3241 Lab 1 Solved](https://mantutor.com/product/cs3241-solved-9/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;113002&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3241 Lab 1  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
LEARNING OBJECTIVES

Basic OpenGL, input &amp; interaction, and animation. After completing the programming assignment, you should have learned

• the basic structure of an OpenGL program,

• how to use some basic OpenGL functions,

• how to use the GLUT (FreeGLUT) callback to get user input and enable interaction,

• how to use double-buffering to make animation look smoother, and

• how to use the GLUT (FreeGLUT) timer callback to control the speed of animation.

TASKS

From the Canvas &gt; CS3241 &gt; Files &gt; Lab Assignments folder, download the ZIP file Lab1_todo_(*).zip.

You are provided with an incomplete C++ application program main.cpp, and your job is to complete it according to the requirements. The program is supposed to do the followings:

• Opens a blank window in the beginning.

• Lets user click the left mouse button anywhere in the window to add a disc centered at the position of the mouse cursor. The disc is given a random size (there is a lower and an upper limits), a random speed (there is an upper limit), and a random color. There is a limit to the total number of discs that the user can add.

• Once added, every disc continues to fly with a constant speed until it hits the window boundary. Then it is reflected (simple reflection with no energy loss).

• User can press the ‘w’ key to toggle between wireframe polygon mode and filled polygon mode.

+x main_done to give the file execute permission before running it.)

Please read the instructions shown in the console window to learn how to operate the program. Try to resize the window and see what happens to the flying discs. Press the ‘w’ key to switch between wireframe polygon mode and filled polygon mode.

Moving discs drawn in filled polygon mode.

Moving discs drawn in wireframe polygon mode.

Follow the following instructions to complete main.cpp as required. You must not add or change any other files.

1) Study the source program very carefully.

2) Complete the DrawDisc() function. The function must draw the input disc using

GL_TRIANGLE_FAN in its color. You can refer to

a. https://www.khronos.org/registry/OpenGL-Refpages/gl2.1/xhtml/glBegin.xml

b. http://www.glprogramming.com/red/chapter02.html#name2

for more information on GL_TRIANGLE_FAN. Note that the vertices on the triangle fan must be provided in counter-clockwise direction. Since the trigonometric functions (e.g. sine and cosine) are quite expensive to compute, you should pre-compute the vertices once (for a unit-radius disc) and re-use them for all the discs later.

3) Complete the MyMouse() function. If the left mouse button is pressed, and if the maximum limit on the number of discs has not been reached, a new disc is generated centered at the position of the mouse cursor. The disc is given

• a random radius (value is between MIN_RADIUS and MAX_RADIUS),

• a random speed in the x direction (value is between −MAX_X_SPEED and −MIN_X_SPEED and between MIN_X_SPEED and MAX_X_SPEED),

• a random speed in the y direction (value is between −MAX_Y_SPEED and −MIN_Y_SPEED and between MIN_Y_SPEED and MAX_Y_SPEED), and

• a random RGB color.

4) Setting up the correct viewing in the MyReshape() function. You should use the glOrtho() or gluOrtho2D() function to set the viewing volume. The viewing volume should be set up in such a way that when the window is resized, the discs do not change their sizes or get distorted on the screen. Instead, the discs can move in the whole window interior, and get reflected by the boundaries of the new window.

5) Complete the UpdateAllDiscPos() function. This function updates the position of each disc by its speed in each of the x and y directions. At its new position, if the disc is entirely or partially outside the left window boundary, then shift it right so that it is inside the window and just touches the left window boundary. Its speed in the x direction must now be reversed (negated). Similar update is applied for the cases of the right, top, and bottom window boundaries.

6) Change the program to use double-buffering.

7) If you have a fast computer, you will notice that the animation is too fast to show anything clearly. You can use the GLUT timer callback to control the speed of the

animation by maintaining a constant frame rate (DESIRED_FPS). Refer to https://www.opengl.org/resources/libraries/glut/spec3/node64.html to find out more about the GLUT function glutTimerFunc().

DO NOT HARD-CODE VALUES. You should write your code in such a way that when the values of the named constants (defined in the beginning of the program) are changed to other valid values, your program should function accordingly. For example, if the value of the constant MAX_NUM_OF_DISCS is changed, your program should allow only that new maximum number of discs to be added.

GRADING

Good coding style. Comment your code adequately, use meaningful names for functions and variables, and indent your code properly. You must fill in your name, and NUS User ID in the header comment.

SUBMISSION

For this assignment, you need to submit only your completed main.cpp.

You must put it/them in a ZIP file and name your ZIP file nus-user-id_lab1.zip. For example, if your NUS User ID is e0123456, you should name your file e0123456_lab1.zip.

Note that you will be penalized for submitting non-required files.

——— End of Document ———
