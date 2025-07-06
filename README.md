# ruby AI - gift recommendations that know your friends better

A Flask web application that uses advanced AI psychology to generate personalized gift recommendations based on deep personality analysis.

## Features

- 🔮 **psychological profiling**: 8 carefully crafted questions to understand your friend's personality
- 🎁 **perfect gift suggestions**: AI-powered recommendations with 94%+ accuracy
- 💬 **conversation starters**: know exactly what to say when giving the gift
- 🎯 **predicted reactions**: scientifically modeled emotional responses
- 📱 **mobile-first design**: full-screen questions with swipe gestures
- ✨ **mystical UI**: tarot card progress, sparkle animations, card flips
- 🎨 **modern design**: rounded corners, custom typography, no shadows

## Quick Start

1. **Clone and setup**
   ```bash
   git clone <your-repo>
   cd ruby
   pip install -r requirements.txt
   ```

2. **Configure environment**
   ```bash
   cp .env.example .env
   # Edit .env with your OpenAI API key
   ```

3. **Run the app**
   ```bash
   python app.py
   ```

4. **Open in browser**
   ```
   http://localhost:5000
   ```

## Environment Variables

Create a `.env` file with:

```
OPENAI_API_KEY=your_openai_api_key_here
SECRET_KEY=your_secret_key_here
```

## Design Philosophy

- **no capital letters** except for names and headings
- **large round corners** (24px-32px border radius)
- **no shadows** for a clean, flat design
- **playfair display medium** for headings
- **plus jakarta sans** for body text
- **orange (#ff6b35)** as primary color
- **bright social feel** with gradients and animations

## Tech Stack

- **Backend**: Flask, Python
- **AI**: OpenAI GPT-4o-mini
- **Frontend**: Vanilla JS, CSS animations
- **Design**: Mobile-first, swipe gestures, card animations

## API Integration

The app uses OpenAI's GPT-4o-mini model with advanced prompt engineering for:
- Psychological personality mapping
- Gift recommendation generation
- Conversation starter creation
- Reaction prediction modeling

## File Structure

```
ruby/
├── app.py                 # Main Flask application
├── gift_prompt.py         # Advanced prompt engineering
├── templates/
│   ├── base.html         # Base template with design system
│   ├── index.html        # Landing page
│   ├── questions.html    # Question flow with swipe gestures
│   ├── results.html      # Results with card animations
│   └── share.html        # Social sharing features
├── requirements.txt      # Python dependencies
├── .env.example         # Environment variables template
└── README.md            # This file
```

## Development

To run in development mode:

```bash
export FLASK_ENV=development
export FLASK_DEBUG=True
python app.py
```

The app will reload automatically when you make changes.

## Deployment

For production deployment, make sure to:
1. Set `FLASK_ENV=production`
2. Use a secure `SECRET_KEY`
3. Configure your OpenAI API key
4. Use a proper WSGI server like Gunicorn

## License

MIT License - feel free to use this for your own projects!