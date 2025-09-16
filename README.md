# Log Archive Tool

A robust command-line utility for archiving log files with automatic timestamping. This tool is perfect for system administrators, DevOps engineers, and anyone who needs to maintain organized log archives.

## 📋 Features

- **Simple Command-Line Interface**: Archive logs with a single command
- **Automatic Timestamping**: Each archive is uniquely identified with date and time
- **Compressed Storage**: Efficiently stores logs using tar.gz compression
- **Archive Logging**: Maintains a detailed log of all archiving operations
- **Error Handling**: Robust validation of inputs and operations

## 🚀 Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/MGhaith/Log-Archive-Tool.git
cd Log-Archive-Tool
```
Make the script executable:
```bash
chmod +x log-archive
```

## 💻 Usage

Archive logs from a directory:

```bash
./log-archive /path/to/logs
```
>**Note:** 
- The most common location for logs on a unix based system is ```/var/log```.
- The script must be run with appropriate permissions (e.g., sudo) to access log directories.

### Example

```bash
./log-archive /var/log
```

This will:
1. Create a timestamped archive in `~/log_archives/`
2. Record the operation in `~/log_archives/archive.log`
3. Display a success message with the archive location

## 📁 Output

- Archives are stored in `~/log_archives/` by default
- Each archive is named `logs_archive_YYYYMMDD_HHMMSS.tar.gz`
- A log entry is added to `~/log_archives/archive.log` for each operation
## 🔧 Technical Details

The tool:
- Uses bash scripting for maximum compatibility
- Implements error handling for directory validation
- Creates necessary directories automatically
- Provides clear feedback on operations

## 🛠️ Future Enhancements

- Configurable archive location
- Email/SMS notification.
- Remote server upload (scp, rsync, or S3 upload)
- Config file support

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](https://github.com/MGhaith/Log-Archive-Tool/blob/main/LICENSE) file for details.