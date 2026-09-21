Happy Birthday, Kanishka 

A fun and interactive Birthday Greeting Card Website created with HTML, CSS, and JavaScript.
The project presents a colorful animated birthday card for Kanishka, with a flip-card interaction, birthday message, animated balloons, cake illustration, candle flame animation, and a friendship-themed message.

Features
- 🎉 Interactive birthday card with front/back flip animation
- 🎈 Animated floating balloons with randomized positions
- 🎂 Birthday cake illustration
- 🕯️ Animated candle flame
- 💌 Personal birthday message from Tejaswini
- 🌈 Colorful gradient background
- ✨ CSS 3D card-flip effect
- 😂 Funny birthday quote
- 💖 Friendship-themed birthday message
  
🛠️ Technologies Used

Technology	Purpose
HTML5	Page and card structure
CSS3	Styling, gradients, animations, and 3D flip
JavaScript	Card interaction and balloon positioning
External Images/GIFs	Balloons and birthday cake


📁 Project Structure
Birthday-Card/
│
├── index.html
└── README.md
The current project contains HTML, CSS, and JavaScript in a single index.html file.

 Design
The website uses:
- Pink, peach, and cream gradient background
- Yellow/orange card front
- Green card back
- Rounded corners and shadows
- Comic Sans MS typography
- Birthday emojis
- Animated balloons
- Flickering candle flame
  
🔄 How It Works
Open Website
     ↓
Birthday Card Appears
     ↓
Click Card
     ↓
Card Flips
     ↓
Birthday Message + Cake
     ↓
Friendship Message + Quote

Card Flip
JavaScript toggles the open class when the card is clicked:
card.addEventListener('click', () => {
    card.classList.toggle('open');
});
The CSS then rotates the inner card:
#card.open #card-inner {
    transform: rotateY(180deg);
}
🎈 Balloon Animation
The project uses CSS animation for floating balloons. JavaScript also gives each balloon a random horizontal position and animation delay:
balloons.forEach(balloon => {
    balloon.style.left = Math.random() * 100 + '%';
    balloon.style.animationDelay = Math.random() * 3 + 's';
});
🕯️ Candle Flame Animation
The candle flame uses a CSS flicker animation:
@keyframes flicker {
    0%, 100% {
        opacity: 1;
    }

    50% {
        opacity: 0.5;
    }
}
▶️ How to Run
This is a static HTML project, so PHP, MySQL, and a backend server are not required.

Option 1 — Open Directly
1. Save the code as:
index.html
2. Double-click index.html.
3. The birthday card will open in your browser.

Option 2 — VS Code Live Server
1. Open the project folder in VS Code.
2. Install the Live Server extension if required.
3. Right-click index.html.
4. Select Open with Live Server.

Current Code Note
The JavaScript contains:
const messageInput = document.getElementById('messageInput');
and later uses:
messageInput.value
However, the provided HTML does not currently contain an element with:
id="messageInput"
Therefore, the custom message-input feature is not fully connected in the current version.
The birthday card and flip animation can still be used, but an input or textarea should be added if visitors are intended to submit their own messages.

Future Enhancements
- ✍️ Add a birthday message textarea
- 💌 Allow multiple messages
- 🎊 Add confetti animation
- 🎵 Add optional birthday music
- 🎈 Add more balloon effects
- 📸 Add a custom birthday photo
- 🎁 Add an animated gift-opening effect
- 📱 Improve mobile responsiveness
- 🔗 Add a share button
- 📝 Allow the birthday person's name to be customized

Author
Tejaswini Rakhunde
GitHub: Tejaswini-2006

🎂 Happy Birthday, Kanishka! 🎉
