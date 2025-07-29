# 🔍 Finder — A Rust Terminal Simulator


    ███████╗██╗███╗   ██╗██████╗ ███████╗██████╗ 
    ██╔════╝██║████╗  ██║██╔══██╗██╔════╝██╔══██╗
    █████╗  ██║██╔██╗ ██║██║  ██║█████╗  ██████╔╝
    ██╔══╝  ██║██║╚██╗██║██║  ██║██╔══╝  ██╔══██╗
    ██║     ██║██║ ╚████║██████╔╝███████╗██║  ██║
    ╚═╝     ╚═╝╚═╝  ╚═══╝╚═════╝ ╚══════╝╚═╝  ╚═╝
    
    Finder is a terminal simulator built in Rust that replicates some of the most common UNIX-like shell commands.
    It’s designed to give a colorful, lightweight, and interactive experience for navigating directories and exploring files,
    while being simple enough for beginners to understand Rust module-based projects.
    
    The ASCII banner you see above is the Finder logo, which greets you when you launch the program.
    It represents the idea of finding and navigating files in a fun, visually engaging way.

## 📝 What Finder Does

    Finder simulates a mini shell environment with the following built-in commands:
    
    cp (Current Path) → Prints the current working directory
    
    vt (View Tree) → Displays a tree-like structure of files and folders
    
    cd (Change Directory) → Navigate into other directories (supports .. to go up)
    
    exit → Gracefully exits the simulator
    
    This makes Finder a practical tool for learning how shells work and exploring file system traversal using Rust.

## ⚡ Key Features

    📂 Navigate your file system without leaving the program
    
    🌳 Generate a tree view of your directories
    
    🎨 Colored and styled CLI output for better readability
    
    🛡️ Handles invalid paths gracefully with helpful error messages
    
    🔑 Built modularly (main.rs, mod_cd.rs, mod_cp.rs, mod_vt.rs) — easy to extend with more commands

    
## 🛠️ Tech Stack
- **Language**: [Rust](https://www.rust-lang.org/) 🦀  
- **CLI Styling**: [colored](https://crates.io/crates/colored) crate for colorful terminal output 🎨  
- **File System Operations**: Rust standard library (`std::fs`, `std::env`, `std::path::PathBuf`) 📂  
- **Program Structure**: Modular design with separate `.rs` files (`main.rs`, `mod_cd.rs`, `mod_cp.rs`, `mod_vt.rs`) 🧩  
- **Build Tool**: [Cargo](https://doc.rust-lang.org/cargo/) ⚙️

  
## 🚀 Getting Started

    Make sure you have Rust installed:
    rustc --version
    
    Clone the repository and build the project:
    git clone https://github.com/SD-Dev10/Explorer_sturct_backup.git
    
    cd Explorer_sturct_backup
    cargo build --release
    Run Finder:
    cargo run
    
## 🖥️ Usage Examples

    Finder ---> cp
    # Output: Current working directory
    
    Finder ---> vt
    # Output: Tree view of the folder structure
    
    Finder ---> cd src
    # Moves into the "src" directory
    
    Finder ---> exit
    # Exits the Finder simulator
    Example Tree Output:
    
    text
    Copy
    Edit
    Finder ---> vt
    |-- "src"
       |__ "main.rs"
       |__ "mod_cd.rs"
       |__ "mod_cp.rs"
       |__ "mod_vt.rs"
## 🔮 Future Plans
    ➕ Add more commands (ls, rm, touch, mv)
    
    ⌨️ Command history and auto-completion
    
    📊 Adjustable depth for tree view (vt)
    
    🖼️ Improved formatting with file type icons

### ⚡ Finder — making terminal exploration simple, colorful, and fun with Rust!
