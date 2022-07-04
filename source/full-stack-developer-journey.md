# Full Stack Developer Journey

## 80/20 Rule

The [Pareto Principle](https://en.wikipedia.org/wiki/Pareto_principle) states that we can attribute 80% of all results to 20% of all possibilities.

Software Development is no different.

The problem is figuring out what that 20% is.

## How this talk is Structured

Everything in this talk is "personal opinion", please don't take it as an absolute.

> Pirate Code - They're more like guidelines

Lists are in order:

:blue_heart: - Computer Science concept
:green_heart: - Language Paradigm
:yellow_heart: - Pattern
:heart: - Library/Framework
:black_heart: - Key Concept

Think of the topics given to you today as a 1, 3, 5, 10 year plan. Don't get overwhelmed.

## Knowing vs Knowing

When have I reached the point when I am competent in a subject/topic?

When you can explain/teach it to someone else without outside help.

## 10 Commandments for any Developer

1. Keep learning
2. Keep re-learning, you will forget
3. [Get .1% better every day](https://en.wikipedia.org/wiki/Compound_interest)
4. Use the 80/20 rule for everything
5. Frameworks come and go, concepts are forever
6. Put everything on GitHub
7. Coding is easy, engineering is hard
8. Making testing a first-class citizen :black_heart:
9. Find a mentor and become a mentor to someone else
10. Your job isn't to code, its to provide a (customer) service

## Everything is both related and separate

Gaining knowledge in one area/concept will further your knowledge in another.

Getting better at OOP will help your functional skills and visa versa.

## Why should I care about CS?

Computer Science is the foundation for everything we do.

It may only apply to 1% of what we do, but that 1% is important.

### What if I don't have a CS degree?

Concepts that go the distance:

You don't need to memorize is, just be comfortable with the conceptual knowledge.

[Base 2/Binary](https://en.wikipedia.org/wiki/Binary_number) - Why does an int only go to ~2 million?

[Base 10/Decimal](https://en.wikipedia.org/wiki/Decimal) - Why do I need a separate type to represent money?

[Base 16/Hexadecimal](https://en.wikipedia.org/wiki/Hexadecimal) - Why are these CSS color codes?

[MS/Unix File Systems](https://en.wikipedia.org/wiki/File_system) - Imports, paths, a lot of command prompts

[Memory Management](https://en.wikipedia.org/wiki/Memory_management) - Creation and scope

[Stack vs Heap](https://www.linux.com/training-tutorials/stack-vs-heap-whats-difference-and-why-should-i-care/) - Memory, Value vs Ref

[Pointers, Objects & Functions](<https://en.wikipedia.org/wiki/Pointer_(computer_programming)>) - What causes half my exceptions?

[Boolean Logic](https://en.wikipedia.org/wiki/Boolean_algebra) - Comparisons

[Time Complexity](https://en.wikipedia.org/wiki/Time_complexity) - Why does my 10x for loop take so long?

[Finite State Machine](https://en.wikipedia.org/wiki/Finite-state_machine) - Logic Flow, Asynchronous

[Basic Data Structures](https://en.wikipedia.org/wiki/Data_structure) - Stack vs Queue vs Array vs Vector?

#### Don't memorize algorithms or data structures, and if any job interviewer ask you to create a linked-list or stack by hand you don't want that job

## Environment & Tooling

- Know your IDE inside and out, Visual Studio/IntelliJ/VSCode
- Know all the [important keywords/shortcuts](https://docs.microsoft.com/en-us/visualstudio/ide/default-keyboard-shortcuts-in-visual-studio?view=vs-2022)
- [Code Snippets](https://docs.microsoft.com/en-us/visualstudio/ide/visual-csharp-code-snippets?view=vs-2022) (I.E. ctor + tab = constructor)
- [ReSharper](https://www.jetbrains.com/resharper/)
- [VSCode Plugins](https://marketplace.visualstudio.com/VSCode)

### .NET

- [Solution Files](https://docs.microsoft.com/en-us/visualstudio/extensibility/internals/solutions-overview?view=vs-2022)
- Know the [project types](https://docs.microsoft.com/en-us/visualstudio/extensibility/internals/project-types?view=vs-2022) (I.E. Test/Web Projects are really fancy console apps)
- [csproj file](https://docs.microsoft.com/en-us/aspnet/web-forms/overview/deployment/web-deployment-in-the-enterprise/understanding-the-project-file)
- [Directory.Build.Props](https://docs.microsoft.com/en-us/visualstudio/msbuild/customize-your-build?view=vs-2022#:~:text=Directory.Build.props%20is%20a%20user-defined%20file%20that,provides%20customizations%20to%20projects%20under%20a%20directory.)
- [NuGet](https://docs.microsoft.com/en-us/dotnet/standard/library-guidance/nuget) - Understand how dependencies are resolved and how to fix common issues

### Java

<!-- To Add -->

### Linters & Formatters

#### Back-End Based

- [.NET Analyzers](https://docs.microsoft.com/en-us/dotnet/fundamentals/code-analysis/overview)
- [Style Cop Analyzers](https://github.com/DotNetAnalyzers/StyleCopAnalyzers)

#### Front-End

- [Prettier](https://prettier.io/)
- [ESLint](https://eslint.org/) - [Awesome ESLint Plugin List](https://github.com/dustinspecker/awesome-eslint)

### Testing :black_heart:

- Want to be a better developer overnight? Put (automated) testing first.
- Favor branch coverage
- 100% test coverage is a false sense of security
- You can't automate 100%
- Every logical branch requires a test :black_heart:
- Focus on Unit/Integration tests
  
#### .NET Testing

- Choose one of the following [MSTest](https://docs.microsoft.com/en-us/dotnet/core/testing/unit-testing-with-mstest) or [NUnit](https://nunit.org/) or [XUnit](https://xunit.net/)
- [Moq](https://github.com/moq/moq4) for Mocking
- **DO NOT** use the [in-memory db](https://docs.microsoft.com/en-us/ef/core/providers/in-memory/?tabs=dotnet-core-cli) for integration testing
- You **CAN NOT** mock the [DBContext](https://docs.microsoft.com/en-us/dotnet/api/system.data.entity.dbcontext?view=entity-framework-6.2.0) class in EF, so don't try

#### Front-End Testing

- [Jest](https://jestjs.io/) or [Vitest for Vite](https://vitest.dev/) - Test Framework
- [TestingLibrary](https://testing-library.com/) - Core Testing Utilities for React, Vue, Angular
- [JestDom](https://testing-library.com/docs/ecosystem-jest-dom/) - Custom DOM Matchers
- [UserEvent](https://testing-library.com/docs/user-event/intro) - User Interactions
- [Cypress](https://www.cypress.io/) - Integration, E2E, Links, Mobile Views

## Functional Programming

- [Methods](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/methods) :blue_heart:
- [Overloading](https://docs.microsoft.com/en-us/cpp/cpp/function-overloading?view=msvc-170) :blue_heart:
- [Delegates](https://docs.microsoft.com/en-us/dotnet/csharp/delegates-overview) :blue_heart:
- [Default/Optional Arguments](https://docs.microsoft.com/en-us/cpp/cpp/default-arguments?view=msvc-170) :green_heart:
- [Callbacks](<https://en.wikipedia.org/wiki/Callback_(computer_programming)>) :black_heart:
- [Anonymous Functions/Closure](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/delegates/delegates-with-named-vs-anonymous-methods) :green_heart:
- [Lambda Expressions](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/operators/lambda-expressions) :green_heart:
- [Extension Methods](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/extension-methods) :green_heart: - [Static](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/static) is a pre-requisite
- [Generic Delegates](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/generics/generic-delegates) :yellow_heart: - [Generics](https://docs.microsoft.com/en-us/dotnet/csharp/fundamentals/types/generics) are a pre-requisite
- [Pure Functions](https://en.wikipedia.org/wiki/Pure_function) :yellow_heart:
- [Higher-Order Functions](https://en.wikipedia.org/wiki/Higher-order_function) :yellow_heart:
- [First Class Functions](https://en.wikipedia.org/wiki/First-class_function) :yellow_heart:
- [Events](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/events/) :yellow_heart:
- [LINQ/Streams](https://docs.microsoft.com/en-us/dotnet/csharp/linq/) :heart:
- [RxJS](https://rxjs.dev/) :heart:
- [Angular](https://angular.io/) :heart: - RxJS is a hard pre-requisite
- [React](https://reactjs.org/) :heart:
- [Vue](https://vuejs.org/) :heart:
- [Azure Function Apps](https://docs.microsoft.com/en-us/azure/azure-functions/functions-overview) :heart:

### Functional Litmus Test

- I understand when to use functions vs non-functions (I.E. Don't turn everything into a LINQ/Stream expression)
- I understand how basic functional concepts translate into real implementations

### 80/20 Rule of Functions

- Callbacks, Callbacks, Callbacks

## OO Programming

- [Encapsulation](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming)) :blue_heart:
- [Inheritance](https://en.wikipedia.org/wiki/Inheritance_(object-oriented_programming)) :blue_heart:
- [Abstraction](https://en.wikipedia.org/wiki/Abstraction_(computer_science)) :blue_heart:
- [Polymorphism](https://en.wikipedia.org/wiki/Polymorphism_(computer_science)) :black_heart:
- [Access Modifiers](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/access-modifiers) :green_heart:
- [Interfaces](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/interface) :green_heart:
- [Abstract & Sealed](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/classes-and-structs/abstract-and-sealed-classes-and-class-members) :green_heart:
- [Generics](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/generics/generic-classes) :green_heart:
- [Constraints](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/generics/constraints-on-type-parameters) :green_heart:
- [Fluent Interfaces](https://en.wikipedia.org/wiki/Fluent_interface) :yellow_heart:
- [Gof Patterns](https://en.wikipedia.org/wiki/Design_Patterns) :yellow_heart:

### OO Litmus Test

- I understand Abstraction, Inheritance, Encapsulation, and Polymorphism and how they relate to each other
- When and how to abstract, virtual, new, override, readonly, const, and sealed
- I understand how OO concepts are enhanced by generics and constraints
- I know when to use a class vs when to use a function

### 80/20 Rule of OOP

- Polymorphism, polymorphism, polymorphism

## Honorable Mention - Static

- Understand what the [static](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/static) keyword does
- Know when, where, why to use it
- Scoped to object level, not instance level :black_heart:

## Data-Access

- [SQL](https://en.wikipedia.org/wiki/SQL) :blue_heart: - “Never memorize what you can look up in books” (The sames goes for RegEx)
- [ODBC](https://en.wikipedia.org/wiki/Open_Database_Connectivity) :blue_heart: - Just know the history/usage

### .NET Data Access

- [SSMS](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-ver16) - SQL IDE
- [SQL Server Profiler](https://docs.microsoft.com/en-us/sql/tools/sql-server-profiler/sql-server-profiler?view=sql-server-ver16) - SQL Server Tracer

- [LINQ to SQL](https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/sql/linq/) **is depreciated**
- [OLE DB](https://en.wikipedia.org/wiki/OLE_DB) - :green_heart: - Again just read and understand
- [ADO.NET](https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/) :heart:
- [Dapper](https://github.com/DapperLib/Dapper) :heart:
- [Entity Framework](https://docs.microsoft.com/en-us/aspnet/entity-framework) :heart:

### Java Data Access



## Patterns

### Common Pitfalls

- Patterns are not silver bullets
- Every nail do not require a hammer
- No such thing as an anti-pattern, they're all situational
- Most patterns are just polymorphism or callbacks on crack cocaine :black_heart:
- A lot of libraries/frameworks exist to do the work for you
- Patterns play nicely with each other (I.E. Command/Mediator/Observer)
- Lots of overlap, copy-pasta, and redundancy (I.E. Repository == Facade == Interface)
- [Large Compendium](https://www.martinfowler.com/articles/enterprisePatterns.html)

General Order:

1. [Gang of Four](https://en.wikipedia.org/wiki/Design_Patterns)
2. [Enterprise Application](https://www.martinfowler.com/eaaCatalog/)
3. [Domain Driven Design](https://docs.microsoft.com/en-us/archive/msdn-magazine/2009/february/best-practice-an-introduction-to-domain-driven-design)
4. [Enterprise Integration](https://www.enterpriseintegrationpatterns.com/)

#### Gof

##### Creational

###### Your [DI Framework](https://docs.microsoft.com/en-us/dotnet/core/extensions/dependency-injection) does the heavy lifting

- [Factory](https://en.wikipedia.org/wiki/Factory_method_pattern)
- [Builder](https://en.wikipedia.org/wiki/Builder_pattern)

##### Structural

- [Bridge](https://en.wikipedia.org/wiki/Bridge_pattern) - [AutoMapper](https://automapper.org/)
- [Decorator](https://en.wikipedia.org/wiki/Decorator_pattern) - [Attributes](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/attributes/)
- [Facade](https://en.wikipedia.org/wiki/Facade_pattern) - Very abstract in nature
- [Proxy](https://en.wikipedia.org/wiki/Proxy_pattern) - [Moq](https://github.com/moq/moq)

##### Behavioral

- [Chain of Responsibility](https://en.wikipedia.org/wiki/Chain-of-responsibility_pattern)
- [Command](https://en.wikipedia.org/wiki/Command_pattern) - [HTTP Request Body](https://developer.mozilla.org/en-US/docs/Web/API/Request/body) :black_heart:
- [Mediator](https://en.wikipedia.org/wiki/Mediator_pattern) - [MediatR](https://github.com/jbogard/MediatR)
- [Observer](https://en.wikipedia.org/wiki/Observer_pattern) - [MediatR](https://github.com/jbogard/MediatR)
- [State](https://en.wikipedia.org/wiki/State_pattern) - [Async](https://docs.microsoft.com/en-us/dotnet/csharp/async)
- [Strategy](https://en.wikipedia.org/wiki/Strategy_pattern) - [Switch](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/statements/selection-statements#the-switch-statement)

#### Domain Driven Design

- DDD is just a bunch of patterns bundled together
- Most DDD patterns are just a fancier, crank cocain-ier versions of their Gof/Enterprise counterparts (I.E. What if I could make a object into a value type)
- DDD is the OG micro-services **don't touch micro-services until you know DDD inside and out**
- Purpose of DDD is to distill a complex domain into easy to understand concepts
- DDD is **not easy**, don't get frustrated
- DDD is not zero-sum, or mutually exclusive
- You don't have to use everything in DDD, its a buffet lunch
- DDD does not imply Micro-services, Docker, Kubernetes, EventSourcing, CQRS, and the same goes for most of those topics
- Bound Contexts (Sales vs Marketing vs Inventory) :black_heart:

## Recommended Books

### Pattern Based

- [A Pattern Language](https://www.amazon.com/Pattern-Language-Buildings-Construction-Environmental/dp/0195019199/ref=sr_1_1?keywords=a+pattern+language+christopher+alexander&qid=1656870154&s=books&sprefix=a+patt%2Cstripbooks%2C103&sr=1-1) - Building Architecture (Optional)
- [Design Patterns](https://www.amazon.com/Design-Patterns-Elements-Reusable-Object-Oriented/dp/0201633612/ref=sr_1_1?crid=3LZ431GEDF332&keywords=design+patterns+elements+of+reusable+object-oriented+software&qid=1656870103&s=books&sprefix=design+patterns%2Cstripbooks%2C87&sr=1-1)

### CSharp

- [C# In Depth](https://www.amazon.com/C-Depth-Jon-Skeet/dp/1617294535/ref=sr_1_1?crid=RJ2G41D5Y9Y9&keywords=c+in+depth&qid=1656870028&sprefix=c%23+in+depth%2Caps%2C192&sr=8-1)
- [Adaptive Code via C#](https://www.amazon.com/Adaptive-Code-Developer-Best-Practices-dp-0136891446/dp/0136891446/ref=dp_ob_title_bk)

### DDD Books

- [Original Blue Book](https://www.amazon.com/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215/ref=sr_1_6?crid=1YCV48H6KQOR5&keywords=ddd&qid=1656870336&s=books&sprefix=ddd%2Cstripbooks%2C99&sr=1-6) - Original DDD book, I can't give you my opinion on it
- [Other DDD Book](https://www.amazon.com/Patterns-Principles-Practices-Domain-Driven-Design/dp/1118714709/ref=sr_1_6?keywords=domain+driven+design&qid=1656870402&s=books&sprefix=domain+dri%2Cstripbooks%2C82&sr=1-6)

### Architecture

- [Clean Architecture](https://www.amazon.com/Clean-Architecture-Craftsmans-Software-Structure/dp/0134494164/ref=pd_bxgy_img_sccl_1/146-6357958-3857264?pd_rd_w=RwhPI&content-id=amzn1.sym.7757a8b5-874e-4a67-9d85-54ed32f01737&pf_rd_p=7757a8b5-874e-4a67-9d85-54ed32f01737&pf_rd_r=VX8R66M5WF7NTFFEMW3Z&pd_rd_wg=slM2J&pd_rd_r=bcd73204-76bb-4629-ae6a-2673b4c2b16f&pd_rd_i=0134494164&psc=1) - Or just [watch the video](https://www.youtube.com/watch?v=WpkDN78P884)

### Free E-Books

- [.NET Compendium](https://dotnet.microsoft.com/en-us/learn/aspnet/microservices-architecture)
- [.NET Micro-services](https://raw.githubusercontent.com/dotnet-architecture/eBooks/main/current/microservices/NET-Microservices-Architecture-for-Containerized-NET-Applications.pdf)
- [Cloud Native .NET App](https://raw.githubusercontent.com/dotnet-architecture/eBooks/main/current/cloud-native/Architecting-Cloud-Native-NET-Apps-for-Azure.pdf)
- [Dapr for .NET](https://raw.githubusercontent.com/dotnet-architecture/eBooks/main/current/dapr-for-net-developers/Dapr-for-NET-Developers.pdf)
- [.NET Docker App](https://raw.githubusercontent.com/dotnet-architecture/eBooks/main/current/containerized-lifecycle/Containerized-Docker-Application-Lifecycle-with-Microsoft-Platform-and-Tools.pdf)
- [Azure Quick Start](https://raw.githubusercontent.com/dotnet-architecture/eBooks/main/current/azure-quick-start/Azure-Quick-Start-for-NET-Developers.pdf)
- [Modernize Existing Apps](https://raw.githubusercontent.com/dotnet-architecture/eBooks/main/current/modernize-with-azure-containers/Modernize-Existing-.NET-applications-with-Azure-cloud-and-Windows-Containers.pdf)