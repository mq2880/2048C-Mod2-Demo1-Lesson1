# 2048C-Mod2-Demo1-Lesson1

# Module 2: Creating and Styling HTML Pages

Wherever a path to a file starts with *[Repository Root]*, replace it with the absolute path to the folder in which the 20480 repository resides. For example, if you cloned or extracted the 20480 repository to **C:\Users\John Doe\Downloads\20480**, change the path: **[Repository Root]\AllFiles\20480C\Mod01** to **C:\Users\John Doe\Downloads\20480\AllFiles\20480C\Mod01**.

# Lesson 1: Creating an HTML5 Page

### Demonstration: Using HTML5 Features in a Simple Contact Form

#### Preparation Steps 

Ensure that you have cloned the 20480C directory from GitHub (**https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/master/Allfiles**). It contains the code segments for the labs and demos in this course.

#### Demonstration Steps

#### Divide the Content for a Page into an Article with Sections

1. Open Microsoft Visual Studio 2017.

2. In Visual Studio, on the **File** menu, point to **Open**, and then click **Project/Solution**.

3. In the **Open Project** dialog box, browse to the **[Repository Root]\Allfiles\Mod02\Democode\Starter** folder, click **DemoWebSite.sln**, and then click **Open**.

4. In Solution Explorer, expand **DemoWebSite** project, and then double-click **ContactUs.html**.

5. In the **ContactUs.html** file, enclose the contents of the **&lt;body&gt;** element in an **&lt;article&gt;** element as shown in the following code example:

   ```html
       <!DOCTYPE HTML>
       <html lang="en">  
         ...
         </head>
         <body>
           <article>
           ...
           </article>
         </body>
       </html>
   
   ```

6. Within the **&lt;article&gt;** element, enclose the first three **&lt;p&gt;** elements containing the company name, address, and contact email in a **&lt;section&gt;** element, as shown in the following code example:

   ```html
       ...
       <h1>Contact Contoso Conferencing</h1>
         <section>
           <p>Contoso Conferencing Ltd.</p>
           <p>123 South Street<br />
           Somewhere<br />
           Over There<br />
           <em>USA</em></p>
           <p>
             <a href="mailto:contact@contoso.com">contact@contoso.com</a>
           </p>
         </section>
       <p>
       If you would like to contact Contoso Conferencing ...
       </p>
       ...
   ```

7. Wrap the HTML form and **&lt;p&gt;** element immediately above it in a second **&lt;section&gt;** element, as shown in the following code example:

   ```html
       ...
       <section>
         <p>
         If you would like to contact Contoso Conferencing ...
         </p>
         <form method="POST" action="support.aspx">
           ...
         </form>
       </section>
       ...
   ```

8. On the **File** menu, click **Save All**.

#### Add a Header and a Footer to the Page

1. Enclose the **&lt;h1&gt;** element near the top of the **ContactUs.html** file in a **&lt;header&gt;** element, as shown in the following code example:

   ```html
       ...
       <article>
         <header>
           <h1>Contact Contoso Conferencing</h1>
         </header>
         ...
       </article>
       ...
   ```

2. Add the following **&lt;img&gt;** element to the **&lt;header&gt;** element, which is above the **&lt;h1&gt;** element.

   ```html
       <header>
         <img src="images/Contoso.png" alt="Company Logo" />
         <h1>Contact Contoso Conferencing</h1>
       </header>
   ```

3. Add the following HTML markup immediately after the **&lt;/article&gt;** tag near the end of the document such that the code should look as follows:

   ```html
       ...
       </article>
       <footer>
         <p>
           <small>
             Last updated 
             <time datetime="2012-08">
               August 2012
             </time>
           </small>
         </p>
       </footer>
     </body>
   </html>
   ```

4. On the **File** menu, click **Save All**.

#### View the Structure of the Page by Using the F12 Developer Tools

1.	On the **Debug** menu, click **Start Without Debugging**.
2.	In Microsoft Edge, if the **Intranet settings are turned off by default** message appears, click **Don’t show this message again**.
3.	Press F12.
4.	In the **F12** window, click the **HTML** tab.
5.	Expand the **&lt;html&gt;** element.
6.	Expand the **&lt;body&gt;** element.
7.	Expand the **&lt;article&gt;** element, and then verify that it contains a **&lt;header&gt;** element and two **&lt;section&gt;** elements.
8.	Expand the **&lt;header&gt;** element.
9.	View the **&lt;h1&gt;** element.
10.	In the **F12** window, click each element and verify that Microsoft Edge surrounds each element as you select it.



#### Make a Temporary Change to the Page by Using the F12 Developer Tools

1.	In the **&lt;h1&gt;** element, click **Contact Contoso Conferencing**.
2.	Change this text to **We'd love to hear from you…**, and then press Enter.
3.	Verify that Microsoft Edge displays the modified text.
4.	To close the **F12** window, press F12.
5.	Close Microsoft Edge, and then close Visual Studio.