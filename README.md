Download Link: https://assignmentchef.com/product/solved-cse3122-homework-1
<br>
The operating system that comes with SPIM is very primitive. It only supports a few trivial system calls, such as reading and printing, which are defined in /CPU/syscall.h .  The position of our SPIM OS is shown in the main software architecture diagram below, which indicates that our SPIM OS will be implemented on both SPIM and LINUX. In other words, some of our OS packages will be in MIPS assembly and some of them will be in C++.

<table width="0">

 <tbody>

  <tr>

   <td width="72">Shell.asm</td>

   <td width="82">Search.asm</td>

   <td width="30">…</td>

   <td width="66">Sort.asm</td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td colspan="3" width="250">                           SPIM OS</td>

  </tr>

  <tr>

   <td colspan="2" width="183"> </td>

   <td rowspan="2" width="66">  </td>

  </tr>

  <tr>

   <td width="154">SPIM(MIPS simulator)</td>

   <td width="30"> </td>

  </tr>

  <tr>

   <td width="154"></td>

   <td width="30"></td>

   <td width="66"></td>

  </tr>

 </tbody>

</table>




LINUX (VMware)

HARDWARE

<strong>Figure 1: System architecture </strong>

For this homework, you will implement 3 regular MIPS assembly programs, which can run with the simple SPIM OS without any modification. You will write another MIPS assembly program that needs a new OS service, which will be implemented by you as part of this homework.

First, download and study the SPIM package very carefully from the above link. Then, you will write and test the following MIPS assembly files. Use the provided sample assembly files to learn about how to use the MIPS simulator.

<ol>

 <li>asm : given 3 integers by user, your code will find and show the numbers between the given first and second integers that can be exactly divided by the third given number. For example: Given 10, 20, 3 Print 12,15, 18.</li>

 <li>asm : your code will find the target number by implementing the binary search algorithm for in given integer list. Note that the list should be given in increasing order for the binary search.</li>

 <li>asm : this will be very similar to the previous example. This time the list does not have to be sorted.</li>

 <li>asm : your code will sort the given integers in increasing order by implementing selection sort algorithm.</li>

 <li>asm: You will write a shell program that will be very similar to the example given in the textbook in Fig 1-19. Note that, our current SPIM OS does not support fork, waitpid, and execve system calls, so you will have to implement some system services for this shell. Instead of implementing these three system services, you will implement the Windows system procedure call CreateProcess which loads an assembly file from the disk and executes it. After this call is processed, the OS returns to the caller. You will have to change the SPIM source code in two places:</li>

</ol>

/CPU/syscall.h and /CPU/syscall.cpp . Do not modify any other SPIM code other than these files.




Below are the instructions for homework submission

<ol>

 <li>Download and Install Vmware Player from official site.</li>

 <li>Download and install our virtual machine from https://drive.google.com/open?id=1YppX3lNkyTsHV_lvA4w9TomNCUkpLeEg</li>

 <li>Carefully examine SPIM simulator and MIPS instruction set.</li>

</ol>

<u><a href="https://web.stanford.edu/class/cs143/materials/SPIM_Manual.pdf">https://web.stanford.edu/class/cs143/materials/SPIM_Manual.pdf</a></u> is a very good SPIM documentation.

<ol start="4">

 <li>Your submission includes only the files below

  <ul>

   <li>asm</li>

   <li>asm</li>

   <li>asm</li>

   <li>asm</li>

   <li>asm</li>

   <li>cpp</li>

   <li>h</li>

  </ul></li>

</ol>

















