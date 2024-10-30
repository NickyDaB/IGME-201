### Exercise: Creating a Simple Contact Book

**Objective:** Implement a small contact book using a `Dictionary<string, string>`. Students will practice adding, retrieving, and removing contacts using dictionary operations.

#### Instructions:

1. **Create a Contact Book:**
   - Use a `Dictionary<string, string>` where the key is the contact's name, and the value is the phone number.
   
2. **Basic Operations:**
   - Add new contacts to the dictionary.
   - Search for a contact by name to retrieve their phone number.
   - Remove a contact by name.
   - Display all contacts in the dictionary.

#### Sample Code Structure:

```csharp
using System;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        Dictionary<string, string> contactBook = new Dictionary<string, string>();

        // Adding contacts
        contactBook["Alice"] = "123-456-7890";
        contactBook["Bob"] = "987-654-3210";
        contactBook["Charlie"] = "555-123-4567";

        // Retrieving a contact's phone number
        Console.WriteLine("Enter a name to search for:");
        string name = Console.ReadLine();

        if (contactBook.ContainsKey(name))
        {
            Console.WriteLine($"Phone number for {name}: {contactBook[name]}");
        }
        else
        {
            Console.WriteLine($"{name} not found in contacts.");
        }

        // Removing a contact
        Console.WriteLine("Enter a name to remove from contacts:");
        string removeName = Console.ReadLine();

        if (contactBook.Remove(removeName))
        {
            Console.WriteLine($"{removeName} has been removed from contacts.");
        }
        else
        {
            Console.WriteLine($"{removeName} not found in contacts.");
        }

        // Displaying all contacts
        Console.WriteLine("\nAll Contacts:");
        foreach (var contact in contactBook)
        {
            Console.WriteLine($"{contact.Key}: {contact.Value}");
        }
    }
}
```

#### Task for Students:
1. Modify the code to allow dynamic user input for adding multiple new contacts.
2. Add error handling for duplicate contact names when adding.
3. Have them try to find a contact that does not exist to observe what happens.

This exercise will provide a solid introduction to dictionary operations, focusing on practical usage and common dictionary methods.