# LegenMusic 🧘‍♂️✨

LegenMusic is an interactive, modern music therapy web application designed to serve as a digital sanctuary of healing sounds. Built with a responsive, glassmorphic layout inspired by leading audio platforms like Spotify and Audiomack, the site serves a unique therapeutic purpose: aligning biological and neurological frequencies to reduce anxiety, promote mental clarity, and facilitate deep rest.

Developed in collaboration with clinical mental health insights from **Confivent Therapy** (Accra, Ghana), the platform bridges the gap between sound technology and psychological wellness.

---

## 🎨 Design & Aesthetic Philosophy
- **Midnight Serenity Theme:** A dark, ultra-sleek visual experience using deep obsidian backgrounds (`#050814`) paired with calming eucalyptus greens, soft lavender, and oceanic teals.
- **Micro-Interactions & Glassmorphism:** Semi-transparent structural cards with heavy background blur effects (`backdrop-filter`) and gentle glow borders that reduce cognitive overload.
- **Dynamic Equalizer & Audio State:** Fully animated CSS audio frequency waves sync with the playback engine to provide comforting visual feedback.

---

## ⚡ Key Features
- **HTML5 Streaming Audio Engine:** Powered natively by the browser's audio clock to handle play, pause, sequential track playing, and real-time progress seeking.
- **Frequency & Mood Selector:** Instantly filters the active playlist based on specific mental wellness states: *Anxiety Relief*, *Mental Clarity*, *Deep Rest*, or *Uplifting*.
- **Integrated Support Systems:**
  - Direct request workflows for Bespoke Psychological Soundscapes.
  - Dedicated clinical consultation paths routed through **Confivent Therapy**.
  - One-click portals for listener-supported mission funding.

---

## 🛠️ Technology Stack
- **HTML5:** Semantic markup structure.
- **Tailwind CSS (via CDN):** Responsive layout utility framework.
- **Vanilla JavaScript:** Event-driven state management and browser media playback.
- **Typography:** *Syne* (for expressive headlines) and *Plus Jakarta Sans* (for optimal screen legibility).

---

## 🚀 Deployment

### Run Locally
1. Clone this repository or download the files.
2. Open the `index.html` file in any modern web browser.

### Hosting on GitHub Pages
1. Go to repository **Settings** > **Pages** in the left sidebar.
2. Under **Build and deployment**, set the source to **Deploy from a branch**.
3. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. Within minutes, your site will be live at `https://<your-username>.github.io/<your-repo-name>/`.

### Hosting on Netlify (For custom domain legenmusic.com)
1. Log in to your Netlify dashboard.
2. Drag and drop the folder containing your `index.html` file into the deployment zone.
3. Once deployed, add your custom domain `legenmusic.com` under **Domain Management**.

---

## 🎵 Customizing Your Tracks
To update or change the audio files to your own therapeutic productions, open `index.html` and locate the `database` array inside the `<script>` tag at the bottom. 

Update the metadata and replace the `src` values with direct links to your hosted `.mp3` files (e.g., direct download URLs from cloud hosts, CDNs, or file storage networks):

```javascript
const database = [
  {
    id: 1,
    title: "Your New Track Name",
    artist: "Legen Muzic",
    mood: "Anxiety Relief", // Options: "Anxiety Relief", "Mental Clarity", "Deep Rest", "Uplifting"
    album: "Healing Album",
    emoji: "🌊",
    duration: "04:12",
    link: "https://www.legenmusic.com/your-custom-page",
    src: "https://yourdomain.com/path-to-your-audio.mp3" // Swap with your live .mp3 link
  },
  // Add or update additional tracks here...
];
