# Pintos Operating System Implementation

This repository contains my implementation of the Pintos operating system, a teaching operating system framework originally developed by Ben Pfaff at Stanford University. The project consists of four major components, each building upon the previous to create a fully functional operating system.

## 📚 About Pintos

Pintos is a simple operating system framework for the 80x86 architecture. It supports kernel threads, loading and running user programs, and a file system, but it implements all of these in a very simple way.

## 🚀 Project Structure

### Project 1: Threads
**Objective**: Implement a functional thread system with priority scheduling and synchronization primitives.

**Key Features**:
- Priority-based thread scheduling
- Implementation of 4.4BSD scheduler
- Synchronization mechanisms (locks, semaphores, condition variables)
- Alarm clock functionality
- Advanced scheduler with multi-level feedback queue

**Implementation Highlights**:
- Solved thread synchronization problems
- Implemented priority donation mechanism
- Created efficient waiting queue management

### Project 2: User Programs
**Objective**: Enable user-space program execution and system call handling.

**Key Features**:
- Process creation and termination
- System call implementation (exec, wait, exit, etc.)
- File descriptor management
- Argument parsing and stack setup
- Exception handling and error reporting

**Implementation Highlights**:
- Robust argument passing mechanism
- Proper parent-child process relationship management
- Secure system call validation

### Project 3: Virtual Memory
**Objective**: Implement virtual memory management with page swapping and memory-mapped files.

**Key Features**:
- Page fault handling
- Page replacement algorithms (LRU/Clock algorithm)
- Memory-mapped files
- Lazy loading of executables
- Stack growth on demand

**Implementation Highlights**:
- Efficient page table management
- Swapping mechanism with disk I/O
- Memory-mapped file support for efficient file access

### Project 4: File System
**Objective**: Implement a persistent, extensible file system similar to FFS (Fast File System).

**Key Features**:
- Extensible file system structure
- Directory operations
- File creation, deletion, and modification
- Buffer cache implementation
- Subdirectories support

**Implementation Highlights**:
- Efficient inode management
- Buffer cache with LRU replacement
- Robust file system consistency

## 🛠️ Building and Running

### Prerequisites
- GCC cross-compiler for x86
- QEMU or Bochs emulator
- Perl (for test scripts)

### Build Instructions

Navigate to the project directory:
```bash
cd "Project 1 - Threads/src/threads"  # or Project 2, 3, or 4
make
```

### Running Tests

Each project includes comprehensive test suites:

```bash
cd tests
make check
```

## 📝 Notes

- This is an academic project focused on understanding operating system internals
- The implementation follows the Pintos design document specifications
- All code includes detailed comments explaining design decisions
- Test coverage includes edge cases and stress tests

## 🎯 Learning Outcomes

Through this project, I gained hands-on experience with:
- Operating system kernel development
- Thread scheduling algorithms
- Memory management techniques
- File system design and implementation
- System call interfaces
- Synchronization primitives

## 📄 License

This project is based on Pintos, which is released under the GNU GPL v2 license. See the LICENSE file in each project's source directory for details.

## 🙏 Acknowledgments

- Ben Pfaff and the Pintos development team at Stanford University
- The educational design that made this learning experience possible

---


