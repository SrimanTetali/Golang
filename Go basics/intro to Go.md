# Introduction to Go

### What is Go?
- Go is often referred as Golang.
- it is Statically typed (type of variable is determined at compile time).
- Go is a compiled programming language designed by Google.
- Go is known for its simplicity, efficiency, and strong support for concurrent programming.
- Go was created to enhance programming productivity, particularly for modern computing environments. It addresses the challenges of multicore processors, networked systems, and large codebases.

### Why Learn Go?
- **Concurrency:** Go has built-in support for concurrent programming using goroutines and channels.
- **Performance:** Go is a compiled language, which means it performs faster than interpreted languages like Python.
- **Simplicity:** The syntax of Go is clean and easy to understand, making it a great choice for both beginners and experienced developers.
- **Strong Standard Library:** Go comes with a powerful standard library that supports a wide range of functionalities, from web servers to cryptography.

### Installing Go
To start writing Go programs, you need to install Go on your system.
#### Download Go
- Go to the official [Go download page](https://golang.org/dl/) and download the latest stable version for your operating system.

#### Installation
- **On Windows**: Run the installer and follow the prompts.
- **On macOS**: You can use Homebrew:
  ```bash
  brew install go
  ```
- **On Linux**: You can use the following commands to install Go:
  ```bash
  wget https://golang.org/dl/go1.21.0.linux-amd64.tar.gz
  sudo tar -xvf go1.21.0.linux-amd64.tar.gz -C /usr/local
  ```
- Add Go to your PATH by adding these lines to your ~/.profile or ~/.bashrc file:
  ```bash
  export GOROOT=/usr/local/go
  export GOPATH=$HOME/go
  export PATH=$GOPATH/bin:$GOROOT/bin:$PATH
  ```
- Reload the profile:
  ```bash
  source ~/.profile
  ```
#### Verify Installation:
- This command should output the installed Go version.
  ```bash
  source ~/.profile
  ```
#### Your First Go Program
Let’s write a simple "Hello, World!" program in Go to ensure everything is set up correctly.
1. **Create a new directory for your project:**
   ```bash
   mkdir hello
   cd hello
   ```
2. **Create a new Go file named main.go:**
   ```bash
   touch main.go
   ```
3. Write the following code into main.go
   ```bash
   package main
   import "fmt"
   func main() {
    fmt.Println("Hello, World!")
   }
   ```
4. **Run the Program**
   ```bash
   go run main.go
   ```
## Understanding the Code

Let’s understand the above Go program:

- **`package main`**: Defines the package name. `main` is a special package in Go, the program will start executing from the `main` package.
- **`import "fmt"`**: Imports the `fmt` package, which contains functions for formatting and printing text to the console.
- **`func main()`**: Defines the `main` function, which is the entry point of a Go program.
- **`fmt.Println("Hello, World!")`**: Calls the `Println` function from the `fmt` package to print `Hello, World!` to the console.

