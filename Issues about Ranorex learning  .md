# Issues about Ranorex learning  

* How to find proper Ranorex Xpath?   

Step1. Read the document about Ranorex Xpath in Ranorex user guide from the URL (http://www.ranorex.com/support/user-guide-20/ranorexpath.html) or help in Ranorex studio.   

Step2. Use View Spy to track the element’s path, and the specific utilization of View Spy can be found in the URL (http://www.ranorex.com/support/user-guide-20/lesson-9-ranorex-spy.html) or help in Ranorex studio.    

(The element’s path should be modified manually to indentify an unique UI element. In specific situation, it may choose different attribute to mark a UI element, such as id, innertext,  text.) Step3. According to the requirement, reference similar module in the existing testcases.  


*  How to share a variable value between different testcases or modules?  


Step1. Create a new variable   

In a key Sequence action of a module, select “As new Variable” to create a variable.   

Step2. Data binding   

Right-click on the testcase, you can select the “Data binding”.  In Data binding, you can create a new parameter or select the existing parameter to bound the variables in modules.  Then the bounded variables can share the value.  



*  How to run a single module?  
 
Step1. Ranorex is opened in the corresponding module page.    

Step2. Click “VARIABLES” and set the corresponding value of “Domain”.  

Step3.  Run the single module.   


Notice: Run a single module will save a lot of time. But you must run the related testcase to ensure it could perform correctly.

4.	Q: why is running a single module successful, but running the related testcase failed?
A:  There are several elements that have the same path. So Ranorex can't find the proper one.

5.	Q: Which situation we need to use user code?
A:  The existing actions of Ranorex are unable to implement requirements.

6.	Q: How to add new requirement in the existing testcase?
A: 
Step1. Figure out the function and specified realization of the existing testcase.
Step2.  Choose specified located position of new module.
Step3.  In new module, create new actions and elements to realize requirements.

Notice: Don’t create repetitive actions and elements.

7.	Q: Why it runs failed now while the previous test is correct?
A: Possible causes：  

①	Developers have changed the element.

②	Loading speed is too slow.  

③	Jump out the other Windows when run testcase.   

④	The browser is not maximized.   

⑤	Input method is not set as English.   

⑥	The window is not properly closed.   


