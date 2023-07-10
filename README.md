# Path Ops

Automate tasks in specific directories for a streamlined workflow.

Path Ops is a lightweight script designed to automate tasks when entering specific directories, streamlining your workflow and saving you time. Whether you're a developer, system administrator, or power user, Path Ops allows you to define custom actions that will be automatically executed upon navigating to specific folders.

## Features

- Automate tasks by running commands upon entering specific directories
- Customizable configuration file for defining folder-specific commands
- Compatible with sh, Bash, and zsh shells
- Silent mode option for suppressing output
- Flag file-based tracking to avoid unnecessary repetitions
- Lightweight and dependency-free

## How to Use

1. Clone this repository to your local machine.
2. Make sure the `path_ops` script is executable: `chmod +x path_ops`.
3. Open the `.path_ops.cfg` configuration file and define your desired folder-specific commands. Follow the provided format: `folder|command1|command2|...`. Place each entry on a new line.
4. Run the `path_ops` script in the background, allowing it to monitor your current directory: `./path_ops &`.
5. Optionally, you can run the script in silent mode by passing the `--silent` flag: `./path_ops --silent &`.
6. Enter any of the configured folders, and the corresponding commands will be executed automatically.
7. The script will create a `.path_ops` flag file in each folder where commands have been executed, ensuring they are not repeated unnecessarily.
8. Enjoy a more streamlined workflow with automated tasks in specific directories!

Note: If you prefer not to use the configuration file, you can modify the `path_ops` script directly by defining folder paths and commands within the script itself. However, using the configuration file provides a more flexible and maintainable approach.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to contribute to this project by opening issues or submitting pull requests. Your feedback and contributions are greatly appreciated!

