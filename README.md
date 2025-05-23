# prowlerscan-aws-sso

Automated **Prowler** security scanning for **AWS** using SSO profiles on Linux (Debian/Ubuntu and RedHat-based distros).

## Features

- One-command setup and run: Installs dependencies, logs into AWS SSO, and runs Prowler
- Works on both Debian/Ubuntu and RedHat/CentOS/Fedora/AlmaLinux/Rocky Linux
- Shows live Prowler progress in terminal (with log)
- Archives all scan results and compliance data to `/tmp`
- Cleans up after run

## Usage

1. Clone this repo or download the script:
   ```sh
   git clone <this-repo-url>
   cd <repo-directory>
   chmod +x prowlerscan-aws-sso

2. Make sure you have an AWS SSO profile configured.

3. Run the scan: ./prowlerscan-aws-sso my-infra

4. After the scan, open the HTML report or compliance folder:
   ```
   🌐 View the report in your browser:
    file:///tmp/prowlerscan-out-YYYYMMDD-HHMMSS/output/prowler-output-....html
   📊 Detailed compliance results archived at:
    file:///tmp/prowlerscan-out-YYYYMMDD-HHMMSS/output/compliance/
   ```

### Requirements

    Linux (Debian, Ubuntu, CentOS, RedHat, Fedora, AlmaLinux, Rocky Linux)

    AWS SSO profile already configured (aws configure sso)

    Sudo privileges to install packages

### Notes

    The script installs all required system and Python packages automatically.

    For other OS or manual installation, see the script for dependency hints.
