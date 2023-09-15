# Powershell

1. **PowerShell**: PowerShell is a command-line shell and scripting language developed by Microsoft for managing and automating tasks in Windows environments.

2. **Cmdlet**: Short for "commandlet," a cmdlet is a lightweight command used in PowerShell for performing specific tasks. Cmdlets are the building blocks of PowerShell scripts.

3. **Scripting Language**: PowerShell is not just a shell; it's also a scripting language. It allows users to write scripts to automate tasks and perform more complex operations.

4. **Pipeline**: The pipeline is a powerful feature of PowerShell that allows you to chain cmdlets together, passing the output of one cmdlet as the input to another, creating a flow of data and actions.

5. **Variable**: A variable in PowerShell is used to store and manage data temporarily. Variables are defined with a dollar sign ($), like `$myVariable`.

6. **Module**: A module in PowerShell is a collection of related cmdlets, functions, and scripts packaged together for easy distribution and use. Modules help organize and extend PowerShell's capabilities.

7. **Parameter**: Parameters are options or settings that you can pass to cmdlets and functions to customize their behavior. They follow the cmdlet name and are often preceded by a hyphen, like `-ParameterName`.

8. **Function**: In PowerShell, a function is a reusable block of code that performs a specific task. Functions are defined using the `function` keyword.

9. **Script Block**: A script block is a section of code enclosed in curly braces `{}`. It can be used to define functions, loops, and conditional statements in PowerShell.

10. **Alias**: An alias is a shorthand or alternate name for a cmdlet or command. PowerShell provides predefined aliases for common commands to make typing quicker.

11. **Profile**: A PowerShell profile is a script that runs automatically when you start a PowerShell session. It allows you to customize your environment with functions, aliases, and variables.

12. **ISE (Integrated Scripting Environment)**: The PowerShell ISE is an integrated development environment that provides a graphical interface for writing, testing, and debugging PowerShell scripts.

13. **Execution Policy**: PowerShell execution policies control the level of security for running scripts. There are different levels, such as "Restricted," "RemoteSigned," and "Unrestricted."

14. **Remoting**: PowerShell Remoting enables you to run PowerShell commands and scripts on remote computers, allowing for remote management and automation.

15. **Active Directory**: PowerShell is often used for managing and automating tasks related to Microsoft's Active Directory, a directory service used for user and resource management in Windows environments.

16. **Syntax**: PowerShell has a specific syntax and grammar for writing commands and scripts. Understanding PowerShell syntax is crucial for effective scripting.

17. **Get-Help**: `Get-Help` is a cmdlet used to retrieve information and documentation about other cmdlets, functions, or topics in PowerShell.

18. **Debugging**: Debugging in PowerShell involves identifying and fixing errors in scripts. Tools like `Write-Host` and the PowerShell ISE debugger help with this.

19. **Scripting Constructs**: These are essential elements of PowerShell scripts, including loops (e.g., `foreach`, `while`), conditional statements (e.g., `if`, `else`), and error handling.

20. **Providers**: PowerShell providers allow you to access different data stores like the file system, registry, and Active Directory using a unified interface.

21. **PowerShell Gallery**: The PowerShell Gallery is a repository where you can find and share PowerShell modules, scripts, and DSC resources. You can use the `Install-Module` cmdlet to download modules from the gallery.

22. **Desired State Configuration (DSC)**: DSC is a PowerShell extension for configuring and managing the state of machines. It allows you to define and enforce the desired configuration of servers and resources.

23. **Environment Variables**: PowerShell, like other command-line interfaces, supports environment variables that store system and user-specific information, such as paths, temporary directories, and user profiles.

24. **Hashtable**: A hashtable is a data structure used to store key-value pairs in PowerShell. It is often used for configuring cmdlets and functions with named parameters.

25. **Splatting**: Splatting is a technique in PowerShell where you use a hashtable to pass a collection of parameters to a cmdlet or function, making code more readable and maintainable.

26. **Error Handling**: PowerShell provides mechanisms for handling errors, including the `Try`, `Catch`, `Finally`, and `Throw` statements, to gracefully manage exceptions and unexpected issues in scripts.

27. **Script Signing**: PowerShell scripts and modules can be digitally signed to ensure their authenticity and integrity, enhancing security when running scripts.

28. **PowerShell Core**: PowerShell Core (also known as PowerShell 7 and later) is a cross-platform version of PowerShell that runs on Windows, macOS, and various Linux distributions, expanding its reach beyond Windows.

29. **.NET Integration**: PowerShell seamlessly integrates with the .NET Framework, allowing you to access and use .NET classes and libraries in your scripts.

30. **Scheduled Tasks**: PowerShell can be used to create and manage scheduled tasks and jobs on Windows systems, automating tasks to run at specified times.

31. **Event Handling**: PowerShell can respond to system events and triggers using event handling, making it useful for monitoring and automating reactions to system changes.

32. **Scripting Security**: PowerShell includes security features like constrained language mode and script block logging to help protect against malicious scripts and code execution.

33. **Web Requests**: You can use PowerShell to make HTTP requests and interact with web services, making it a versatile tool for web-related automation tasks.

34. **Windows Management Instrumentation (WMI)**: PowerShell provides cmdlets for querying and managing WMI information, which is used for system administration and monitoring.

35. **Jupyter Notebooks**: PowerShell can be used within Jupyter notebooks, allowing for interactive and documented scripting in a notebook-style environment.

36. **Background Jobs**: PowerShell supports background jobs, allowing you to run tasks in the background without blocking the console.

37. **Package Management**: PowerShell includes cmdlets like `Install-Package` for managing software packages, making it useful for software installation and management.

38. **Object-Oriented**: PowerShell treats data as objects, making it easy to manipulate and work with structured data, such as JSON and XML.

39. **Azure PowerShell**: There is a specific module for managing Microsoft Azure resources using PowerShell, which is essential for cloud-based automation.

40. **Community Support**: PowerShell has a vibrant and active community of users and contributors who share scripts, modules, and knowledge, making it easier to learn and solve problems.

## Powershell Commands

1. **Get-Help**: Retrieve information and documentation about other cmdlets, functions, or topics in PowerShell. Usage: `Get-Help cmdletName`.

2. **Get-Command**: List all available cmdlets and functions in your PowerShell session.

3. **Get-Module**: List loaded modules or import a specific module for additional functionality.

4. **Get-Item**: Retrieve information about files, folders, registry keys, or other items. Usage: `Get-Item path`.

5. **Get-Process**: List running processes on your system.

6. **Get-Service**: List all services on your computer and their status.

7. **Get-EventLog**: Retrieve entries from event logs on your system.

8. **Get-Content**: Read and display the content of a file. Usage: `Get-Content filePath`.

9. **Set-Content**: Write content to a file. Usage: `Set-Content filePath -Value "Content"`.

10. **New-Item**: Create a new file, folder, or registry key. Usage: `New-Item path`.

11. **Remove-Item**: Delete a file, folder, or registry key. Usage: `Remove-Item path`.

12. **Copy-Item**: Copy a file or folder from one location to another. Usage: `Copy-Item sourcePath -Destination destinationPath`.

13. **Move-Item**: Move a file or folder from one location to another. Usage: `Move-Item sourcePath -Destination destinationPath`.

14. **Rename-Item**: Rename a file or folder. Usage: `Rename-Item path -NewName newName`.

15. **Test-Path**: Check if a file, folder, or registry key exists. Usage: `Test-Path path`.

16. **Start-Process**: Start a new process (application) from PowerShell. Usage: `Start-Process -FilePath "executablePath"`.

17. **Stop-Process**: Terminate a running process. Usage: `Stop-Process -Name processName`.

18. **New-Object**: Create a new instance of a .NET object. Usage: `New-Object TypeName`.

19. **Get-Variable**: List all variables in the current session.

20. **Set-Variable**: Set the value of a variable. Usage: `Set-Variable -Name variableName -Value "NewValue"`.

21. **Clear-Variable**: Remove the value from a variable. Usage: `Clear-Variable variableName`.

22. **Write-Host**: Display output directly to the console. Usage: `Write-Host "Message"`.

23. **Write-Output**: Send output to the pipeline (used within scripts and functions).

24. **ForEach-Object**: Iterate through a collection and perform actions on each item. Usage: `ForEach-Object { code block }`.

25. **Where-Object**: Filter objects in the pipeline based on a condition. Usage: `Where-Object { $_.Property -eq "Value" }`.

26. **Sort-Object**: Sort objects in the pipeline based on specified properties.

27. **Group-Object**: Group objects in the pipeline based on specified properties.

28. **Select-Object**: Select specific properties of objects in the pipeline. Usage: `Select-Object Property1, Property2`.

29. **Measure-Object**: Calculate statistics on objects in the pipeline, such as count, sum, or average.

30. **New-Alias**: Create a new alias for a cmdlet or function. Usage: `New-Alias -Name AliasName -Value cmdletName`.
