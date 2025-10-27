Module 3

Video 1 - Streaming Interruptions
Streaming interruptions in LangGraph let you pause and inspect the agent while it’s running, so you can change inputs or control the flow in real time.

Changes made - I added a token counter and formatted output to keep track of how many streamed chunks were received. This helps me understand how the model sends partial responses in real time.”

Video 2 - Breakpoints
I learned that breakpoints let me stop the agent midway to inspect what it plans to do next. This helps me control its actions before allowing it to continue.

Changes made - I added more custom math functions like power and fibonacci to test the tool-calling feature.
The prompt message was updated to match the new functions.

Video 3 - Edit state human feedback
Instead of simply pausing for user approval, I learned how to use breakpoints to directly modify the graph’s state. I also explored the LangGraph UI to understand how the workflow updates in real time.

Changes made - I modified the input prompt to calculate the 6th Fibonacci number and added my own custom Fibonacci function. This helped me test how the agent handles user feedback and continues execution after interruptions.
