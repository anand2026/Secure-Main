# Secure-Main

**Secure** is a powerful, privacy-focused encryption and decryption application. No fees. No servers. No tracking.

[![GitHub](https://img.shields.io/badge/GitHub-Secure--Main-blue)](https://github.com/anand2026/Secure-Main)

## 🔐 What is it?

A Next.js-based web application that encrypts and decrypts your data using industry-standard cryptographic algorithms. Encrypt files or text using either symmetric (password-based) or asymmetric (public/private key) encryption. Everything runs entirely in your browser—no data ever leaves your machine.

## ✨ Features

### Security
- **XChaCha20-Poly1305** - for symmetric encryption
- **Argon2id** - for password-based key derivation
- **X25519** - for key exchange
- **libsodium** - industry-standard cryptographic library

### Privacy
- 🔒 All operations happen client-side in your browser
- 📴 No data is ever collected or sent to anyone
- 🚫 No tracking, no analytics, no third-party services
- 💾 Your data stays on your machine

### Functionality
- 🔑 Symmetric and asymmetric encryption/decryption
- 📁 File encryption (any file type)
- 📝 Text encryption
- 🔐 Secure password generation
- 🔑 Key pair generation (public/private keys)
- 📊 Password strength estimation
- 📱 QR code support for sharing encrypted data
- 🌐 Multilingual support (12 languages)
- 📴 PWA with offline support
- 🐳 Docker support for easy deployment

## 🚀 Getting Started

### Prerequisites

- Node.js 14.x or higher
- npm or yarn

### Installation with npm

1. **Clone the repository**
   ```bash
   git clone https://github.com/anand2026/Secure-Main.git
   cd Secure-Main
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   
   Navigate to [http://localhost:3000](http://localhost:3000)

### Installation with Docker

```bash
# Using docker-compose
docker-compose up

# Or build and run manually
docker build -t secure-main .
docker run -p 3000:3000 secure-main
```

## 📖 Usage

### Encryption with Password (Symmetric)

1. Navigate to the main page
2. Enter your text or upload a file
3. Choose a strong password
4. Click "Encrypt"
5. Download the encrypted data or copy it to your clipboard
6. Share the encrypted data securely

### Encryption with Keys (Asymmetric)

1. Go to the "Generate Keys" page
2. Create a new key pair
3. Share your **public key** with others
4. When someone sends you an encrypted message:
   - They use your public key to encrypt
   - You use your private key + password to decrypt

### Decryption

1. Paste the encrypted data or upload an encrypted file
2. Enter your password (symmetric) or private key (asymmetric)
3. Click "Decrypt"
4. Access your original data

## 🛠️ Technology Stack

| Category | Technology |
|----------|-----------|
| **Framework** | Next.js 12 |
| **UI Library** | Material-UI v4 |
| **Encryption** | libsodium-wrappers |
| **Testing** | Cypress |
| **PWA** | Custom service worker |
| **Styling** | Material-UI + Custom CSS |
| **Internationalization** | 12 languages |
| **Deployment** | Docker, GitHub Actions |

## 📜 Available Scripts

```bash
npm run dev      # Start development server (localhost:3000)
npm run build    # Build for production
npm run start    # Start production server (port 3991)
npm test         # Open Cypress test runner
npm run lint     # Run ESLint code quality checks
```

## 🌍 Supported Languages

English (en_US) • Spanish (es_ES) • French (fr_FR) • German (de_DE) • Italian (it_IT) • Japanese (ja_JP) • Chinese (zh_CN) • Russian (ru_RU) • Czech (cs_CS) • Slovak (sk_SK) • Turkish (tr_TR)

## 🔒 Security & Privacy

**Complete Privacy**
- ✅ All encryption/decryption happens locally in your browser
- ✅ No data is ever sent to any server
- ✅ No tracking or analytics
- ✅ No user accounts or data storage
- ✅ Open source—review the code yourself

**Industry-Standard Cryptography**
- Uses libsodium for all cryptographic operations
- XChaCha20-Poly1305 for authenticated encryption
- Argon2id for password-based key derivation
- X25519 for secure key exchange

## 🧪 Testing

Run the Cypress test suite:

```bash
npm test
```

Tests include:
- Symmetric encryption/decryption
- Asymmetric encryption/decryption
- File upload and download
- Password generation
- Key pair generation

## 📁 Project Structure

```
secure-main/
├── pages/              # Next.js pages
├── src/
│   ├── components/     # React components
│   ├── config/         # Configuration files
│   ├── helpers/        # Helper functions
│   ├── utils/          # Utility functions
│   └── views/          # View containers
├── public/             # Static assets
├── locales/            # Internationalization
├── cypress/            # E2E tests
└── service-worker/     # PWA service worker
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is open source and available under the MIT License.

## 👤 Author

**Anand Singh**
- GitHub: [@anand2026](https://github.com/anand2026)
- Repository: [Secure-Main](https://github.com/anand2026/Secure-Main)

## ⚠️ Security Note

While this application uses industry-standard encryption libraries (libsodium), please:
- Conduct your own security audit before using it for highly sensitive data
- Always use strong, unique passwords
- Keep your private keys secure and never share them
- Backup your keys in a safe place

## 🙏 Acknowledgments

- Built with [libsodium](https://libsodium.gitbook.io/)
- UI powered by [Material-UI](https://material-ui.com/)
- Framework by [Next.js](https://nextjs.org/)

---

**Made with ❤️ for privacy and security**

