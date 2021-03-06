## History

In 2006, Sergi Àlvarez (aka pancake), was working as a forensic analyst. As long as he wasn't allowed to use private software for his personal needs, he decided to write a small tool, an hexadecimal editor with very basic characteristics:

* be extremely portable (unix friendly, command line, c, small)
* open disk devices, this is using 64bit offsets
* search for a string or hexpair
* review and dump the results to disk

It was designed to recover a deleted file from an HFS+ partition.

After that, pancake decided to extend the tool to have a pluggable io to be able to attach to processes, implemented the debugger functionalities, support for multiple archs and code analysis.

The project has evolved to provide a complete framework for analyzing binaries while making use of basic UNIX concepts. Those concepts include the famous "everything is a file", "small programs that interact using stdin/stdout", and "keep it simple" paradigms.

But then the need for scripting showed up the fragility of the initial monolithic design of the tool. Making it hard to use the api. A refactoring was needed, in 2009, radare was forked into radare2, a complete refactor of radare1, in a more flexible and dynamic way, enabling a much better integration for using r2 from different programming languages.

It's been a one man project, with some eventual contributions, to a big community project around 2014. The number of users was growing fast, and the author, and main developer had to switch the role from coder to manager, in order to manage the different developers that join the project.

Instructing the users to report their issues allows us to define the new directions of the project in order to evolve. Everything is managed in the [radare2 GitHub](https://github.com/radare/radare2) and discussed in the Telegram channel.

The project remains active at the moment of writing this book, and there are several side projects that provide a graphical user interface (Cutter), a decompiler (r2dec, radeco), Frida integration (r2frida), Yara, Unicorn, Keystone, and many other projects indexed in the r2pm (the radare2 package manager).
