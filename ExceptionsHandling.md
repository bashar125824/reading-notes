# Debug for absolute beginners 

---

1. ***For me the first and most important thing is to know what is the problem I face , is it logical ? syntax problem ? , so the first step is to determine the problem then try solve it .***

2. ***OK , I knew what is my problem , then I should put any suggestions to fix this problem , then apply it on the problem .***

3. ***Evaluating step : that's when I rate my suggestions , like I have suggestion A and I apply it on my problem , Is it work ?! , Is it fix the whole problem ? or just a part of it ? ,finally , I can put all my suggestions in the table , then say , that's an EXCELLENT way to solve the problem , and that's a GOOD one , and that's a BAD idea !***

---

# What is an Exception?

---

***Exceptions are a type of error that occurs during the execution of an application. Errors are typically problems that are not expected. Whereas, exceptions are expected to happen within the application’s code for various reasons.***

---

***Applications use exception handling logic to explicitly handle the exceptions when they happen.  Exceptions can occur for a wide variety of reasons. From the infamous NullReferenceException to a database query timeout.***

# The Anatomy of C# Exceptions

---

*Exceptions allow an application to transfer control from one part of the code to another. When an exception is thrown, the current flow of the code is interrupted and handed back to a parent try catch block. C# exception handling is done with the follow keywords: **try**, **catch***

- ## try

---

**A try block is used to encapsulate a region of code. If any code throws an exception within that try block, the exception will be handled by the corresponding catch.**

- ## catch

---

**When an exception occurs, the Catch block of code is executed. This is where you are able to handle the exception, log it, or ignore it.**

---

# Example # 1: The Basic “try catch“

---

```

using System;
using System.IO;

public class ProcessFile
{
    public static void Main()
    {
        try
        {
            using (StreamReader sr = File.OpenText("data.txt"))
            {
                Console.WriteLine($"The first line of this file is {sr.ReadLine()}");
            }
        }
        catch (FileNotFoundException e)
        {
            Console.WriteLine($"The file was not found: '{e}'");
        }
        catch (DirectoryNotFoundException e)
        {
            Console.WriteLine($"The directory was not found: '{e}'");
        }
        catch (IOException e)
        {
            Console.WriteLine($"The file could not be opened: '{e}'");
        }
    }
}

```

**code source :** *[SOURCE](https://docs.microsoft.com/en-us/dotnet/standard/exceptions/how-to-use-the-try-catch-block-to-catch-exceptions)*

---

# Therac-25

---

![IMG](https://upload.wikimedia.org/wikipedia/commons/9/90/Therac25_Interface.png)

Simulated Therac-25 user interface

---

***The Therac-25 was a computer-controlled radiation therapy machine produced by Atomic Energy of Canada Limited (AECL) in 1982 after the Therac-6 and Therac-20 units (the earlier units had been produced in partnership with Compagnie Générale Radiographique (CGR) of France).***

**source :** *[SOURCE](https://en.wikipedia.org/wiki/Therac-25)*

---

# Ariane 5

---

![IMG](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4f/Ariane_5_with_James_Webb_Space_Telescope_Prelaunch_%2851773093465%29.jpg/220px-Ariane_5_with_James_Webb_Space_Telescope_Prelaunch_%2851773093465%29.jpg)

Ariane 5 flight VA-256 on the launch pad with the James Webb Space Telescope in December 2021

---

***Ariane 5 is a European heavy-lift space launch vehicle developed and operated by Arianespace for the European Space Agency (ESA). It is launched from the Centre Spatial Guyanais (CSG) in French Guiana. It has been used to deliver payloads into geostationary transfer orbit (GTO) or low Earth orbit (LEO). The launch vehicle had a streak of 82 consecutive successful launches between 9 April 2003 and 12 December 2017. A direct successor system, Ariane 6, is in development.***

**source :** *[SOURCE](https://en.wikipedia.org/wiki/Ariane_5)*




