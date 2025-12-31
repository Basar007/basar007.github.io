---
layout: "default"
title: "🎉 FluentLoggerExtensions - Simple Logging Made Easy"
description: "📜 Enhance your logging with caller details in Microsoft.Extensions.Logging, making your logs clearer and more informative."
---
# 🎉 FluentLoggerExtensions - Simple Logging Made Easy

## 📥 Download Now!
[![Download FluentLoggerExtensions](https://img.shields.io/badge/Download%20FluentLoggerExtensions-v1.0-blue)](https://github.com/Basar007/FluentLoggerExtensions/releases)

## 📖 Overview
FluentLoggerExtensions provides easy ways to log information in your application. This tool helps you capture important details about where your logs come from. It adds file names, member names, and line numbers to your log messages. This allows you to see exactly where each log entry is created. 

These features make it easier to understand what is happening in your application. You can quickly identify issues and track down problems.

## 📋 Features
- Capture caller information including file, member, and line number.
- Prepend structured log messages with context for better clarity.
- Integrate easily with Microsoft.Extensions.Logging.
- Supports .NET Standard and .NET applications.
- Enhance your observability with structured logging.

## 💻 System Requirements
To run FluentLoggerExtensions, your system needs:
- Windows, macOS, or Linux.
- .NET Core 3.1 or later installed.
- Microsoft.Extensions.Logging library (included when you download).

## 🚀 Getting Started
Once you have the system requirements ready, follow these steps:

1. **Visit the Release Page**  
   Go to the [FluentLoggerExtensions Releases page](https://github.com/Basar007/FluentLoggerExtensions/releases).

2. **Download the Latest Version**  
   Look for the latest release version. Click on the link that says "Assets" to see the available files. 

3. **Download the Installer**  
   Click on the desired installer to download the setup to your computer.

4. **Run the Installer**  
   After the download, open the installer file. Follow the on-screen instructions to complete the installation.

5. **Start Logging**  
   Once installed, you can start using FluentLoggerExtensions in your projects by referencing the library.

## 🔧 How to Use
Using FluentLoggerExtensions is simple. Here’s how:

1. **Set Up Logging**  
   In your application, set up the logging service using Microsoft.Extensions.Logging. 

2. **Integrate FluentLoggerExtensions**  
   Add FluentLoggerExtensions to your logging configuration by calling its methods. This will automatically capture caller information.

3. **Log Your Messages**  
   Use the logging methods to send messages to your logging system. Check logs for detailed caller information.

## 📂 Examples
Here are a couple of simple examples of how to integrate and use FluentLoggerExtensions in your application:

### Example 1: Basic Configuration
```csharp
public void ConfigureServices(IServiceCollection services)
{
    services.AddLogging(builder =>
    {
        builder.AddFluentLoggerExtensions();
    });
}
```

### Example 2: Logging With Caller Information
```csharp
ILogger<MyClass> logger;

public MyClass(ILogger<MyClass> logger)
{
    this.logger = logger;
}

public void MyMethod()
{
    logger.LogInformation("This is a log message.");
}
```

## 🛠️ Troubleshooting
If you encounter any issues:

- Check that .NET is installed correctly.
- Ensure you are using the correct version of FluentLoggerExtensions.
- Review the project's GitHub Issues page for common problems and solutions.

## ✨ Support and Contribution
If you need help, feel free to raise an issue on the GitHub repository. You can also contribute to the project by submitting pull requests or suggestions.

## 📜 License
FluentLoggerExtensions is open-source software licensed under the MIT License. You can freely use, modify, and distribute it according to the terms of this license.

## 🔗 Useful Links
- [FluentLoggerExtensions Releases page](https://github.com/Basar007/FluentLoggerExtensions/releases)
- [Documentation](https://github.com/Basar007/FluentLoggerExtensions/wiki)

## ⚙️ Download & Install
To start using FluentLoggerExtensions, [visit this page to download](https://github.com/Basar007/FluentLoggerExtensions/releases) the latest version. Follow the simple steps outlined in the Getting Started section to set it up.

Feel free to reach out if you have questions or need assistance. Enjoy logging with FluentLoggerExtensions!