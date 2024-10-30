

### Exercise: Managing a Print Queue and Browser History

**Objective:** Implement and compare stack and queue operations by simulating two different scenarios—a print queue (using a queue) and a browser history (using a stack).

#### Instructions:

1. **Print Queue Simulation (Queue):**
   - Create a `Queue<string>` to represent a print queue.
   - Allow the user to add documents to the queue.
   - Each time a document is "printed," it should be removed from the queue.
   - Display the queue status after each operation.

2. **Browser History (Stack):**
   - Create a `Stack<string>` to represent browser history.
   - Allow the user to "visit" pages (add URLs to the stack).
   - Allow the user to "go back" to the previous page (pop URLs from the stack).
   - Display the stack status after each operation.

#### Sample Code Structure:

```csharp
using System;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        // Print Queue
        Queue<string> printQueue = new Queue<string>();
        
        // Add documents to print queue
        printQueue.Enqueue("Document1");
        printQueue.Enqueue("Document2");
        printQueue.Enqueue("Document3");
        
        Console.WriteLine("Print Queue:");
        while (printQueue.Count > 0)
        {
            Console.WriteLine($"Printing: {printQueue.Dequeue()}");
        }

        // Browser History
        Stack<string> browserHistory = new Stack<string>();
        
        // Visit pages
        browserHistory.Push("Page1");
        browserHistory.Push("Page2");
        browserHistory.Push("Page3");

        Console.WriteLine("\nBrowser History:");
        while (browserHistory.Count > 0)
        {
            Console.WriteLine($"Going back to: {browserHistory.Pop()}");
        }
    }
}
```

#### Task for Students:
1. Modify the code to allow dynamic user input for adding/removing documents and visiting pages.
2. Have them add comments explaining the differences between the stack and queue behavior they observe.