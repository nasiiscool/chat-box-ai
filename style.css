:root {
  --bg-deep: #071a2b;
  --bg-mid: #0d2340;
  --panel: rgba(13, 35, 64, 0.8);
  --panel-alt: rgba(17, 42, 70, 0.95);
  --line: rgba(255, 255, 255, 0.08);
  --text: #edf6ff;
  --muted: #a5bdd8;
  --blue: #4ea2ff;
  --blue-strong: #2d7df6;
  --yellow: #ffd54a;
  --yellow-soft: #ffe78e;
  --user-bubble: linear-gradient(135deg, #2d7df6, #1e5fd2);
  --assistant-bubble: rgba(255, 255, 255, 0.06);
  --shadow: rgba(5, 10, 20, 0.5);
}

* {
  box-sizing: border-box;
}

html, body {
  margin: 0;
  min-height: 100%;
  font-family: "Inter", sans-serif;
  background:
    radial-gradient(circle at top left, rgba(255, 213, 74, 0.16), transparent 28%),
    radial-gradient(circle at bottom right, rgba(78, 162, 255, 0.28), transparent 30%),
    linear-gradient(135deg, var(--bg-deep), #0a1d36 40%, #0d2948 100%);
  color: var(--text);
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  padding: 24px;
}

button, input {
  font: inherit;
}

.app-shell {
  width: min(1400px, 100%);
  height: min(92vh, 900px);
  background: rgba(5, 14, 25, 0.4);
  border: 1px solid var(--line);
  border-radius: 28px;
  backdrop-filter: blur(18px);
  box-shadow: 0 40px 80px var(--shadow);
  display: grid;
  grid-template-columns: 290px 1fr;
  overflow: hidden;
}

.sidebar {
  background: rgba(7, 20, 35, 0.75);
  border-right: 1px solid var(--line);
  display: flex;
  flex-direction: column;
  padding: 18px 16px;
}

.brand-wrap {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 8px 8px 18px;
}

.brand-icon {
  width: 36px;
  height: 36px;
  display: grid;
  place-items: center;
  border-radius: 12px;
  background: linear-gradient(135deg, var(--yellow), #ffc84d);
  color: #0a1d36;
  font-weight: 800;
  box-shadow: 0 10px 24px rgba(255, 213, 74, 0.3);
}

.brand-text {
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: -0.04em;
  color: var(--text);
}

.new-chat-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  padding: 14px 16px;
  border: 1px solid rgba(255, 213, 74, 0.45);
  background: linear-gradient(135deg, rgba(255, 213, 74, 0.18), rgba(78, 162, 255, 0.12));
  color: var(--text);
  border-radius: 14px;
  cursor: pointer;
  font-weight: 600;
  transition: transform 0.2s ease, border-color 0.2s ease;
}

.new-chat-btn:hover {
  transform: translateY(-1px);
  border-color: rgba(255, 213, 74, 0.8);
}

.plus {
  color: var(--yellow);
  font-size: 1.1rem;
}

.chat-list {
  margin-top: 18px;
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.chat-item {
  padding: 12px 14px;
  border-radius: 12px;
  color: var(--muted);
  background: transparent;
  border: 1px solid transparent;
  transition: all 0.2s ease;
  font-size: 0.96rem;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}

.chat-item.active {
  background: rgba(78, 162, 255, 0.12);
  border-color: rgba(78, 162, 255, 0.3);
  color: var(--text);
}

.chat-item:hover {
  background: rgba(255, 255, 255, 0.03);
  border-color: rgba(255, 255, 255, 0.06);
}

.sidebar-footer {
  margin-top: auto;
  padding-top: 16px;
  border-top: 1px solid var(--line);
}

.user-card {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 10px 8px;
  border-radius: 12px;
  background: rgba(255, 255, 255, 0.02);
}

.avatar {
  width: 34px;
  height: 34px;
  border-radius: 50%;
  display: grid;
  place-items: center;
  font-size: 0.8rem;
  font-weight: 700;
  background: linear-gradient(135deg, var(--yellow), #ffb703);
  color: #0b1b2a;
}

.user-card strong {
  display: block;
  font-size: 0.93rem;
}

.user-card small {
  color: var(--muted);
}

.chat-panel {
  display: flex;
  flex-direction: column;
  background: rgba(6, 18, 31, 0.4);
}

.topbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 20px 24px 12px;
  border-bottom: 1px solid var(--line);
}

.topbar-left,
.topbar-right {
  display: flex;
  align-items: center;
  gap: 12px;
}

.model-label {
  border: 1px solid rgba(255, 255, 255, 0.08);
  background: rgba(255, 255, 255, 0.03);
  color: var(--text);
  padding: 8px 12px;
  border-radius: 999px;
  font-size: 0.85rem;
  font-weight: 600;
}

.icon-btn {
  width: 38px;
  height: 38px;
  display: grid;
  place-items: center;
  border-radius: 10px;
  border: 1px solid var(--line);
  background: rgba(255, 255, 255, 0.02);
  color: var(--text);
  cursor: pointer;
}

.messages {
  flex: 1;
  overflow-y: auto;
  padding: 26px 28px 16px;
  display: flex;
  flex-direction: column;
  gap: 18px;
}

.message-row {
  display: flex;
  align-items: flex-end;
  gap: 12px;
}

.message-row.user {
  justify-content: flex-end;
}

.assistant-avatar {
  width: 36px;
  height: 36px;
  font-size: 0.72rem;
  background: linear-gradient(135deg, rgba(255, 213, 74, 0.8), rgba(255, 184, 0, 0.85));
  color: #071a2b;
}

.bubble {
  max-width: min(72%, 650px);
  padding: 16px 18px;
  border-radius: 20px;
  line-height: 1.6;
  font-size: 0.98rem;
  letter-spacing: -0.02em;
}

.message-row.assistant .bubble {
  background: var(--assistant-bubble);
  border: 1px solid rgba(255, 255, 255, 0.04);
  color: var(--text);
}

.message-row.user .bubble {
  background: var(--user-bubble);
  color: white;
  box-shadow: 0 16px 36px rgba(54, 122, 255, 0.45);
}

.composer {
  display: flex;
  align-items: center;
  gap: 12px;
  padding: 20px 24px 24px;
  border-top: 1px solid var(--line);
  background: rgba(10, 22, 37, 0.42);
}

.tool-btn {
  width: 42px;
  height: 42px;
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 12px;
  background: rgba(255, 255, 255, 0.03);
  color: var(--yellow);
  cursor: pointer;
  font-size: 1.1rem;
}

#user-input {
  flex: 1;
  height: 52px;
  border-radius: 16px;
  border: 1px solid rgba(255, 255, 255, 0.08);
  background: rgba(255, 255, 255, 0.03);
  color: var(--text);
  padding: 0 18px;
  font-size: 1rem;
  outline: none;
}

#user-input::placeholder {
  color: var(--muted);
}

#user-input:focus {
  border-color: rgba(255, 213, 74, 0.45);
  box-shadow: 0 0 0 3px rgba(255, 213, 74, 0.12);
}

.send-btn {
  height: 52px;
  padding: 0 22px;
  border: none;
  border-radius: 16px;
  background: linear-gradient(135deg, var(--yellow), #ffc94d);
  color: #091c2d;
  font-weight: 800;
  cursor: pointer;
  box-shadow: 0 14px 28px rgba(255, 213, 74, 0.28);
}

@media (max-width: 900px) {
  .app-shell {
    grid-template-columns: 1fr;
    height: auto;
  }

  .sidebar {
    border-right: none;
    border-bottom: 1px solid var(--line);
  }

  .messages {
    padding: 20px 18px 12px;
  }

  .bubble {
    max-width: 85%;
  }
}

@media (max-width: 520px) {
  body {
    padding: 12px;
  }

  .topbar,
  .composer {
    padding-left: 14px;
    padding-right: 14px;
  }

  .composer {
    gap: 8px;
  }

  .send-btn {
    padding: 0 14px;
  }
}
