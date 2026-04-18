# AI Security Check

A security solution designed to prevent phone scams by detecting AI-cloned biometric attempts when phones are borrowed for help.

## 🎯 Problem Statement

Phone scams have evolved beyond simple social engineering. Scammers now exploit a common scenario: when someone borrows your phone to make a call or access an app, they can attempt to bypass biometric authentication using AI-generated clones of your face, voice, or fingerprints. This creates a critical security vulnerability where your biometric data becomes a liability.

## 🛡️ Solution

AI Security Check is a comprehensive security framework that:

- **Detects anomalies** in biometric authentication patterns
- **Identifies AI clones** of facial features, voice, and fingerprints using advanced AI detection
- **Alerts users** to suspicious authentication attempts
- **Prevents unauthorized access** during phone borrowing scenarios
- **Provides security insights** about potential vulnerabilities

## 🔧 Tech Stack

### Backend
- **Framework**: FastAPI (Python)
- **Type Checking**: Pydantic
- **Code Quality**: Black, isort

### Frontend
- **Framework**: Next.js 16
- **Language**: TypeScript
- **UI Styling**: Tailwind CSS 4
- **Runtime**: React 19

## 📁 Project Structure

```
ai-security-check/
├── backend/                 # FastAPI backend service
│   ├── app/
│   │   └── main.py         # Main application entry point
│   ├── requirements.txt     # Python dependencies
│   └── .venv/              # Python virtual environment
│
├── frontend/                # Next.js frontend application
│   ├── app/
│   │   ├── page.tsx        # Home page
│   │   ├── layout.tsx      # Root layout
│   │   └── globals.css     # Global styles
│   ├── public/             # Static assets
│   ├── package.json        # Node.js dependencies
│   ├── tsconfig.json       # TypeScript configuration
│   ├── next.config.ts      # Next.js configuration
│   └── eslint.config.mjs   # ESLint configuration
│
└── README.md               # Project documentation
```

## 🚀 Getting Started

### Prerequisites

- **Python 3.8+** (for backend)
- **Node.js 18+** (for frontend)
- **pip** (Python package manager)
- **npm** or **yarn** (Node.js package manager)

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a Python virtual environment:
   ```bash
   python -m venv .venv
   ```

3. Activate the virtual environment:
   - **Windows**:
     ```bash
     .venv\Scripts\activate
     ```
   - **macOS/Linux**:
     ```bash
     source .venv/bin/activate
     ```

4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

5. Run the backend server:
   ```bash
   python -m uvicorn app.main:app --reload
   ```

   The API will be available at `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

   The application will be available at `http://localhost:3000`

## 📝 Scripts

### Backend
```bash
# Format code with Black
black app/

# Sort imports with isort
isort app/
```

### Frontend
```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Run ESLint
npm run lint
```

## 🔐 Key Features (In Development)

- [ ] AI-powered biometric anomaly detection
- [ ] Real-time threat alerts
- [ ] Facial recognition clone detection
- [ ] Voice authentication verification
- [ ] Fingerprint pattern analysis
- [ ] User dashboard with security insights
- [ ] Authentication logs and history
- [ ] Security recommendations

## 🧪 Testing

(Testing setup documentation to be added)

## 🤝 Contributing

Contributions are welcome! Please follow these guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

### Code Quality

- Use **Black** for Python formatting
- Use **isort** for import sorting
- Use **ESLint** for JavaScript/TypeScript
- Maintain type safety with TypeScript and Pydantic

## 📖 API Documentation

Once the backend is running, access the interactive API documentation:
- **Swagger UI**: http://localhost:8000/docs
- **ReDoc**: http://localhost:8000/redoc

## 🔒 Security Considerations

- Never commit sensitive credentials
- Use environment variables for API keys and secrets
- Enable CORS only for trusted domains
- Validate all user inputs
- Keep dependencies updated regularly

## 📝 License

(Add your license information here)

## 👥 Contact

For questions or feedback about this project, please reach out to the development team.

---

**Status**: 🚧 Under Development

This project is actively being developed. Features and documentation are subject to change.
