// ULTRA FAST Auto Clicker with On/Off Switch
let clicking = false;
let clickInterval;

// Toggle function
window.toggleClicker = function() {
    clicking = !clicking;
    
    if (clicking) {
        console.log("🔥 AUTO CLICKER ON - MAX SPEED");
        clickInterval = setInterval(() => {
            document.elementFromPoint(mouseX, mouseY)?.click();
        }, 1); // 1ms = 1000 clicks per second
    } else {
        console.log("⏸️ AUTO CLICKER OFF");
        clearInterval(clickInterval);
    }
}

// Track mouse position
let mouseX = 0;
let mouseY = 0;
document.addEventListener('mousemove', (e) => {
    mouseX = e.clientX;
    mouseY = e.clientY;
});

console.log("✅ Ultra fast auto clicker loaded!");
console.log("Type: toggleClicker() to start/stop");
console.log("Or press Ctrl+Shift+C to toggle");

// Keyboard shortcut (Ctrl+Shift+C)
document.addEventListener('keydown', (e) => {
    if (e.ctrlKey && e.shiftKey && e.key === 'C') {
        toggleClicker();
    }
});

