* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

:root {
  --background: #f5f7fb;
  --white: #ffffff;
  --text: #172033;
  --muted: #7b8496;
  --border: #e7eaf0;
  --purple: #5b4bdb;
  --purple-light: #ece9ff;
  --green: #20a463;
}

body {
  min-height: 100vh;

  font-family:
    Arial,
    Helvetica,
    sans-serif;

  background: var(--background);
  color: var(--text);
}


/* MAIN APP */

.app {
  width: 1200px;
  max-width: 95%;

  height: 90vh;

  margin: 5vh auto;

  display: flex;

  background: white;

  border: 1px solid var(--border);

  border-radius: 24px;

  overflow: hidden;

  box-shadow:
    0 20px 60px rgba(30, 30, 70, 0.12);
}


/* SIDEBAR */

.sidebar {
  width: 350px;

  padding: 22px;

  background: #fbfbfe;

  border-right: 1px solid var(--border);
}


/* BRAND */

.brand {
  display: flex;

  align-items: center;

  gap: 12px;

  margin-bottom: 22px;
}

.brand img {
  width: 52px;
  height: 52px;

  object-fit: contain;

  border-radius: 12px;
}

.brand h1 {
  font-size: 21px;
}

.brand p {
  margin-top: 4px;

  color: var(--muted);

  font-size: 12px;
}


/* MY PROFILE */

.my-profile {
  display: flex;

  align-items: center;

  gap: 12px;

  padding: 14px;

  margin-bottom: 18px;

  border-radius: 16px;

  background: #efedff;
}

.my-profile small {
  display: block;

  margin-top: 4px;

  color: var(--green);

  font-size: 12px;
}


/* AVATAR */

.avatar {
  width: 46px;
  height: 46px;

  flex-shrink: 0;

  display: flex;

  align-items: center;
  justify-content: center;

  border-radius: 50%;

  background:
    linear-gradient(
      135deg,
      #7969ed,
      #4434bd
    );

  color: white;

  font-weight: bold;

  font-size: 17px;
}

.my-avatar {
  background: #252b3c;
}


/* SEARCH */

.search-box input {
  width: 100%;

  padding: 13px 15px;

  border: 1px solid var(--border);

  border-radius: 13px;

  outline: none;

  background: white;

  font-size: 14px;
}

.search-box input:focus {
  border-color: #a9a0ff;

  box-shadow:
    0 0 0 3px #eeeaff;
}


/* CHAT TITLE */

.chat-title {
  margin:

    23px 5px 10px;

  color: var(--muted);

  font-size: 12px;

  font-weight: bold;

  letter-spacing: 1px;
}


/* CHAT ITEM */

.chat-item {
  width: 100%;

  display: flex;

  align-items: center;

  gap: 11px;

  padding: 11px;

  margin-bottom: 7px;

  border: 0;

  border-radius: 14px;

  background: transparent;

  cursor: pointer;

  text-align: left;
}

.chat-item:hover,
.chat-item.active {
  background: var(--purple-light);
}

.chat-info {
  flex: 1;

  min-width: 0;
}

.chat-info strong {
  display: block;

  margin-bottom: 4px;
}

.chat-info small {
  color: var(--muted);

  font-size: 12px;
}

.chat-time {
  color: var(--muted);

  font-size: 11px;
}


/* CHAT WINDOW */

.chat-window {
  flex: 1;

  min-width: 0;

  display: flex;

  flex-direction: column;

  background: #f8f9fd;
}


/* HEADER */

.chat-header {
  height: 86px;

  display: flex;

  align-items: center;

  justify-content: space-between;

  padding: 17px 24px;

  background: white;

  border-bottom: 1px solid var(--border);
}

.person {
  display: flex;

  align-items: center;

  gap: 12px;
}

.person h2 {
  font-size: 18px;
}

.person p {
  margin-top: 4px;

  color: var(--green);

  font-size: 12px;
}

.header-buttons {
  display: flex;

  gap: 8px;
}

.header-buttons button {
  width: 40px;
  height: 40px;

  border: 0;

  border-radius: 12px;

  background: #f1f2f7;

  cursor: pointer;

  font-size: 17px;
}


/* MESSAGES */

.messages {
  flex: 1;

  overflow-y: auto;

  padding: 25px 7%;

  background:

    radial-gradient(
      circle,
      rgba(91, 75, 219, 0.035) 2px,
      transparent 3px
    );

  background-size: 40px 40px;
}


/* DATE */

.date {
  width: max-content;

  margin: 0 auto 22px;

  padding: 6px 13px;

  border-radius: 20px;

  background: #e8eaf0;

  color: var(--muted);

  font-size: 11px;
}


/* MESSAGE */

.message {
  max-width: 70%;

  display: flex;

  flex-direction: column;

  margin: 11px 0;
}

.message.sent {
  margin-left: auto;

  align-items: flex-end;
}

.message.received {
  align-items: flex-start;
}


/* BUBBLE */

.bubble {
  padding: 11px 15px;

  border-radius: 17px;

  line-height: 1.45;

  box-shadow:
    0 2px 8px rgba(20, 20, 40, 0.04);
}

.received .bubble {
  background: white;

  border: 1px solid var(--border);

  border-bottom-left-radius: 5px;
}

.sent .bubble {
  background: var(--purple-light);

  border-bottom-right-radius: 5px;
}

.message > span {
  margin: 4px 6px 0;

  color: var(--muted);

  font-size: 10px;
}


/* MESSAGE FORM */

.message-form {
  display: flex;

  align-items: center;

  gap: 10px;

  padding: 14px 20px;

  background: white;

  border-top: 1px solid var(--border);
}

.message-form input {
  flex: 1;

  min-width: 0;

  padding: 13px 15px;

  border: 1px solid var(--border);

  border-radius: 15px;

  outline: none;

  background: #f7f8fb;
}

.message-form input:focus {
  border-color: #aaa0ff;

  box-shadow:
    0 0 0 3px #eeeaff;
}

.emoji-button,
.send-button {
  width: 46px;
  height: 46px;

  border: 0;

  border-radius: 14px;

  cursor: pointer;
}

.emoji-button {
  background: #f0f1f6;

  font-size: 19px;
}

.send-button {
  background: var(--purple);

  color: white;

  font-size: 20px;
}

.send-button:hover {
  background: #4938c5;
}


/* MOBILE */

@media (max-width: 760px) {

  .app {
    width: 100%;
    max-width: 100%;

    height: 100vh;

    margin: 0;

    border: 0;

    border-radius: 0;
  }

  .sidebar {
    width: 82px;

    padding: 10px 7px;
  }

  .brand div,
  .my-profile div:not(.avatar),
  .search-box,
  .chat-title,
  .chat-info,
  .chat-time {
    display: none;
  }

  .brand,
  .my-profile,
  .chat-item {
    justify-content: center;
  }

  .brand img {
    width: 48px;
    height: 48px;
  }

  .my-profile {
    padding: 8px;

    background: transparent;
  }

  .chat-item {
    padding: 8px;
  }

  .messages {
    padding: 20px 13px;
  }

  .message {
    max-width: 85%;
  }

  .chat-header {
    padding: 13px 14px;
  }
}
