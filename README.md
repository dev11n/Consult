# Consult
## What is it?
Consult is a stripped down memory library which aims to just provide the most basic of features, and a bit more.
## What's different from other libraries?
- Less bloat code
- It's easy to understand (well, unless you are skid)
- Straight forward
- Commented unlike most others
## Credits
- erfg12 from Memory.dll : `get_real_address` & `cache_modules` functions in `Utils`
- Guided Hacking : Great place for learning game cheating
## Usage
**Please keep in mind that this library was made with .NET 5.0 and C# 9.0, so it may or may not work in your project!**
***
First download the DLL (`~/bin/Debug/net5.0/Consult.dll`) and then reference it in your project

Then open whatever process you want using this code snippet:
```csharp
private Consult consult = new();

private static void main()
{
   if (!consult.open_process(Process.GetProcessesByName("whatever").FirstOrDefault()) return;
   // Open!
}
```
After that, you can access `consult.Memory.*` to find several functions you can use. All of them are straight forward for anyone that isn't a goldfish.
