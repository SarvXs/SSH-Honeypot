# SSH-Honeypot
This project is an SSH server honeypot written in Python. It emulates an SSH service, capturing credentials used in attempted logins. This tool can be used to study and monitor unauthorized access attempts.
Here’s your **fully formatted `README.md`** for the **SSH Honeypot project**, ready to drop into your GitHub repo.


---

 ✨ Features

- 🪧 Customizable Banners: Use default or custom SSH banners to mimic real environments
- 🔐 RSA Key Management: Generates or uses existing RSA keys for secure communication
- 🧾 Detailed Logging: Logs timestamp, IP address, username, and password of all attempts
- 🧵 Multi-threaded: Handles multiple SSH connections simultaneously

---

 📦 Requirements

- Python 3.x
- Install dependencies:

```bash
pip install paramiko pyfiglet
````

---

 🚀 Usage

To run the honeypot:

```bash
python ssh-honeypot.py [options]
```

---

 🧰 Command-Line Options

| Option                                 | Description                                      |
| -------------------------------------- | ------------------------------------------------ |
| `-l`, `--list-banners`                 | List available banners                           |
| `-b INDEX`, `--banner INDEX`           | Select banner from list by index                 |
| `-B STRING`, `--banner-string STRING`  | Use a custom banner string                       |
| `-f RSA_FILE`, `--file RSA_FILE`       | Path to RSA key file (generates if not provided) |
| `-n MAX_NUMBER`, `--number MAX_NUMBER` | Max simultaneous connections (default: 10)       |
| `-o LOG_FILE`, `--output LOG_FILE`     | Output log file (default: `./ssh-honeypot.log`)  |
| `-p PORT`, `--port PORT`               | Port to listen on (default: 2222)                |

---

 💡 Example

Start the SSH honeypot on port `2222` with a custom banner and log file:

```bash
python ssh-honeypot.py -B "SSH-2.0-OpenSSH_8.0p1 Ubuntu-6ubuntu0.1" -o my_log.log -p 2222
```

---

 📄 Logging Format

Each login attempt is logged like this:

```
timestamp    IP_address    username    password
```

Log file default location: `./ssh-honeypot.log`

---

 🤝 Contributions

Contributions are welcome!
Fork this repository, make your changes, and open a pull request.

---

 📝 License

This project is licensed under the **MIT License**.
See the `LICENSE` file for details.

---

 👤 Author

Developed by [Sarvesvaraan (SarvXs)](https://github.com/SarvXs)
📫 [k.s.sarvesvaraan@gmail.com](mailto:k.s.sarvesvaraan@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/sarvesvaraan-k-s-a06a76251)

---




