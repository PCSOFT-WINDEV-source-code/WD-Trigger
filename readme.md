  
<span style="font-family:Arial sans-serif;font-size:16px;">WD Trigger</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">This example explains how to use the triggers with WINDEV. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">A trigger is a WLanguage procedure automatically called by the HFSQL engine whenever a HFSQL function is run. </span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">The following topics are presented in this example:</span>

<span style="font-family:Arial sans-serif;font-size:14px;">1/ how to branch a trigger on a HFSQL function</span>

<span style="font-family:Arial sans-serif;font-size:14px;">2/ the code that must be used in the function called by trigger.</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Summary of the example supplied with WINDEV: </span>

<span style="font-family:Arial sans-serif;font-size:14px;">This application is used to enter the expenses for the contributors of a company. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">Two modes can be used:</span>

<span style="font-family:Arial sans-serif;font-size:14px;">- the mode with read/write rights</span>

<span style="font-family:Arial sans-serif;font-size:14px;">- the mode with read-only rights. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">The triggers will be used to control the access to the files according to the current mode. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">In this example, the triggers are also used to write the different events into a log file. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">This log file can be directly consulted in the application.</span>

  
  
<span style="font-family:Arial sans-serif;font-size:14px;">( \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ ° \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ )</span>

  
<span style="text-decoration:underline;font-family:Arial sans-serif;font-size:10px;">Conditions of Use.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">This program is supplied for training purposes.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">The use of this program is the responsibility of the user. </span>

<span style="font-family:Arial sans-serif;font-size:10px;">PC SOFT will not be liable for damage or loss of any nature whatsoever, including data loss, corruption or deterioration as a result of using this program.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Any person owning a WINDEV 28 US license is authorized to use and/or modify the program and to use it in their own applications. </span>

<span style="font-family:Arial sans-serif;font-size:10px;">In this case all references to PC SOFT and/or to WinDev or WebDev must be removed.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">You may not distribute or sell this example program without substantial modification or include it in another application unless the application is very large.</span>

  
<span style="font-family:Arial sans-serif;font-size:10px;">No Hot Line Support is available for this program.</span>

  
<span style="font-family:Arial sans-serif;font-size:10px;">CAUTION: Many users may have modified this program. </span>

<span style="font-family:Arial sans-serif;font-size:10px;">Make sure that you are working with the original version of this program.</span>

  
  
  
  