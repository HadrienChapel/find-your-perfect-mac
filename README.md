# Mac Finder - Interactive Mac Selection Guide

An interactive web application that helps users find the perfect Mac computer based on their needs and preferences. Built with React, TypeScript, and Tailwind CSS.

![Mac Finder Screenshot](https://images.unsplash.com/photo-1517336714731-489689fd1ca8?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80)

## Features

- 🎯 Personalized Mac recommendations based on user preferences
- 📊 Interactive questionnaire with progress tracking
- 💻 Comprehensive Mac options including:
  - MacBook Air (13" & 15")
  - MacBook Pro (14" & 16")
  - iMac 24"
  - Mac Mini
  - Mac Studio
- ✨ Smooth animations and transitions
- 📱 Responsive design for all screen sizes
- 🎨 Modern UI with Tailwind CSS
- 🔍 Detailed product information and descriptions

## Tech Stack

- React 18
- TypeScript
- Tailwind CSS
- Vite
- Lucide React (for icons)

## Project Structure

```
src/
├── components/           # React components
│   ├── ProgressBar.tsx  # Progress indicator
│   ├── QuestionCard.tsx # Question display
│   └── Result.tsx       # Recommendation display
├── data/
│   └── questions.ts     # Questionnaire data
├── types/
│   └── index.ts         # TypeScript interfaces
├── utils/
│   └── recommendations.ts # Recommendation logic
├── App.tsx              # Main application component
└── main.tsx            # Application entry point
```

## Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Adding New Questions

To add new questions, modify the `questions` array in `src/data/questions.ts`. Each question should follow the `Question` interface:

```typescript
interface Question {
  id: string;
  text: string;
  options: {
    text: string;
    value: string;
    description?: string;
  }[];
}
```

### Modifying Recommendations

Update the recommendation logic in `src/utils/recommendations.ts`. The `getMacRecommendation` function takes the user's answers and returns a `MacRecommendation` object.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Acknowledgments

- Icons provided by [Lucide React](https://lucide.dev)
- Images from [Unsplash](https://unsplash.com)
- Built with [Vite](https://vitejs.dev)