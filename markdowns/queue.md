# Homework: Managing a Print Queue

## Goal 

Continue to practice new material (queue) while applying knowledge aquired over the past few weeks by simulating a printer's document queue.

## Instructions:

1. **Print Queue Simulation (Queue):**
   - Create a `Queue<string>` to represent a print queue.
   - Allow the user to add documents to the queue.
   - Each time a document is "printed," it should be removed from the queue.
   - Display the queue status after each operation.

## Sample Code Structure:

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

        Console.WriteLine("What would you like to do?");
        Console.WriteLine("Options:\n- 'Print' - Print documents in printer queue.\n-'Quit' - End program.");
        
        Console.WriteLine("Print Queue:");
        while (printQueue.Count > 0)
        {
            Console.WriteLine($"Printing: {printQueue.Dequeue()}");
        }
    }
}
```

## Open ended goals to accomplish:

You now have quite a few tools in your tool box. For example, OOP and Error Handling concepts. 

1. Modify and expand the code to allow dynamic user input for adding/removing documents.
2. Add comments explaining the differences between the stack and queue behaviors and why this works the way that it does with the context of a printer queue.

This should give you a hands-on understanding of queues, while applying knowledge of the few previous weeks. This will test to see if we can remember and apply older concepts as we move forward with newer concepts.