# Student Guide to Software Development

### Welcome to Software Development!

In today’s fast-paced world, software development is about more than just writing code; it’s about creating systems that are reliable, scalable, and maintainable. If you’re beginning your journey into software development, you’re in the right place. This guide will walk you through key concepts that are essential in modern development workflows, from managing code versions to deploying applications in a cloud-native environment.

Let's start from the beginning.

## The Lifeblood of Collaboration: Version Control Systems

Imagine you’re working on a project with multiple developers. You each make changes to the code, and suddenly, you find yourselves stepping on each other’s toes. Without a system to manage these changes, chaos would ensue.

This is where **Version Control Systems (VCS)** like **Git** come into play. Version control allows you to track changes, work on different features in parallel, and collaborate smoothly with your team. Whether you're contributing to open source or managing a personal project, Git enables you to save your work, experiment without fear, and always have a history of every change made.

[Learn more about Version Control](https://github.com/cr432/is373guide/blob/development/VersionControl.md)

As you continue to grow as a developer, you’ll see that managing code versions is only the first step toward creating a maintainable workflow. Next, we’ll dive into how to streamline development and deployment with automated pipelines.

## Automating Success: CI/CD Pipelines

Once your team is working in harmony using version control, the next challenge is ensuring that your software is always in a working state, even as changes are made frequently. This is where **Continuous Integration (CI)** and **Continuous Deployment (CD)** come into play.

With CI/CD pipelines, each time you push code to a repository, automated tests are run to ensure that everything works as expected. If the tests pass, the new code is automatically deployed to a production environment. This reduces the time spent on manual testing and deployment, giving developers more time to focus on what they do best: writing code.

[Learn more about CI/CD](https://github.com/cr432/is373guide/blob/development/CICD.md)

As your code moves through the pipeline and your systems become more complex, you’ll likely encounter another important tool for development: Linux.

## Linux: The Developer's Best Friend

Linux is everywhere—on servers, in containers, even on your local development environment. Why is Linux so popular among developers? Because it’s flexible, powerful, and open-source. Whether you're setting up a server, writing scripts, or troubleshooting networking issues, **Linux** gives you full control over your environment.

If you’re working in a cloud environment or with containerized applications, knowing Linux will be crucial. It’s the foundation upon which so many modern development environments are built.

[Learn more about Linux](https://github.com/cr432/is373guide/blob/development/Linux.md)

But what if you want to run multiple operating systems without buying multiple machines? That brings us to virtualization.

## The Magic of Virtualization

Picture this: You’re developing an application that needs to run on different operating systems. Rather than setting up several physical machines, you can use **virtualization** to create multiple virtual environments on a single machine. 

With tools like **VirtualBox** and **VMware**, virtualization allows you to run different operating systems side-by-side. It’s a vital tool for testing, development, and even security research. In a way, virtualization is like creating small, self-contained universes that each serve a specific purpose.

[Learn more about Virtualization](https://github.com/cr432/is373guide/blob/development/virtualization.md)

And if you're a Windows user, you might be interested in an even simpler way to get the power of Linux on your machine through **Windows Subsystem for Linux (WSL2)**.

[Learn more about WSL2](https://github.com/cr432/is373guide/blob/development/WSL2.md)

## From Virtualization to Containerization: A New Era of Development

As you dive deeper into the development world, you’ll encounter **containers**—lightweight, self-contained environments that hold your application and all of its dependencies. Unlike virtual machines, containers don’t need a full operating system to run, which makes them faster and more efficient.

[Learn more about Containerization](https://github.com/cr432/is373guide/blob/development/containerization.md)

**Docker**, the most popular containerization tool, allows developers to package applications into containers that can run anywhere—whether it's on your local machine, in the cloud, or on a server halfway across the world. Containers are the backbone of modern software deployment, and learning how to use them will significantly level up your development skills.

[Learn more about Docker Commands](https://github.com/cr432/is373guide/blob/development/dockercommands.md)

Once you've mastered Docker, you might want to explore **Kubernetes**, which helps you manage clusters of containers at scale.

[Learn more about Docker vs Kubernetes](https://github.com/cr432/is373guide/blob/development/dockervskubernetes.md)

And if you're curious about the history behind this revolutionary technology:

[A Brief History of Docker](https://github.com/cr432/is373guide/blob/development/historyofdocker.md)

## The Kernel: The Heart of the Operating System

While containers and virtual machines give you isolated environments, it’s the **kernel** that makes the magic happen. The kernel is the core part of an operating system, responsible for managing resources, handling processes, and enabling communication between software and hardware.

Understanding the kernel is key to mastering how an operating system works under the hood. Whether you're developing low-level software, troubleshooting performance issues, or simply curious about how your system allocates resources, learning about the kernel will broaden your understanding of operating systems.

[Learn more about Kernels](https://github.com/cr432/is373guide/blob/development/kernel.md)

## Building Scalable, Maintainable Apps: The Twelve-Factor App Methodology

As your applications grow, they become harder to manage. That’s why the **Twelve-Factor App** methodology was created—to guide developers in building apps that are scalable, maintainable, and ready for the cloud. It’s a set of principles that emphasize simplicity, configuration management, and a clean separation of concerns.

Mastering these principles will help you design software that can evolve with changing needs, handle growing traffic, and remain stable as your development team scales.

[Learn more about the Twelve-Factor App](https://github.com/cr432/is373guide/blob/development/TwelveFactorApp.md)

## Monitoring and Debugging: The Importance of Logging

As a developer, you’ll often find yourself asking, “What went wrong?” This is where **logging** comes in. Logging allows you to track the behavior of your application in real time. By analyzing logs, you can diagnose problems, monitor performance, and ensure that your software is running as expected.

Good logging practices are critical, especially when your application is running in production, and understanding how to implement and manage logs is a skill that will save you countless hours of debugging.

[Learn more about Logging](https://github.com/cr432/is373guide/blob/development/Logging.md)

## Conclusion: The Journey Ahead

The world of software development is vast, and this guide is just the beginning. As you explore topics like **version control**, **CI/CD**, **Linux**, **virtualization**, **containerization**, and the **Twelve-Factor App**, you'll be laying the groundwork for a successful career in development. Take your time, dive deep into each section, and enjoy the journey!