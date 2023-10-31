# A Quick Guide to Programming

This document serves as a reference sheet for the various languages and terms you might encounter in the vast world of tech. This is by no means a comprehensive list but may offer guidance regarding the languages you may want to look into depending on your field of interest or make certain resources more accessible by giving you an explanation for some common terms.

## Commonly Used Terms

The following are some terms I hear all the time that typically mean nothing to people outside of this field. People like to fight over the exact meaning of a lot of these, but the definitions here should give you a decent understanding until you can decide for yourself exactly what these all mean. 

- **frontend:** refers to the part of the application that users directly interact with, also known as the **UI** (user interface). Frontend engineers can sometimes be responsible for both designing and creating this part of the application, or UI designers create prototypes that engineers implement.
- **backend:** refers to the part of the application that the user doesn't see. Backend engineers manage the business logic of applications and sometimes handle the storage and processing of application data. They often work on **APIs**.
- **API:** "Application Programming Interface". Think of an API as simply a set of protocols that allows communication between different applications. The term is used *a lot*, which can make it difficult to understand. Let's look at a practical example: imagine a user-facing clothing website that wants to retrieve all "shirt" items from a database securely. However, direct access to the database isn't allowed due to security reasons. In this scenario, a programmer would create an API, acting as an intermediary. Here's how the process works:
  1. The user clicks a button called "Shirts"
  2. The webite tells the API to run the "/shirts" protocol
  3. The API queries the database, selecting only items of type "shirt"
  4. The database sends the result back to the API
  5. The API sends the data to the website
  6. The user sees all items of type "shirt" on the webpage
- **IDE:** An "Integrated Development Environment" is a comprehensive software application that provides programmers with a centralized and unified environment for writing, testing, and managing code. IDEs typically include a text editor, a compiler or interpreter, debugging tools, and other features like code completion, project management, and version control integration. They are designed to streamline the software development process, making it more efficient and productive by providing a convenient and cohesive workspace for writing and maintaining code.
- **Git**: a version control system used widely in software development. It allows multiple developers to collaborate on a codebase by tracking changes to source code, facilitating teamwork, and helping manage different versions of a project. Note that Git and GitHub are two seperate entities. GitHub is basically the "social-networkification" of the Git software.
- **FOSS:** free, open-source software. Describes an application, language, framework, etc. whose source code is freely available online. Contributing to open-source codebases is a great way to gain confidence working on large projects and improving your code literacy. You can easily find open-source projects on GitHub.
- **Linux and UNIX:** UNIX describes a family of operating systems that includes many popular systems like OSX and Linux. Linux is an operating system kernel that's used for many different distributions like Ubuntu, Fedora, and Arch. You can easily install Linux yourself on a personal computer. I highly recommend doing so if you have an older laptop you're not using, but you can also configure your personal laptop to run both Windows/OSX and a Linux distribution (a.k.a. dual-booting). Ubuntu is the most beginner friendly distribution while Arch gives you the most customization.
- **low-level:** describes languages or operations that interact closely with the computer's hardware. Low-level programming often uses detailed and specific instructions that need little interpretation before being executed by the computer. Assembly is a true low-level language where the programmer is directly giving instructions to the system. Because of the proximity to the operating system, low-level languages are specific to the devices they run on and difficult to write in. This sort of tight coupling allows code to run very fast, but it opens up the program to security issues since the computer's operating system can be accessed directly.
- **highly-abstracted:** the opposite of low-level (sometimes also called high-level). Describes languages where instructions are greatly separated from the system hardware. Highly abstracted languages are easier to write in because of this separation. Since this code needs to be translated before the operating system can execute it, programs written in high-level languages are slower than their low-level counterparts. Every language listed below is a high-level language, though some may allow for low-level operations.

## Languages

It would be impossible to list every programming language here, so I've limited my list to the most popular choices. These are grouped by field (excluding the first section), so if you have no interest in the given heading feel free to skip it entirely. I don't want to recommend any resources I haven't used personally, but if I have resources to recommend they'll be listed under the language. Many of these languages can perform the same tasks, so you might be wondering how all of them have achieved such immense popularity. Most decisions on what language to use for a project come down to that language's performance, the target platform for the application, what tasks the language excels at, and simply programmer preference.

### Foundational Languages

These languages are typically used in classroom environments because they have universally applicable capabilites and provide a good understanding of the building blocks of computer science. They are also often taught because they are used so widely in the industry. I'd recommend trying out each of these languages at some point in your programming career but it's by no means necessary to be an expert in every single one (or any at all). All of these languages are united under the "C-style language" umbrella. C is language from 1972 that influenced the design of many modern languages. These languages often have a smiliar syntax to C and follow the design paradigms it established.

- **C:** powerful language still used today for it's low-level capabilities (directly manipulating memory). This makes it a perfect choice for systems programming, creating embedded programs, or any application where speed and efficiency are key. It has some inherent security vulnerabilities that make it a less popular choice these days, and it can often be tedious to code in.
  - *The C Programming Language* by Brian Kernighan and Dennis Ritchie (the creator of the language!)
  - *Programming in C* by Stephen Kochan
- **C++:** An extension of the C language that offers better security features and combines C's low-level memory manipulation with higher level abstractions for easier programming. C++ is still not a particularly easy language to write in (the creator only rated himself a 7/10 in the language), but it's capabilities are essential to millions of embedded systems. Due to its high performance, it's commonly used for game development.
  - [Learn C++ by making games with the Unreal Engine](https://docs.unrealengine.com/5.2/en-US/programming-with-cplusplus-in-unreal-engine/)
  - [Purchase the Arduino Starter Kit to get started with embedded systems](https://store-usa.arduino.cc/products/arduino-starter-kit-multi-language?selectedStore=us)
- **Java:** a widely used platform-independent language renowned for its "write once, run anywhere" capability. Java is so ubiquitous it's difficult to pin down its use cases. It can be used for almost any application and it's a great language to use for personal projects.
- **C#:** very similar to Java with some features that make the programmer experience better. Due to some initial restrictions when C# was released, it tends to be a less popular choice than Java in the industry simply due to the impact of historical precedent. However, it has just as many use cases especially in gaming with the Unity framework.

### Data Science

With the exception of Python, the following langagues are used exclusively to manipulate, analyze, and visualize large quantities of data.

- **Python:** versatile, beginner-friendly language applicable for backend development, data science, machine learning, scripting and much more. Python is used so widely in data due to its extensive libraries for data manipulation (Pandas), numerical computing (NumPy), machine learning (Scikit-learn), and data visualization (Matplotlib and Seaborn).
- **SQL**: essential for working with relational databases. It comes in a variety of flavors (MySQL and PostgreSQL being two popular choices), but if you've learned one you've learned them all.
- **R:** a language designed for statistical analysis and data visualization. R is *the* language for analyzing data, and there is always a need for R programmers in the industry.

### Web Development

Many languages can be used for website development, but these three are essential for understanding how things work on the web. As a side note, I prefer W3 schools for HTML and CSS but MDN for Javascript. Both of these resources have a wealth of information on all things web, so use them however you like.

- **HTML:** a markup language used to create the structure of a website. The standard language for documents designed to be viewed in a browser.
  - [W3Schools has the best HTML resources online](https://www.w3schools.com/html/default.asp) 
- **CSS:** a style sheet language used to describe the presentation of a document writen in a markup language like HTML. If HTML is the architect, CSS is the interior designer.
  - [W3Schools also has the best CSS resources online](https://www.w3schools.com/css/default.asp)
- **JavaScript:** allows developers to make their websites interactive. Handles actions like button clicks, fetching data from APIs, and animating items on the page. JavaScript has a large number of use-cases outside of web development, but its essential to the web.
  - [MDN is my favorite resource for all things JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
  - [React is an increasingly popular framework](https://react.dev/) (HIGHLY recommend not diving into React until you have a good grasp on JavaScript)

### Mobile App Development

These languages and frameworks are used for developing applications for iOS and Android.

- **Swift:** Apple's language for iOS and macOS development known for its modern syntax, strong safety features, and speed. To use Swift to its full capabilities, you'll need to understand advanced programming concepts like memory management and functional programming. However, you can accomplish a lot in Swift using only its high level features and it provides a good introduction to these concepts.
  - [Learn Swift from the ground up in Hacking with Swift](https://www.hackingwithswift.com/)
  - [Create beautiful applications easily with SwiftUI](https://www.hackingwithswift.com/) (I recommend having a good foundation in Swift before starting this series)
- **Java:** used for the development of Android apps. More details mentioned in the foundational section.
- **Dart:** language used by the [Flutter](https://flutter.dev/) development kit that allows developers to make cross-platform apps (same code runs on iOS and Android). Flutter can even be used to create web and desktop applications.
- **JavaScript:** can be used with [React Native](https://reactnative.dev/), another cross-platform development kit. React Native apps tend to be a little slower than native or Flutter apps, but they can be easier to create if you're already familiar with JavaScript.

### Systems and Embedded Programming

As mentioned before, C and C++ are very important languages in this field; however, I wanted to mention a new competitor that's quickly gaining popularity. 

- **Rust:** a general purpose language that focuses on safety, performance, and concurrency. Rust works seamlessly with C and C++, so it's become a popular option for developers maintaining legacy codebases who want to shift to a language with more modern features. Rust can often feel like writing in any other highly-abstracted language, but it still offers low-level capabilities like C and C++. Since it's a new, open-source language, Rust's features are constantly evolving and driven by developer feedback.
  - [The tutorial on the Rust website is incredible](https://www.rust-lang.org/learn)
