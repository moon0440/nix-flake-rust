# Rust Development with Nix Flake

Welcome to my template, designed to streamline your Rust development process using Nix. This comprehensive guide aims to provide you with a detailed understanding of how to leverage various tools for an efficient and organized development workflow in Rust. We utilize Nix, a powerful package manager, to create a consistent development environment. Alongside, we integrate several tools, each serving a unique purpose in enhancing your Rust programming experience.

## Key Components 
At the core, we use Nix, an advanced package manager, to set up a reliable and reproducible development shell specifically for Rust projects. This ensures that you work in a controlled environment with consistent dependencies and tooling. 
- **divnix - Standard:** Used to maintain organization and clarity in your Nix code. It helps in keeping the structure of your Nix configurations neat and readable. 
- **Fenix:** Responsible for fetching the latest Rust binaries through Nix. This ensures that you always have access to the newest features and updates in Rust. 
- **Crane:** A tool that enhances the building process of Rust projects within Nix. It allows for incremental builds, significantly speeding up the development cycle and facilitating rapid iteration. 
- **Rust Analyzer Integration:**  We've seamlessly integrated Rust Analyzer to work out-of-the-box. This is particularly beneficial for terminal-based editors supporting language servers, offering immediate and efficient code analysis. 
- **Editor Recommendation:**  For an editor with exceptional support for both Nix and Rust, we recommend trying out [Helix](https://github.com/helix-editor/helix#readme) . It's configured to work smoothly with this setup, providing an enriched coding experience.

## Getting Started: Bootstrap Your Project

Follow these steps to set up a new Rust project using this template:

```bash
# Create a new empty project directory
mkdir my-project
cd my-project

# Initialize the project with this template
nix flake init -t github:moon0440/nix-flake-rust

# Initialize Git and Cargo, and perform initial build
git init
cargo init # Use --lib for library projects
cargo build # Generates Cargo.lock
git add .
git commit -m "Initial project setup"

# Enter the development shell
direnv allow || nix develop
```



By following these steps, you'll have a Rust project environment ready, complete with all the necessary tools and configurations for an efficient and organized development process.
## Links to Tools 
- **divnix - Standard (std):**  [GitHub - divnix/std](https://github.com/divnix/std#readme) 
- **Nix:**  [NixOS - Nix](https://nixos.org/)
- **Flakes:** [NixOS - Flakes](https://nixos.wiki/wiki/Flakes)
- **Fenix:**  [GitHub - nix-community/fenix](https://github.com/nix-community/fenix#readme) 
- **Crane:**  [GitHub - ipetkov/crane](https://github.com/ipetkov/crane#readme) 
- **Helix Editor:**  [GitHub - helix-editor/helix](https://github.com/helix-editor/helix#readme)

