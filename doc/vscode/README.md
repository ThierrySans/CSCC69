---
layout: default
permalink: /doc/vscode/
---

# Debug Pintos in VS Code (by Darren Liu)

Basically `dpin` starts Pintos and expose the port `1234` so it can be accessible at `localhost:1234` on the host machine. Since it is accessible, we can now hook up VS Code's debugger (or any other debugger)

## Installation
1. Install this:
```
Name: C/C++
Id: ms-vscode.cpptools
Description: C/C++ IntelliSense, debugging, and code browsing.
Version: 1.0.1
Publisher: Microsoft
VS Marketplace Link: https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools
```
2. Make a symlink from your source code and `/pintos` by doing `sudo ln -s $PINTOS_PATH /`
- This is needed or you'll get some error because you need the file paths to be the same or it gives you an error like `Unable to open 'init.c': Unable to read file '/pintos/src/threads/init.c' (Error: Unable to resolve non-existing file '/pintos/src/threads/init.c').`

## Usage

1. Run `dpin` on your host machine
2. Run `pintos` in the container with `--gdb --`
3. In VS Code, `CTRL+P`
4. Select `>Debug: Start Debugging`
5. **Note** Pintos GDB macros (`dumplist` and friends) can be run using `-exec XXX` (Example: `-exec dumplist &all_list thread allelem`)

## Resources Used

- [Remote debugging or debugging with a local debugger server](https://code.visualstudio.com/docs/cpp/launch-json-reference#_remote-debugging-or-debugging-with-a-local-debugger-server)
- [How to attach to remote gdb with vscode?](https://stackoverflow.com/questions/53519668/how-to-attach-to-remote-gdb-with-vscode)