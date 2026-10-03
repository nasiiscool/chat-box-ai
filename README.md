const form = document.getElementById('chat-form');
const input = document.getElementById('user-input');
const messages = document.getElementById('messages');

const quickReplies = [
  'Here’s a clean strategy: start with a bold hero section, a strong benefit statement, and a modern CTA styled with blue and yellow highlights.',
  'I would build a premium aesthetic using a dark navy base, warm yellow accents, and glassy UI cards to make the product feel futuristic.',
  'A great conversion-focused layout includes a headline, trust indicators, a quick feature list, and a clear action button above the fold.',
  'If you want a more advanced launch page, I’d add a feature grid, customer testimonials, and an interactive product mockup section.'
];

function appendMessage(text, sender) {
  const row = document.createElement('div');
  row.className = `message-row ${sender}`;

  if (sender === 'assistant') {
    const avatar = document.createElement('div');
    avatar.className = 'avatar assistant-avatar';
    avatar.textContent = 'AI';
    row.appendChild(avatar);
  }

  const bubble = document.createElement('div');
  bubble.className = 'bubble';
  bubble.textContent = text;
  row.appendChild(bubble);

  messages.appendChild(row);
  messages.scrollTop = messages.scrollHeight;
}

function getAssistantReply(prompt) {
  const lower = prompt.toLowerCase();

  if (lower.includes('design') || lower.includes('website')) {
    return 'A premium website should focus on clarity, trust, and bold contrast. Use a deep blue theme, yellow highlights, crisp copy, and simple navigation to keep the brand memorable.';
  }

  if (lower.includes('brand') || lower.includes('logo')) {
    return 'For a strong AI brand, use a confident typeface, minimal symbols, and a memorable color contrast. Blue conveys intelligence, and yellow adds optimism and energy.';
  }

  if (lower.includes('marketing') || lower.includes('plan')) {
    return 'I’d create a launch plan with a clear value proposition, 3 key differentiators, a short funnel, and a social proof section to build trust quickly.';
  }

  return quickReplies[Math.floor(Math.random() * quickReplies.length)];
}

form.addEventListener('submit', (event) => {
  event.preventDefault();

  const value = input.value.trim();
  if (!value) return;

  appendMessage(value, 'user');
  input.value = '';

  setTimeout(() => {
    appendMessage(getAssistantReply(value), 'assistant');
  }, 500);
});

const newChatBtn = document.querySelector('.new-chat-btn');
newChatBtn.addEventListener('click', () => {
  const confirmClear = confirm('Start a new chat?');
  if (confirmClear) {
    messages.innerHTML = `
      <div class="message-row assistant">
        <div class="avatar assistant-avatar">AI</div>
        <div class="bubble">
          New chat started. What would you like to build next?
        </div>
      </div>
    `;
  }
});

input.focus();

