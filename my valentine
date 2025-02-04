// Cache DOM elements to optimize access
const questionsElement = document.getElementById("questions");
const queElement = document.getElementById("que");
const initElement = document.getElementById("init");
const messageElement = document.getElementById("message");
const messageTextElement = document.getElementById("messageText");

function startQuestions() {
    questionsElement.style.display = "block";
}

function answerYes() {
    showAnswerMessage("peehu peehu! udud udud!");
}

function answerNo() {
    questionsElement.style.display = "block";
    queElement.style.display = "block";
    initElement.innerText = "peehu peehu! udud udud!🎉🎉🎉";
    messageElement.style.display = "block";
    messageTextElement.innerText = "Do you happen to like someone named Jeeva?";
    showHearts();
}

function showAnswerMessage(message) {
    questionsElement.style.display = "none";
    queElement.style.display = "none";
    initElement.innerText = "peehu peehu! 🎉🎉🎉";
    messageElement.style.display = "block";
    messageTextElement.innerText = message;
    showHearts();
}

// Function to show hearts
function showHearts() {
    const heartsSettings = {
        target: 'hearts-canvas',
        respawn: true,
        colors: ['#ff0000', '#ff5e5e', '#ff9d9d', '#ff69b4'],
    };

    try {
        const hearts = new ConfettiGenerator(heartsSettings);
        hearts.render();
        setTimeout(() => {
            hearts.clear();
        }, 5000);
    } catch (error) {
        console.error("Hearts rendering failed: ", error);
    }
}

// New question functions
function askFavoriteColor() {
    showAnswerMessage("What is your favorite color?");
}

function askFavoriteFood() {
    showAnswerMessage("What is your favorite food?");
}

function askHobbies() {
    showAnswerMessage("What are your hobbies?");
}

function askValentine() {
    showAnswerMessage("So, will you be my valentine?");
}

// Set canvas background color to light pink
document.addEventListener("DOMContentLoaded", () => {
    document.getElementById('hearts-canvas').style.backgroundColor = '#ffc0cb';
});
