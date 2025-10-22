# WhatsApp Bot - Ready Made Commands

## 🤖 Overview
This is a comprehensive WhatsApp bot built with Python that provides various ready-to-use commands for automation, information retrieval, and entertainment.

## 🚀 Installation

### Prerequisites
- Python 3.8+
- pip package manager
- WhatsApp Business API or WhatsApp Web access

### Setup Steps
```bash
# Clone the repository
git clone https://github.com/yourusername/whatsapp-bot.git
cd whatsapp-bot

# Install dependencies
pip install -r requirements.txt

# Install ChromeDriver (for WhatsApp Web)
# Download from: https://chromedriver.chromium.org/
# Or use: pip install chromedriver-autoinstaller
```

## 🔧 Configuration

Create a `.env` file in your project root:
```env
PHONE_NUMBER=+1234567890
WEBHOOK_URL=https://your-webhook-url.com
API_KEY=your_api_key_here
```

## 📋 Ready-Made Commands

### 🎯 Basic Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!help` | Show all available commands | `!help` |
| `!ping` | Check bot status | `!ping` |
| `!info` | Get bot information | `!info` |
| `!uptime` | Check bot uptime | `!uptime` |

### 💬 Utility Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!weather [city]` | Get current weather | `!weather London` |
| `!define [word]` | Get word definition | `!define python` |
| `!translate [text]` | Translate text to English | `!translate Hola mundo` |
| `!currency [amount] [from] [to]` | Convert currency | `!currency 100 USD EUR` |
| `!time [timezone]` | Get current time | `!time America/New_York` |

### 🎮 Entertainment Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!joke` | Get a random joke | `!joke` |
| `!quote` | Get inspirational quote | `!quote` |
| `!meme` | Get random meme | `!meme` |
| `!trivia` | Start trivia game | `!trivia` |
| `!8ball [question]` | Magic 8-ball response | `!8ball Will I win?` |

### 📊 Group Management Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!kick [@user]` | Kick user from group | `!kick @John` |
| `!ban [@user]` | Ban user from group | `!ban @John` |
| `!unban [@user]` | Unban user | `!unban @John` |
| `!mute [@user] [time]` | Mute user temporarily | `!mute @John 30m` |
| `!warn [@user] [reason]` | Warn user | `!warn @John Spamming` |
| `!poll [question]` | Create poll | `!poll Best programming language?` |

### 🔍 Information Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!whois [@user]` | Get user info | `!whois @John` |
| `!serverinfo` | Get server info | `!serverinfo` |
| `!avatar [@user]` | Get user avatar | `!avatar @John` |
| `!roleinfo [role]` | Get role info | `!roleinfo admin` |

### 🎨 Creative Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!qr [text]` | Generate QR code | `!qr Hello World` |
| `!ascii [text]` | Convert text to ASCII art | `!ascii BOT` |
| `!color [hex]` | Show color info | `!color #FF5733` |
| `!emoji [text]` | Convert text to emojis | `!emoji love` |

### 📈 Admin Commands
| Command | Description | Usage |
|---------|-------------|-------|
| `!prefix [symbol]` | Change command prefix | `!prefix $` |
| `!settings` | View bot settings | `!settings` |
| `!backup` | Backup server data | `!backup` |
| `!restore` | Restore from backup | `!restore` |
| `!logs` | View recent logs | `!logs` |

## 🛠️ Advanced Features

### Auto-Responses
- **Greetings**: Automatically responds to "hi", "hello", "hey"
- **Goodbyes**: Responds to "bye", "goodbye", "see you"
- **Thank you**: Responds to "thanks", "thank you"

### Scheduled Messages
```python
# Schedule daily reminders
!schedule daily 09:00 "Good morning! 🌅"
!schedule weekly Monday 10:00 "Weekly team meeting"
```

### Custom Commands
```python
# Create custom responses
!custom add greeting "Hello there! 👋 How can I help?"
!custom add rules "1. Be respectful\n2. No spam\n3. Have fun!"
```

## 📁 Project Structure
```
whatsapp-bot/
├── main.py              # Main bot file
├── commands/            # Command modules
│   ├── basic.py
│   ├── utility.py
│   ├── entertainment.py
│   ├── moderation.py
│   └── admin.py
├── utils/               # Utility functions
│   ├── database.py
│   ├── api_helpers.py
│   └── validators.py
├── config/              # Configuration files
│   ├── settings.json
│   └── commands.json
├── requirements.txt     # Dependencies
├── .env                 # Environment variables
└── README.md            # This file
```

## ⚙️ Running the Bot

### Method 1: WhatsApp Web (Development)
```bash
python main.py --web
```

### Method 2: WhatsApp Business API (Production)
```bash
python main.py --api
```

### Method 3: Docker
```bash
docker build -t whatsapp-bot .
docker run -d --env-file .env whatsapp-bot
```

## 🔒 Security Features
- **Rate limiting** to prevent spam
- **Permission checks** for admin commands
- **Input validation** to prevent injection attacks
- **Encrypted storage** for sensitive data
- **Two-factor authentication** support

## 📊 Monitoring & Logging
- Real-time command usage tracking
- Error logging with timestamps
- Performance monitoring
- User activity reports

## 🌍 Localization
Supports multiple languages:
- English (default)
- Spanish
- French
- Portuguese
- Arabic
- Hindi

To change language:
```bash
!language es
```

## 🤝 Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support
For issues and feature requests, please open an issue on GitHub or contact:
- Email: support@whatsappbot.dev
- Discord: [Join our Discord server](https://discord.gg/your-invite)

## 🙏 Acknowledgments
- [Selenium](https://www.selenium.dev/) - Web automation
- [Requests](https://docs.python-requests.org/) - HTTP library
- [Pillow](https://python-pillow.org/) - Image processing
- [OpenWeatherMap API](https://openweathermap.org/api) - Weather data
- [Free Dictionary API](https://dictionaryapi.dev/) - Dictionary service

---

**Note**: Always comply with WhatsApp's Terms of Service and local laws when using automated bots. This bot is designed for legitimate use cases like customer support, information sharing, and group management.            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: "";
            position: absolute;
            top: -50px;
            right: -50px;
            width: 200px;
            height: 200px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
        }
        
        header h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
            position: relative;
            z-index: 2;
        }
        
        .whatsapp-icon {
            width: 60px;
            height: 60px;
            background: var(--whatsapp-green);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
        }
        
        header p {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }
        
        .card {
            background: var(--white);
            border-radius: 15px;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            border-left: 4px solid var(--whatsapp-green);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
        }
        
        .card h2 {
            color: var(--whatsapp-darker-green);
            margin-bottom: 1.5rem;
            font-size: 1.8rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .card h2::before {
            content: "🔹";
            color: var(--whatsapp-green);
        }
        
        .card h3 {
            color: var(--whatsapp-dark-green);
            margin: 1.2rem 0 0.8rem;
            font-size: 1.3rem;
        }
        
        .code-block {
            background: var(--medium-gray);
            color: var(--text-light);
            padding: 1.5rem;
            border-radius: 10px;
            margin: 1rem 0;
            overflow-x: auto;
            font-family: 'Courier New', monospace;
            font-size: 14px;
        }
        
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }
        
        .feature-card {
            background: var(--white);
            border-radius: 12px;
            padding: 1.5rem;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.08);
            border-top: 3px solid var(--whatsapp-green);
        }
        
        .feature-card h4 {
            color: var(--whatsapp-darker-green);
            margin-bottom: 0.8rem;
            font-size: 1.2rem;
        }
        
        .badge {
            display: inline-block;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-right: 8px;
            margin-bottom: 8px;
        }
        
        .badge-success {
            background: rgba(76, 175, 80, 0.1);
            color: var(--success);
        }
        
        .badge-warning {
            background: rgba(255, 193, 7, 0.1);
            color: var(--warning);
        }
        
        .badge-info {
            background: rgba(33, 150, 243, 0.1);
            color: var(--info);
        }
        
        ul, ol {
            margin-left: 1.5rem;
            margin-bottom: 1rem;
        }
        
        li {
            margin-bottom: 0.5rem;
        }
        
        a {
            color: var(--whatsapp-green);
            text-decoration: none;
            font-weight: 600;
        }
        
        a:hover {
            text-decoration: underline;
        }
        
        .note {
            background: rgba(37, 211, 102, 0.1);
            border-left: 4px solid var(--whatsapp-green);
            padding: 1rem;
            border-radius: 0 8px 8px 0;
            margin: 1rem 0;
        }
        
        footer {
            text-align: center;
            padding: 2rem;
            color: var(--gray);
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }
            
            .card {
                padding: 1.5rem;
            }
            
            .container {
                padding: 10px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1>
                <div class="whatsapp-icon">💬</div>
                WhatsApp Bot Base
            </h1>
            <p>A comprehensive foundation for building powerful WhatsApp automation bots using the WhatsApp Business API or third-party solutions</p>
        </header>

        <div class="card">
            <h2>Overview</h2>
            <p>WhatsApp Bot Base provides a ready-to-use framework for creating automated WhatsApp bots that can handle customer service, notifications, marketing campaigns, and more. This base includes essential components, best practices, and example implementations to get you started quickly.</p>
            
            <div class="note">
                <strong>⚠️ Important:</strong> Always comply with WhatsApp's Terms of Service and Business Policy. Automated messaging must provide value to users and include proper opt-out mechanisms.
            </div>
        </div>

        <div class="card">
            <h2>Features</h2>
            <div class="feature-grid">
                <div class="feature-card">
                    <h4>Message Handling</h4>
                    <p>Process incoming messages, detect keywords, and respond automatically with intelligent routing.</p>
                </div>
                <div class="feature-card">
                    <h4>Media Support</h4>
                    <p>Handle images, documents, audio, and video files with proper validation and storage.</p>
                </div>
                <div class="feature-card">
                    <h4>Interactive Messages</h4>
                    <p>Send buttons, lists, and quick replies to create engaging user experiences.</p>
                </div>
                <div class="feature-card">
                    <h4>Database Integration</h4>
                    <p>Store user data, conversation history, and preferences in your preferred database.</p>
                </div>
                <div class="feature-card">
                    <h4>Webhook Support</h4>
                    <p>Receive real-time message notifications and send responses instantly.</p>
                </div>
                <div class="feature-card">
                    <h4>Rate Limiting</h4>
                    <p
