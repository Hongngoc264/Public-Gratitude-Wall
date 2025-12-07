# Public Gratitude Wall

A blockchain-based decentralized application (dApp) that allows users to share appreciation messages and celebrate those who make a difference in their community.

##  Overview

**Public Gratitude Wall** is an innovative platform built on the IOTA blockchain that enables users to:
-  Post meaningful gratitude messages
-  Appreciate and celebrate community members
-  Earn recognition badges for spreading positivity
-  Track your gratitude impact with detailed metrics
-  Build a culture of appreciation and kindness

##  Features

### Core Features
- **Gratitude Messages**: Share heartfelt appreciation with specific recipients
- **Multiple Categories**: Kindness, Leadership, Teamwork, Inspiration, Support, and Generosity
- **Impact Metrics**: Track hearts, shares, views, and community engagement
- **Achievement Badges**: Earn "Gratitude Champion" awards for meaningful contributions
- **Wallet Integration**: Connect via IOTA dApp Kit for secure transactions
- **Transaction Tracking**: Monitor all gratitude posts on the blockchain

### User Profile
- **Messages Posted**: Total gratitude messages shared
- **Hearts Received**: Recognition from the community
- **Community Impact**: Overall positive influence measured
- **Positive Vibes**: Engagement and shares from your messages

## 🛠️ Tech Stack

- **Frontend**: React + TypeScript
- **Styling**: Radix UI + Custom CSS
- **Blockchain**: IOTA dApp Kit
- **State Management**: React Hooks
- **Build Tool**: Next.js

##  Installation

### Prerequisites
- Node.js (v16+)
- npm or yarn
- IOTA wallet (for blockchain interaction)

### Setup

1. **Clone the repository**
```bash
git clone https://github.com/Hongngoc264/Public-Gratitude-Wall.git
cd Public-Gratitude-Wall
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
Create a `.env.local` file with required configurations:
```bash
NEXT_PUBLIC_IOTA_NETWORK=testnet
```

4. **Run the development server**
```bash
npm run dev
```

5. **Open in browser**
Navigate to `http://localhost:3000`

## 📱 Usage

### Posting Gratitude

1. **Connect Wallet**: Click the connect button to link your IOTA wallet
2. **Fill the Form**:
   - Enter recipient's name or organization
   - Select appreciation category
   - Write your gratitude message (be specific and heartfelt)
   - Set impact metrics (optional)
3. **Submit**: Click " Post to Gratitude Wall" button
4. **Confirm**: Approve the transaction in your wallet
5. **Celebrate**: Your message appears on the wall!

### Viewing Profile

- See your gratitude statistics
- Track community engagement
- View achievement badges
- Monitor transaction history

### Earning Badges

- Post meaningful gratitude messages
- Engage with the community
- Reach the badge threshold
- Click " Claim Gratitude Badge"

##  UI Components

### Main Sections

**Header**
- Application title and tagline
- Welcome message for new users

**Profile Card**
- Personal gratitude statistics
- Achievement badges
- Profile ID reference

**Gratitude Form**
- Recipient information
- Category selection
- Message composition
- Metric inputs (Impact, Hearts, Shares, Views)

**Transaction Status**
- Transaction hash display
- Confirmation status
- Error handling

## 🔧 API Integration

The application uses smart contract functions via `useContract` hook:

```typescript
actions.cookPizza(
  recipientLength,
  hearts,
  messageLength,
  views,
  shares,
  categoryLength,
  impactScore,
  appreciation
)

actions.getFlag() // Claim badge
```

##  Data Structure

### Gratitude Post
```typescript
{
  recipientName: string      // Who you appreciate
  gratitudeMessage: string   // Your message
  category: string          // Type of appreciation
  impactScore: number       // Impact level (0-100)
  hearts: number            // Likes received
  shares: number            // Times shared
  views: number             // View count
}
```

### User Profile
```typescript
{
  pizzaBoxId: string        // User profile ID
  oliveOils: number         // Messages posted
  yeast: number             // Hearts received
  flour: number             // Community impact
  water: number             // Positive vibes/shares
}
```

##  Project Goals

-  Create a positive community platform
-  Incentivize appreciation and gratitude
-  Build on blockchain for transparency
-  Celebrate human connection
-  Spread kindness and positivity

##  Security

- Wallet-based authentication via IOTA dApp Kit
- Smart contract validation
- Blockchain transaction confirmation
- No sensitive data storage on client

##  Project Structure

```
components/
  └── sample.tsx           # Main application component

hooks/
  └── useContract.ts       # Smart contract integration

pages/
  └── index.tsx            # Home page

styles/
  └── globals.css          # Global styling

.env.local                 # Environment configuration
```

##  Deployment

### Deploy to Vercel

```bash
vercel deploy
```

### Deploy to Other Platforms

1. Build the project:
```bash
npm run build
```

2. Deploy the `.next` folder to your hosting provider

##  Environment Variables

```bash
NEXT_PUBLIC_IOTA_NETWORK=testnet
NEXT_PUBLIC_CONTRACT_ADDRESS=<your_contract_address>
```

##  Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

##  License

This project is licensed under the MIT License - see the LICENSE file for details.

##  Authors

- **Hongngoc264** - Initial development

##  Acknowledgments

- IOTA Foundation for blockchain infrastructure
- Radix UI for beautiful components
- Next.js for the framework

##  Support

For issues, questions, or suggestions:
- Open an issue on GitHub
- Contact: [your-email@example.com]
- Documentation: Check the Wiki section

##  Live Demo

Visit the live application: [Your deployment URL]

---

**Made with  to spread gratitude and positivity** 
