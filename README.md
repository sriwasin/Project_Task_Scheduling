# Project_Task_Scheduling

Hypothetical requirements:
<ul>
  <li>Client is a manufacturing company.</li>
  <li>They are looking for software solution to help manage the assembly lines and ensure that all assembly lines are always operating at optimal capacity.</li>
  <li>The key constraint is that the client has multiple product lines. When an assembly of a product line is active, it will utilise certain combination of available assembly lines, preventing them from being used by other product lines (i.e. when an assembly line is used for one product, the assembly of other products for this stage will be halted).</li>
  <li>Each product line uses varying amount of time for each type of assembly (i.e. a food product will spend more time on packaging than a bodycare product).</li>
  <li>The main task is for the software to find the most optimal scheduling where multiple product lines can be assembled in parallel as efficiently as possible.</li>
</ul>

Abstract:
<ul>
  <li>This project explores the concept of NP-Complete problem, particularly on Independent Set so support task scheduling.</li>
  <li>Since Independent Set solution ensures that no conflicting tasks are run at the same time, we can exploit this principle to help the client manage their assembly and create parallel productions for efficiency.</li>
  <li>The project models the scheduling problem as a graph, where nodes represent product lines and edges represent conflicts in resource usage. Solving the Maximum Independent Set identifies the largest set of tasks that can run in parallel without interference.</li>
</ul>
  
Limitations:
<ul>
  <li>For the purpose of this exploration, we assume that there are no other constraints to the client’s production line other that what product lines they have, what assembly lines are required, time involved and what assembly lines are available.</li>
  <li>We will assume that the assembly lines will also function flawlessly in perpetuity (i.e. there is no possibility of disruption to the assembly process).</li>
  <li>We will also assume that when a product line is active on the assembly, it will utilise the required assembly lines at maximum capacity; thus, there will be no capacity left for any other product lines at the time.</li>
</ul>
