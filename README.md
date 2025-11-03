# Super Siri

Super Siri is a groundbreaking audio analysis application that helps users manage their tasks and track their personal growth through conversation recording and AI-powered analysis.

## What it Does

SuperSiri takes in audio data and analyzes them to create a set of to-do lists and project tracking for work performance purposes. The audio data is first collected with a wireless mic, and then stored in our database. Using an AI API, it can analyze and develop context for the user, then generate a to-do list based on their needs exhibited from their conversation.

## Features

- **Journal**: AI-written personalized journal to track your life journey
- **Recordings**: Store and replay your past conversations
- **To-Do List**: AI-generated task management based on your conversations
- **Self-Reflection**: Look back on your personal growth and conversations

## Project Setup

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- [Optional] A local web server for development

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/super_siri.git
   cd super_siri
   ```

2. **No build process required!** This is a static HTML/CSS/JavaScript application.

### Running the Application

#### Option 1: Direct File Opening
Simply open `index.html` in your web browser:
- Double-click `index.html`
- Or right-click and select "Open with" → your preferred browser

#### Option 2: Using a Local Server (Recommended)

**Using Python:**
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

**Using Node.js (with npx):**
```bash
npx http-server -p 8000
```

**Using PHP:**
```bash
php -S localhost:8000
```

Then navigate to `http://localhost:8000` in your browser.

### Project Structure

```
super_siri/
├── images/              # Image assets
├── recordings/          # Audio recordings storage
├── index.html           # Main landing page
├── index.js             # Main page scripts
├── index.css            # Main page styles
├── journal.html         # Journal page
├── journal.css          # Journal styles
├── recordings.html      # Recordings page
├── recordings.js        # Recordings functionality
├── recordings.css       # Recordings styles
├── todolist.html        # To-do list page
├── todolist.css         # To-do list styles
├── signin.html          # Sign-in page
├── signin.css           # Sign-in styles
├── bootstrap.min.css    # Bootstrap framework
└── README.md            # This file
```

### Dependencies

All dependencies are loaded via CDN:
- Bootstrap 4.1.3
- jQuery 3.3.1

No manual installation required!

### Audio Files

Place your audio recordings (MP3 format) in the `recordings/` directory. The application will display and allow playback of these files.

## Usage

1. **Home Page**: Start at `index.html` to see an overview of features
2. **Sign In**: Navigate to the sign-in page (authentication not fully implemented)
3. **Journal**: View your AI-generated journal entries
4. **Recordings**: Browse and play your audio recordings
5. **To-Do List**: Check your AI-generated tasks

## How We Built It

### Front End
For the front end of SuperSiri, we used a combination of HTML, CSS, and JavaScript to create a user-friendly interface for interacting with the application. The interface allows users to initiate audio recordings and view the generated to-do lists and project tracking information.

### Back End
The backend of SuperSiri consists of server-side code responsible for processing audio data, analyzing it using AI APIs, and generating the corresponding to-do lists and project tracking information. We used Python along with various libraries and frameworks to build the backend functionality.

### Hardware
A novel approach of connecting a Raspberry PI 0w to a rPI microphone and a LCD screen was successfully implemented to collect audio data. The rPI was connected to an external set of monitor, keyboard and mouse. Although we have the camera attached on the rPI, it was proven that either the rPI cannot handle it, or the camera is too slow for analysis video.

## Challenges We Ran Into

To start off, we did attempt to use a Raspberry Pi 0w for wearable technology for the user to use to make it easy to record. Due to unforeseen circumstances, we missed a few wires that are crucial to a steady connection with the rPi. After overcoming that, we had a lot of problems with performance issues such as program efficiency and latency since the rPi 0w was a minimal computer. We still made it work in the end. Due to these technical difficulties, we had to constantly update our front end. Therefore, as of time of submission, we are still endeavoring to keep a consistent set of front end features.

## What We Learned

After going through a 36 hour hackathon, we've learned a few heartfelt things:

- Don't overstretch your team, allocate sufficient sleep
- Focus on creating the core, minimal viable product
- Don't overengineer basic steps
- Raspberry Pi 0w is a bit slow for most applications
- Don't compete in spicy ramen eating contests

## What's Next?

Super Siri is definitely what we think is one of the greatest projects we made, though there are a few features we would love to get to if we had more time to work on it. A few of these features are:

- Video recordings for further, and more accurate analysis
- AI fitness tracker
- Virtual assistant to help look back on conversations
- Conversations to image journaling
- More sophisticated front end and bot
- Using language data collected, we can implement a voice reconstruction system with generative AI to recreate a person's speech

## License

See [Terms & Conditions](https://www.termsfeed.com/live/53b80ab4-ca57-4e79-bcd1-be8cb3aeaccf) for usage agreement.

## Support

For issues or questions, please open an issue on the GitHub repository.
