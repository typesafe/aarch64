# Windows AARCH64 Tutorial

A set of projects to learn aarch64 (ARM64) assembly language for _Windows_.  

While there is some information out there of how to develop for ARM Assembly on Linux, there is virtually nothing available for ARM assembly for Windows.  Granted, it is far from popular and we should all be developing in higher
languages like C, C++ or C# anyway; but its always nice to learn what is going on under the hood.

So it took it upon me to create a series of project that explain aarch64 (aka arm64) assembly language for Windows.
While I have over 20 year of experience in programming, I have never been a low-level developer.  This tutorial is really "on eye leading the blind", so if you spot any mistakes, please feel free to comment or reach out to me in any other way.

I'm planning to make a YouTube series on this, but until then you will have to do with these projects.

Projects so far:

0. **Sum**: Setup of the environment, including debugging and a leaf functions
1. **HelloWorld**: constants, initialized global data, temp registers and unchained functions
2. **MeaningOfLife**: register aliases, uninitialized global data, saved registers and chained functions (WIP)
3. **ArgEcho**: local allocated data and loops (WIP)
4. ...

## Prerequisites

* __Dev PC__: an x64 Windows PC with sufficient disk free
* __Target PC__: Windows PC running on aarch64 (aka ARM64)

See Lesson 0 for how te set it up.

Personally I'm using a first generation Microsoft Surface Pro X as my target PC, but you could use other types of Windows device if you prefer.

## References

This series is made as a tutorial, meaning you learn by example.  It isn't a manual nor a course that will explain aarch64 step by step, instead it are a series of examples that will allow you to figure it out by yourself.  Here are a set link that I found useful in my journey to learn it in the first place:

### developer.arm.com (official)

The following references are provided by ARM inc itself:

* Programmers guide: https://developer.arm.com/documentation/102374/latest/
* ARMASM* reference guide: https://developer.arm.com/documentation/dui0802/b/A64-General-Instructions/A64-general-instructions-in-alphabetical-order
* Instruction reference guide: https://developer.arm.com/documentation/ddi0602/latest

*) While we use clang instead of asm, the armasm reference guide has nice a summary of instructions while the armclang reference guide doesn't.

### Other sources

* Presentation of Matteo Franchin (ARM): https://armkeil.blob.core.windows.net/developer/Files/pdf/graphics-and-multimedia/ARMv8_InstructionSetOverview.pdf
* Microsoft's explanation for C++ project: https://docs.microsoft.com/en-us/cpp/build/configuring-programs-for-arm-processors-visual-cpp?view=msvc-170
* modexp blog post: https://modexp.wordpress.com/2018/10/30/arm64-assembly/
