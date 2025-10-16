Introduction To LangGraph

Module 0
Set API keys, downloaded the ZIP file for the notebooks and the env file.

Module 1)
Video 1: Motivation
Chains in LangGraph are fixed sequences of steps that run in a set order. They’re predictable and fully controlled by the developer, unlike agents, which let an LLM decide the flow dynamically.

Video 2: Simple Graph
A simple graph in LangGraph is a basic structure made of nodes connected by edges. You define nodes with functions and use edges—either simple or conditional—to control the flow from one node to another. StateGraph() helps create this graph, starting from a START node and branching conditionally based on parameters.

changes - Added more nodes. Changed the function to give tips on video games.

Video 3: Langsmith Studio
In this video we visualized graps as flowchart.
<img width="2940" height="1766" alt="image" src="https://github.com/user-attachments/assets/226a656c-e87f-48fe-baa8-c6956b9fc24c" />
changes - made the flowchart in studio with the same example in I did in previous video. We had to edit simple.py file for this.

Video 4: Chain
in this video we learnt about chains. In LangGraph, chains are predefined sequences of steps that execute in a fixed order. They follow a set flow determined by the developer, making them predictable and easy to control.

changes - changed the example with my own. Made my tips function which gave tips for various onine games.

Video 5: Router
In LangGraph, a router is a component that decides which part of the graph to send a message or request to next. It acts like a traffic controller, directing the flow based on conditions or message content, allowing different nodes or chains to be triggered dynamically.
<img width="2940" height="1766" alt="image" src="https://github.com/user-attachments/assets/149b62bf-9c30-4920-a49e-afe9af46ab5c" />

Video 6: Agent
In LangGraph, an Agent is a component that can make decisions and control the flow of the application. It receives messages, decides whether to perform a tool call or move to another node, and can loop back to repeat actions until a satisfactory result is produced. This dynamic decision-making allows the system to handle complex tasks iteratively, similar to the React architecture.

changes - added more fucntions inside the math function like fib and fac. Changed the example at last.
<img width="2940" height="1766" alt="image" src="https://github.com/user-attachments/assets/ae6be0fc-4675-49fb-a14d-5ab79cc466b2" />
<img width="1470" height="883" alt="Screenshot 2025-10-16 at 11 40 35 PM" src="https://github.com/user-attachments/assets/e7346239-6313-4653-943a-270272739a14" />
<img width="2940" height="1766" alt="image" src="https://github.com/user-attachments/assets/52a15dfd-f043-47a1-85cb-8c28c5953d29" />

Video 7: Agent with Memory
In this video we learnt how to add memory using memorysaver().

changes - used the same math function made in previous video with my own fucntions added in this one as well.





