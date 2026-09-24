# VWERX

VWERX is a GUI-based Windows remote administration tool for authorized
security research, lab environments, and system administration.

> **Use responsibly:** Only use VWERX on systems you own or where you have
> explicit permission. Unauthorized access, monitoring, or control is
> prohibited.

## Features

- Browser-based control panel
- Client status and connection monitoring
- Remote terminal, display, webcam, keyboard, microphone, and file controls
- Payload generation for authorized Windows test environments
- Local configuration for the listening port and login credentials

## Requirements

- Node.js 18 or newer
- npm
- A Windows test environment for client-side features

## Installation

Clone the project and install its dependencies:

```bash
git clone https://github.com/x1ilee/VWERX
cd VWERX
npm install
```

Start the control panel:

```bash
npm start
```

Then open [http://localhost:3415](http://localhost:3415) in your browser.

For development with automatic restarts:

```bash
npm run dev
```

## Configuration

Edit [`config.js`](./config.js) before starting the server:

| Setting | Description |
| --- | --- |
| `port` | Port used by the control panel |
| `username` | Control panel username |
| `password` | Control panel password |

The default development credentials are:

- Username: `admin`
- Password: `admin`

Change these values before using VWERX outside a local test environment.

## Notes

- A newly created client may take 40–50 seconds to connect.
- Keep the control panel private and restrict access to trusted users.
- VWERX is provided for educational and authorized administrative use only.

## License

VWERX is released under the MIT License. See [`LICENSE`](./LICENSE).

## Author

Made by [@x1ilee](https://github.com/x1ilee).
