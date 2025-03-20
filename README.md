# ThreatLensAI Backend 🔧

The beating heart of ThreatLensAI! This backend is built with Node.js, Express, and Prisma, serving up threat intel via GraphQL and real-time updates with WebSockets. It integrates feeds like Shodan and stores data in MongoDB and MySQL. Ready to power a cybersecurity empire! 🌐🔒

## Features ✨
- **Threat Intel**: Pulls and processes data from open-source feeds. 🕵️‍♂️
- **GraphQL Goodness**: Fast, flexible APIs for web and mobile clients. 🚀
- **Real-Time Alerts**: WebSockets push new threats instantly. ⚡
- **Locked Down**: OAuth + MFA for secure user auth. 🔐
- **Dual Storage**: MySQL (users) + MongoDB (threats, preferences). 💾

## Tech Stack 🛠️
- Node.js, Express
- Prisma (MySQL)
- MongoDB
- GraphQL (Apollo Server)
- WebSockets (Socket.IO)
- Testing: Jest

## Getting Started 🚀

### Prerequisites
- Node.js (v18 or higher) 🟢
- MySQL (local or hosted) 🗄️
- MongoDB (local or Atlas) 🍃

### Installation Steps
1. Clone the repo:
   ```bash
   git clone https://github.com/G-Hensley/threat-lens-ai-backend.git
   cd threat-lens-ai-backend
   ```
2. Install Dependencies:
   ```bash
   npm install
   ```
3. Set up your '.env' file:
   ```plaintext
   PORT=5000
   MYSQL_URL=mysql://user:password@localhost:3306/threatlensai
   MONGODB_URL=mongodb://localhost:27017/threatlensai
   SHODAN_API_KEY=your-shodan-api-key
   ```
4. Run Prisma migrations:
   ```bash
   npx prisma migrate dev
   ```
5. Start the server:
   ```bash
   npm run dev
   ```
Check it out at `http://localhost:5000`! 🌐

## API Endpoints 🌐
- **GraphQL**: `/graphql` - Query threats, prefs, and more.
- **WebSocket**: Connect to `/` for live threat updates.

## Contributing 🤝
We’re pumped to collaborate! See [CONTRIBUTING.md](CONTRIBUTING.md) for how to join the fun.

## License 📄
Licensed under the MIT License—check [LICENSE](LICENSE) for the full story.
