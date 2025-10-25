<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GlowBet - Wingo Game</title>
  
  <!-- Firebase SDKs -->
  <script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/9.22.0/firebase-database-compat.js"></script>
  
  <style>
    * { 
      margin: 0; 
      padding: 0; 
      box-sizing: border-box; 
      font-family: 'Poppins', sans-serif; 
    }
    
    /* Common Green Theme */
    body {
      background: linear-gradient(135deg, #00b09b, #96c93d);
      color: #333;
    }
    
    /* Customer Support Button - Bottom Right, MOVED UP */
    .customer-support {
      position: fixed;
      bottom: 100px;
      right: 20px;
      background: linear-gradient(135deg, #00a86b, #00c853);
      color: white;
      width: 60px;
      height: 60px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 28px;
      cursor: pointer;
      box-shadow: 0 8px 20px rgba(0, 168, 107, 0.4);
      z-index: 10000;
      transition: all 0.3s;
      animation: pulse 2s infinite;
    }
    
    .customer-support:hover {
      transform: scale(1.1);
      box-shadow: 0 12px 30px rgba(0, 168, 107, 0.6);
    }
    
    @keyframes pulse {
      0%, 100% {
        box-shadow: 0 8px 20px rgba(0, 168, 107, 0.4);
      }
      50% {
        box-shadow: 0 8px 30px rgba(0, 168, 107, 0.7);
      }
    }
    
    /* Login Page Styles */
    .login-page {
      background: linear-gradient(135deg, #00b09b, #96c93d);
      color: #333; 
      display: flex; 
      justify-content: center; 
      align-items: center; 
      height: 100vh;
      padding: 20px;
    }
    
    .container { 
      width: 380px; 
      background: rgba(255, 255, 255, 0.95); 
      border-radius: 15px; 
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2); 
      padding: 30px; 
      backdrop-filter: blur(10px);
      border: 1px solid rgba(255, 255, 255, 0.3);
    }
    
    .logo { 
      text-align: center; 
      margin-bottom: 20px; 
    }
    
    .logo h2 { 
      color: #00a86b; 
      letter-spacing: 1px; 
      font-size: 28px;
      text-shadow: 0 2px 5px rgba(0, 168, 107, 0.3);
    }
    
    h3 { 
      text-align: center; 
      color: #00a86b; 
      margin-bottom: 20px; 
      font-size: 22px;
      font-weight: 600;
    }
    
    label { 
      display: block; 
      font-size: 14px; 
      margin: 12px 0 6px; 
      color: #555; 
      font-weight: 500;
    }
    
    input[type="text"], input[type="password"], input[type="tel"], input[type="number"] {
      width: 100%; 
      padding: 12px 15px; 
      border: 2px solid #e0e0e0;
      border-radius: 10px; 
      font-size: 14px; 
      outline: none;
      transition: all 0.3s ease;
      background: #f8fff8;
    }
    
    input:focus { 
      border-color: #00a86b; 
      box-shadow: 0 0 10px rgba(0, 168, 107, 0.3); 
      background: #ffffff;
      transform: translateY(-2px);
    }
    
    .checkbox { 
      display: flex; 
      align-items: center; 
      font-size: 13px; 
      margin-top: 15px; 
      color: #555;
    }
    
    .checkbox input { 
      margin-right: 8px; 
      accent-color: #00a86b;
    }
    
    .auth-button {
      width: 100%; 
      background: linear-gradient(135deg, #00a86b, #00c853);
      color: white; 
      border: none;
      padding: 14px; 
      border-radius: 10px; 
      margin-top: 20px;
      font-size: 16px; 
      cursor: pointer; 
      transition: all 0.3s ease;
      font-weight: 600;
      letter-spacing: 0.5px;
      box-shadow: 0 4px 15px rgba(0, 168, 107, 0.4);
    }
    
    .auth-button:hover { 
      background: linear-gradient(135deg, #00915c, #00b347);
      transform: translateY(-3px);
      box-shadow: 0 6px 20px rgba(0, 168, 107, 0.6);
    }
    
    .toggle-link {
      text-align: center; 
      margin-top: 20px; 
      font-size: 14px;
      color: #666;
    }
    
    .toggle-link span { 
      color: #00a86b; 
      cursor: pointer; 
      font-weight: 600;
      text-decoration: underline;
      transition: all 0.3s ease;
    }
    
    .toggle-link span:hover {
      color: #007a4f;
      text-shadow: 0 2px 5px rgba(0, 168, 107, 0.3);
    }
    
    .hidden { display: none; }

    /* Ban Message Styles */
    .ban-message {
      background: #ff4444;
      color: white;
      padding: 15px 20px;
      border-radius: 10px;
      margin: 15px 0;
      text-align: center;
      font-weight: 600;
      box-shadow: 0 4px 15px rgba(255, 68, 68, 0.4);
    }

    .ban-icon {
      font-size: 48px;
      margin-bottom: 10px;
    }

    .suspend-message {
      background: #ff9800;
      color: white;
      padding: 15px 20px;
      border-radius: 10px;
      margin: 15px 0;
      text-align: center;
      font-weight: 600;
      box-shadow: 0 4px 15px rgba(255, 152, 0, 0.4);
    }
    
    /* Home Page Styles */
    .home-page {
      display: none;
      background: linear-gradient(135deg, #00b09b, #96c93d);
      color: #333;
      min-height: 100vh;
      padding-bottom: 80px;
    }

    .banner {
      background: linear-gradient(90deg, #00a86b, #00c853, #00a86b);
      padding: 15px 0;
      text-align: center;
      font-size: 2rem;
      font-weight: bold;
      margin-bottom: 20px;
      color: white;
    }

    .games-container {
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 15px;
      padding: 20px;
    }

    .game-option {
      width: 200px;
      height: 200px;
      background: rgba(255, 255, 255, 0.95);
      border-radius: 50%;
      padding: 20px;
      text-align: center;
      cursor: pointer;
      transition: 0.3s;
      border: 2px solid transparent;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
    }

    .game-option:hover {
      border-color: #00a86b;
      transform: translateY(-5px);
      box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
    }

    .game-image {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      margin-bottom: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      color: white;
    }

    .lottery-image {
      background: linear-gradient(45deg, #ff0000, #ff6b00, #ffd700, #00ff00, #0000ff, #8a2be2);
    }

    .wingo-image {
      background: linear-gradient(135deg, #00a86b, #00c853);
    }

    .game-title {
      font-size: 1.2rem;
      font-weight: bold;
      margin-bottom: 5px;
      color: #00a86b;
    }

    /* Bottom Navigation */
    .bottom-nav {
      position: fixed;
      bottom: 0;
      left: 0;
      right: 0;
      background: rgba(255, 255, 255, 0.95);
      display: flex;
      justify-content: space-around;
      padding: 15px 0;
      border-top: 2px solid #00a86b;
      box-shadow: 0 -5px 20px rgba(0, 0, 0, 0.1);
    }

    .nav-item {
      text-align: center;
      cursor: pointer;
      transition: 0.3s;
      color: #666;
    }

    .nav-item.active {
      color: #00a86b;
    }

    .nav-icon {
      font-size: 1.5rem;
      margin-bottom: 5px;
    }

    /* Back Button */
    .back-button {
      position: absolute;
      top: 20px;
      left: 20px;
      background: #00a86b;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 14px;
      display: flex;
      align-items: center;
      gap: 5px;
      box-shadow: 0 4px 15px rgba(0, 168, 107, 0.3);
      z-index: 100;
    }

    /* Wingo Game Page */
    .wingo-page {
      display: none;
      background: linear-gradient(135deg, #00b09b, #96c93d);
      color: #333;
      min-height: 100vh;
      padding: 20px;
      padding-bottom: 80px;
    }

    .wingo-header {
      text-align: center;
      margin-bottom: 20px;
      margin-top: 40px;
    }

    .wingo-title {
      font-size: 2rem;
      font-weight: bold;
      color: #00a86b;
      margin-bottom: 10px;
    }

    .balance-section {
      background: rgba(255, 255, 255, 0.95);
      padding: 15px;
      border-radius: 10px;
      text-align: center;
      margin-bottom: 20px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
    }

    .balance-amount {
      font-size: 1.5rem;
      font-weight: bold;
      color: #00a86b;
    }

    .refresh-btn {
      background: #00a86b;
      color: white;
      border: none;
      padding: 5px 10px;
      border-radius: 5px;
      cursor: pointer;
      margin-left: 10px;
    }

    .wallet-actions {
      display: flex;
      justify-content: space-between;
      margin-bottom: 20px;
    }

    .wallet-btn {
      background: rgba(255, 255, 255, 0.95);
      padding: 10px 20px;
      border-radius: 10px;
      text-align: center;
      cursor: pointer;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
      flex: 1;
      margin: 0 5px;
      font-weight: 600;
      color: #00a86b;
    }

    .timer-section {
      background: rgba(255, 255, 255, 0.95);
      padding: 15px;
      border-radius: 10px;
      text-align: center;
      margin-bottom: 20px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
    }

    .round-info {
      display: flex;
      justify-content: space-between;
      margin-bottom: 10px;
    }

    .timer {
      font-size: 1.5rem;
      font-weight: bold;
      color: #ff6b00;
    }

    .timer.locked {
      color: #ff4444;
    }

    .betting-area {
      background: rgba(255, 255, 255, 0.95);
      padding: 20px;
      border-radius: 10px;
      margin-bottom: 20px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
      position: relative;
    }

    .betting-area.locked::after {
      content: '🔒 Betting Locked';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(255, 68, 68, 0.9);
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1.5rem;
      font-weight: bold;
      border-radius: 10px;
      z-index: 10;
    }

    .color-options {
      display: flex;
      justify-content: space-around;
      margin-bottom: 20px;
    }

    .color-option {
      padding: 10px 20px;
      border-radius: 20px;
      color: white;
      font-weight: bold;
      cursor: pointer;
      text-align: center;
      flex: 1;
      margin: 0 5px;
      transition: 0.3s;
    }

    .color-option:hover {
      transform: scale(1.05);
    }

    .color-option.disabled {
      opacity: 0.5;
      cursor: not-allowed;
      pointer-events: none;
    }

    .red { background: #ff4444; }
    .violet { background: #8a2be2; }
    .green { background: #00a86b; }

    .number-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 10px;
      margin-bottom: 20px;
    }

    .number-cell {
      background: #f0f0f0;
      padding: 15px;
      border-radius: 10px;
      text-align: center;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
      font-size: 1.2rem;
    }

    .number-cell:hover {
      transform: scale(1.05);
    }

    .number-cell.disabled {
      opacity: 0.5;
      cursor: not-allowed;
      pointer-events: none;
    }

    .number-0 { 
      background: linear-gradient(45deg, #ff4444, #8a2be2);
      color: white;
    }
    .number-1, .number-3, .number-7, .number-9 { 
      background: #00a86b;
      color: white;
    }
    .number-2, .number-4, .number-6, .number-8 { 
      background: #ff4444;
      color: white;
    }
    .number-5 { 
      background: linear-gradient(45deg, #00a86b, #8a2be2);
      color: white;
    }

    .size-options {
      display: flex;
      justify-content: space-around;
      margin-top: 20px;
    }

    .size-option {
      background: #f0f0f0;
      padding: 15px 30px;
      border-radius: 10px;
      text-align: center;
      cursor: pointer;
      font-weight: bold;
      transition: 0.3s;
      flex: 1;
      margin: 0 5px;
      color: white;
      font-size: 1.1rem;
    }

    .size-option.small-btn {
      background: #1E90FF;
    }

    .size-option.big-btn {
      background: #FFD700;
    }

    .size-option:hover {
      transform: scale(1.05);
      opacity: 0.9;
    }

    .size-option.disabled {
      opacity: 0.5;
      cursor: not-allowed;
      pointer-events: none;
    }

    .history-tabs {
      display: flex;
      background: rgba(255, 255, 255, 0.95);
      border-radius: 10px 10px 0 0;
      overflow: hidden;
    }

    .history-tab {
      flex: 1;
      padding: 15px;
      text-align: center;
      cursor: pointer;
      background: #e0e0e0;
      transition: 0.3s;
    }

    .history-tab.active {
      background: #00a86b;
      color: white;
    }

    .history-content {
      background: rgba(255, 255, 255, 0.95);
      border-radius: 0 0 10px 10px;
      padding: 15px;
      max-height: 500px;
      overflow-y: auto;
    }

    .history-table {
      width: 100%;
      border-collapse: collapse;
    }

    .history-table th,
    .history-table td {
      padding: 12px 8px;
      text-align: center;
      border-bottom: 1px solid #e0e0e0;
    }

    .history-table th {
      background: #00a86b;
      color: white;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    /* Colorful Result Display */
    .result-number {
      font-weight: bold;
      font-size: 1.1rem;
      display: inline-block;
      padding: 5px 10px;
      border-radius: 5px;
    }

    .result-number-0 { 
      background: linear-gradient(45deg, #ff4444, #8a2be2);
      color: white;
    }
    .result-number-1, .result-number-3, .result-number-7, .result-number-9 { 
      background: #00a86b;
      color: white;
    }
    .result-number-2, .result-number-4, .result-number-6, .result-number-8 { 
      background: #ff4444;
      color: white;
    }
    .result-number-5 { 
      background: linear-gradient(45deg, #00a86b, #8a2be2);
      color: white;
    }

    .result-colors {
      font-size: 1.5rem;
    }

    /* Pagination Controls */
    .pagination-controls {
      display: flex;
      justify-content: center;
      align-items: center;
      margin-top: 15px;
      gap: 15px;
    }

    .page-btn {
      background: #00a86b;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
      transition: 0.3s;
      display: flex;
      align-items: center;
      gap: 5px;
    }

    .page-btn:hover {
      background: #007a4f;
      transform: scale(1.05);
    }

    .page-btn:disabled {
      background: #ccc;
      cursor: not-allowed;
      transform: scale(1);
    }

    .page-info {
      font-weight: bold;
      color: #00a86b;
      font-size: 14px;
    }

    /* Bet Popup */
    .bet-popup {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.7);
      z-index: 1000;
      justify-content: center;
      align-items: center;
    }

    .bet-popup-content {
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      max-width: 400px;
      width: 90%;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
    }

    .bet-amount {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 15px;
      margin: 20px 0;
    }

    .amount-btn {
      background: #00a86b;
      color: white;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1.2rem;
    }

    .amount-display {
      font-size: 1.5rem;
      font-weight: bold;
      color: #00a86b;
      min-width: 100px;
      padding: 10px;
      border: 2px solid #00a86b;
      border-radius: 8px;
      cursor: pointer;
      background: #f0f0f0;
    }

    .amount-display:hover {
      background: #e0e0e0;
    }

    .multiplier-options {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
      margin: 20px 0;
    }

    .multiplier-btn {
      background: #e0e0e0;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      transition: 0.3s;
    }

    .multiplier-btn.active {
      background: #00a86b;
      color: white;
    }

    .bet-actions {
      display: flex;
      gap: 10px;
      margin-top: 20px;
    }

    .bet-action-btn {
      flex: 1;
      padding: 12px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
    }

    .cancel-btn {
      background: #ff4444;
      color: white;
    }

    .place-bet-btn {
      background: #00a86b;
      color: white;
    }

    /* Result Popup */
    .result-popup {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.7);
      z-index: 1000;
      justify-content: center;
      align-items: center;
    }

    .result-popup-content {
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      max-width: 400px;
      width: 90%;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
    }

    .result-icon {
      font-size: 4rem;
      margin-bottom: 15px;
    }

    .win { color: #00a86b; }
    .lose { color: #ff4444; }

    /* Custom Success Popup */
    .custom-popup {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.7);
      z-index: 1000;
      justify-content: center;
      align-items: center;
    }

    .custom-popup-content {
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      max-width: 300px;
      width: 90%;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
    }

    .success-icon {
      font-size: 4rem;
      color: #00a86b;
      margin-bottom: 15px;
    }

    .popup-btn {
      background: #00a86b;
      color: white;
      border: none;
      padding: 12px 30px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
      margin-top: 15px;
    }

    /* Wallet, Deposit, Withdrawal Pages */
    .wallet-page, .deposit-page, .withdrawal-page, .account-page, .activity-page, .withdrawal-history-page {
      display: none;
      background: linear-gradient(135deg, #00b09b, #96c93d);
      min-height: 100vh;
      padding: 20px;
      padding-bottom: 80px;
    }

    .wallet-header, .deposit-header, .withdrawal-header, .account-header, .activity-header, .withdrawal-history-header {
      text-align: center;
      margin-top: 50px;
      margin-bottom: 30px;
    }

    .wallet-balance-card, .deposit-form-card, .bank-details-card, .withdrawal-amount-card, 
    .withdrawal-history-card, .profile-card, .account-options, .gift-code-card, .rewards-card {
      background: rgba(255, 255, 255, 0.95);
      border-radius: 15px;
      padding: 25px;
      margin-bottom: 20px;
      box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
    }

    .wallet-balance-value {
      font-size: 2.5rem;
      font-weight: bold;
      color: #00a86b;
      margin-bottom: 20px;
    }

    .wallet-action-button, .submit-btn {
      background: #00a86b;
      color: white;
      border: none;
      padding: 15px;
      border-radius: 10px;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      transition: 0.3s;
      width: 100%;
    }

    .wallet-action-buttons {
      display: flex;
      gap: 15px;
    }

    .wallet-action-button {
      flex: 1;
    }

    .form-group {
      margin-bottom: 20px;
    }

    .form-label {
      display: block;
      font-size: 14px;
      font-weight: 600;
      color: #555;
      margin-bottom: 8px;
    }

    .form-input {
      width: 100%;
      padding: 12px 15px;
      border: 2px solid #e0e0e0;
      border-radius: 10px;
      font-size: 14px;
      outline: none;
      transition: all 0.3s ease;
    }

    .form-input:focus {
      border-color: #00a86b;
      box-shadow: 0 0 10px rgba(0, 168, 107, 0.3);
    }

    .qr-code-section {
      text-align: center;
      margin: 30px 0;
      padding: 20px;
      background: white;
      border-radius: 10px;
    }

    .qr-code-image {
      width: 250px;
      height: 250px;
      margin: 20px auto;
      border: 3px solid #00a86b;
      border-radius: 10px;
    }

    .guidelines-section {
      background: #fff3cd;
      border: 2px solid #ffc107;
      border-radius: 10px;
      padding: 15px;
      margin-top: 20px;
    }

    .guidelines-list {
      list-style: none;
      padding-left: 0;
    }

    .guidelines-list li:before {
      content: "✓ ";
      color: #00a86b;
      font-weight: bold;
      margin-right: 5px;
    }

    .profile-avatar {
      width: 100px;
      height: 100px;
      background: linear-gradient(135deg, #00a86b, #00c853);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      margin: 0 auto 20px;
      font-size: 3rem;
      color: white;
    }

    .logout-btn {
      width: 100%;
      background: #ff4444;
      color: white;
      border: none;
      padding: 15px;
      border-radius: 10px;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
      margin-top: 20px;
    }

    .saved-bank-info {
      background: #e8f5e9;
      border: 2px solid #00a86b;
      border-radius: 10px;
      padding: 15px;
      margin-bottom: 20px;
    }

    .bank-info-item {
      display: flex;
      justify-content: space-between;
      padding: 8px 0;
      border-bottom: 1px solid #c8e6c9;
    }

    .gift-code-input-group {
      display: flex;
      gap: 10px;
      margin-bottom: 15px;
    }

    .gift-code-input {
      flex: 1;
    }

    .claim-btn {
      background: #00a86b;
      color: white;
      border: none;
      padding: 12px 25px;
      border-radius: 8px;
      font-weight: 600;
      cursor: pointer;
    }

    .reward-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px;
      background: #f5f5f5;
      border-radius: 10px;
      margin-bottom: 10px;
    }

    .account-option-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px;
      border-bottom: 1px solid #e0e0e0;
      cursor: pointer;
    }

    .wallet-history-item, .withdrawal-item {
      display: flex;
      justify-content: space-between;
      padding: 15px;
      border-bottom: 1px solid #e0e0e0;
    }

    .status-badge {
      padding: 5px 10px;
      border-radius: 5px;
      font-size: 12px;
      font-weight: 600;
    }

    .status-pending {
      background: #fff3cd;
      color: #856404;
    }

    .status-completed {
      background: #d1e7dd;
      color: #0f5132;
    }

    .user-id-display {
      background: #e8f5e9;
      padding: 10px;
      border-radius: 8px;
      margin-top: 10px;
      font-size: 14px;
      color: #333;
    }

    /* Custom Amount Modal */
    .custom-amount-modal {
      display: none;
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.7);
      z-index: 2000;
      justify-content: center;
      align-items: center;
    }

    .custom-amount-content {
      background: white;
      padding: 30px;
      border-radius: 15px;
      text-align: center;
      max-width: 350px;
      width: 90%;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.3);
    }

    .custom-amount-input {
      width: 100%;
      padding: 15px;
      font-size: 1.5rem;
      text-align: center;
      border: 2px solid #00a86b;
      border-radius: 10px;
      margin: 20px 0;
      outline: none;
    }

    .custom-amount-actions {
      display: flex;
      gap: 10px;
      margin-top: 15px;
    }

    .custom-amount-btn {
      flex: 1;
      padding: 12px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-weight: bold;
      font-size: 16px;
    }

    .bet-info-row {
      display: flex;
      justify-content: space-between;
      margin: 10px 0;
      padding: 10px;
      background: #f0f0f0;
      border-radius: 8px;
    }

    /* Withdrawal History Specific Styles */
    .withdrawal-detail-card {
      background: white;
      border-radius: 10px;
      padding: 20px;
      margin-bottom: 15px;
      box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
      border-left: 4px solid #00a86b;
    }

    .detail-row {
      display: flex;
      justify-content: space-between;
      padding: 10px 0;
      border-bottom: 1px solid #f0f0f0;
    }

    .detail-row:last-child {
      border-bottom: none;
    }

    .detail-label {
      font-weight: 600;
      color: #666;
    }

    .detail-value {
      color: #333;
      font-weight: 500;
    }

    .no-history {
      text-align: center;
      padding: 40px 20px;
      color: #666;
    }

    .history-btn {
      background: #ff6b00;
      color: white;
      border: none;
      padding: 12px 20px;
      border-radius: 8px;
      cursor: pointer;
      font-weight: 600;
      margin-top: 15px;
      width: 100%;
    }
  </style>
</head>
<body>

  <!-- Customer Support Button -->
  <a href="https://t.me/GlowBet_support" target="_blank" class="customer-support" title="Customer Support">
    💬
  </a>

  <!-- Login Page -->
  <div class="login-page" id="loginPage">
    <div class="container">
      <div class="logo">
        <h2>🌟 GlowBet</h2>
      </div>

      <!-- LOGIN FORM -->
      <div id="login-form">
        <h3>Welcome Back!</h3>
        <label>Phone number</label>
        <input type="tel" placeholder="+91 Enter your phone number" id="login-phone" />
        
        <label>Password</label>
        <input type="password" placeholder="Enter password" id="login-password" />

        <div class="checkbox">
          <input type="checkbox" id="remember"> <label for="remember">Remember password</label>
        </div>

        <button class="auth-button" onclick="login()">Log in</button>

        <div class="toggle-link">
          Don't have an account? <span onclick="showRegister()">Register Now</span>
        </div>
      </div>

      <!-- REGISTER FORM -->
      <div id="register-form" class="hidden">
        <h3>Join GlowBet!</h3>
        <label>Phone number</label>
        <input type="tel" placeholder="+91 Enter your phone number" id="reg-phone" />

        <label>Set password</label>
        <input type="password" placeholder="Set password" id="reg-pass" />

        <label>Confirm password</label>
        <input type="password" placeholder="Confirm password" id="reg-confirm" />

        <label>Invite code (Optional)</label>
        <input type="text" placeholder="Enter invite code" id="reg-invite" />

        <div class="checkbox">
          <input type="checkbox" id="agree"> <label for="agree">I have read and agree <span style="color:#00a86b; font-weight:600;">[Privacy Agreement]</span></label>
        </div>

        <button class="auth-button" onclick="register()">Create Account</button>

        <div class="toggle-link">
          Already have an account? <span onclick="showLogin()">Log in</span>
        </div>
      </div>
    </div>
  </div>

  <!-- Home Page -->
  <div class="home-page" id="homePage">
    <div class="banner">GLOWBET</div>
    <div class="games-container">
      <div class="game-option" onclick="openLottery()">
        <div class="game-image lottery-image">🎰</div>
        <div class="game-title">LOTTERY</div>
        <p>Win up to ₹50,00,000</p>
      </div>
      <div class="game-option" onclick="openWingo()">
        <div class="game-image wingo-image">🎲</div>
        <div class="game-title">WINGO</div>
        <p>Color & Number Game</p>
      </div>
    </div>
    <div class="bottom-nav">
      <div class="nav-item active" onclick="showHome()">
        <div class="nav-icon">🏠</div>
        <div>HOME</div>
      </div>
      <div class="nav-item" onclick="showActivity()">
        <div class="nav-icon">🎁</div>
        <div>ACTIVITY</div>
      </div>
      <div class="nav-item" onclick="showWallet()">
        <div class="nav-icon">💰</div>
        <div>WALLET</div>
      </div>
      <div class="nav-item" onclick="showAccount()">
        <div class="nav-icon">👤</div>
        <div>ACCOUNT</div>
      </div>
    </div>
  </div>

  <!-- Wingo Game Page -->
  <div class="wingo-page" id="wingoPage">
    <button class="back-button" onclick="goBackToHome()">← Back</button>
    <div class="wingo-header">
      <div class="wingo-title">GlowBet Wingo</div>
    </div>
    <div class="balance-section">
      <div>Wallet Balance</div>
      <div class="balance-amount" id="wingoBalance">₹0.00</div>
      <button class="refresh-btn" onclick="refreshWingoBalance()">🔄</button>
    </div>
    <div class="wallet-actions">
      <div class="wallet-btn" onclick="showWithdrawalPage()">Withdraw</div>
      <div class="wallet-btn" onclick="showDepositPage()">Deposit</div>
    </div>
    <div class="timer-section">
      <div class="round-info">
        <div>Round ID: <span id="currentRoundId">Loading...</span></div>
        <div class="timer" id="countdownTimer">60s</div>
      </div>
      <div>1 Minute Timer</div>
    </div>
    <div class="betting-area" id="bettingArea">
      <div class="color-options">
        <div class="color-option red" onclick="selectBet('red')">RED</div>
        <div class="color-option violet" onclick="selectBet('violet')">VIOLET</div>
        <div class="color-option green" onclick="selectBet('green')">GREEN</div>
      </div>
      <div class="number-grid">
        <div class="number-cell number-0" onclick="selectBet(0)">0</div>
        <div class="number-cell number-1" onclick="selectBet(1)">1</div>
        <div class="number-cell number-2" onclick="selectBet(2)">2</div>
        <div class="number-cell number-3" onclick="selectBet(3)">3</div>
        <div class="number-cell number-4" onclick="selectBet(4)">4</div>
        <div class="number-cell number-5" onclick="selectBet(5)">5</div>
        <div class="number-cell number-6" onclick="selectBet(6)">6</div>
        <div class="number-cell number-7" onclick="selectBet(7)">7</div>
        <div class="number-cell number-8" onclick="selectBet(8)">8</div>
        <div class="number-cell number-9" onclick="selectBet(9)">9</div>
      </div>
      <div class="size-options">
        <div class="size-option small-btn" onclick="selectBet('small')">💙 Small</div>
        <div class="size-option big-btn" onclick="selectBet('big')">⭐ Big</div>
      </div>
    </div>
    <div class="history-section">
      <div class="history-tabs">
        <div class="history-tab active" onclick="showGameHistory()">Game History</div>
        <div class="history-tab" onclick="showMyHistory()">My History</div>
      </div>
      <div class="history-content">
        <table class="history-table" id="historyTable">
          <thead>
            <tr>
              <th>Period</th>
              <th>Number</th>
              <th>Big/Small</th>
              <th>Colour</th>
            </tr>
          </thead>
          <tbody id="historyTableBody">
            <tr>
              <td colspan="4" style="text-align: center; padding: 20px;">Loading results...</td>
            </tr>
          </tbody>
        </table>
        <div class="pagination-controls">
          <button class="page-btn" id="prevPageBtn" onclick="previousPage()" disabled>
            ← Previous
          </button>
          <div class="page-info">
            Page <span id="currentPageNum">1</span> of <span id="totalPagesNum">1</span>
          </div>
          <button class="page-btn" id="nextPageBtn" onclick="nextPage()">
            Next →
          </button>
        </div>
      </div>
    </div>
  </div>

  <!-- Wallet Page -->
  <div class="wallet-page" id="walletPage">
    <button class="back-button" onclick="goBackToHome()">← Back</button>
    <div class="wallet-header">
      <h2 style="color: white; font-size: 2rem;">My Wallet</h2>
    </div>
    <div class="wallet-balance-card">
      <div class="wallet-balance-label">Total Balance</div>
      <div class="wallet-balance-value" id="walletBalance">₹0.00</div>
      <div class="wallet-action-buttons">
        <button class="wallet-action-button" onclick="showDepositPage()">Deposit</button>
        <button class="wallet-action-button" onclick="showWithdrawalPage()">Withdraw</button>
      </div>
    </div>
  </div>

  <!-- Deposit Page -->
  <div class="deposit-page" id="depositPage">
    <button class="back-button" onclick="goBackToWallet()">← Back</button>
    <div class="deposit-header">
      <h2 style="color: white; font-size: 2rem;">Deposit Money</h2>
    </div>
    <div class="deposit-form-card">
      <div class="form-group">
        <label class="form-label">Enter Deposit Amount</label>
        <input type="number" class="form-input" id="depositAmount" placeholder="Minimum ₹80" min="80" />
      </div>
      <button class="submit-btn" onclick="proceedToPayment()">Proceed to Payment</button>
    </div>
    <div class="deposit-form-card" id="paymentSection" style="display: none;">
      <div class="qr-code-section">
        <h3 style="color: #00a86b;">Scan QR Code to Pay</h3>
        <img src="https://page.gensparksite.com/v1/base64_upload/078530ab3aa732ed608eeba4b8bd7b89" alt="Payment QR Code" class="qr-code-image" />
        <p style="margin-top: 10px; color: #666;">Amount: <strong id="displayAmount">₹0</strong></p>
      </div>
      <div class="guidelines-section">
        <div class="guidelines-title">Important Guidelines</div>
        <ul class="guidelines-list">
          <li>Please submit UTR after completing payment</li>
          <li>Payment will be processed within 5-10 minutes</li>
          <li>Keep your UTR number safe for reference</li>
        </ul>
      </div>
      <div class="form-group">
        <label class="form-label">Enter UTR Number</label>
        <input type="text" class="form-input" id="utrNumber" placeholder="Enter 12-digit UTR number" />
      </div>
      <button class="submit-btn" onclick="submitUTR()">Submit UTR</button>
    </div>
  </div>

  <!-- Withdrawal Page -->
  <div class="withdrawal-page" id="withdrawalPage">
    <button class="back-button" onclick="goBackToWallet()">← Back</button>
    <div class="withdrawal-header">
      <h2 style="color: white; font-size: 2rem;">Withdraw Money</h2>
    </div>
    <div class="bank-details-card">
      <h3 style="color: #00a86b; margin-bottom: 20px;">Bank Details</h3>
      <div id="savedBankDetails" style="display: none;">
        <div class="saved-bank-info">
          <div class="bank-info-item">
            <span>Account Number:</span>
            <strong id="savedAccNumber">****</strong>
          </div>
        </div>
        <button class="submit-btn" onclick="editBankDetails()" style="background: #ff6b00;">Edit</button>
      </div>
      <div id="bankDetailsForm">
        <div class="form-group">
          <label class="form-label">Account Number</label>
          <input type="text" class="form-input" id="accNumber" placeholder="Enter account number" />
        </div>
        <div class="form-group">
          <label class="form-label">IFSC Code</label>
          <input type="text" class="form-input" id="ifscCode" placeholder="Enter IFSC code" />
        </div>
        <button class="submit-btn" onclick="saveBankDetails()">Save Bank Details</button>
      </div>
    </div>
    <div class="withdrawal-amount-card">
      <h3 style="color: #00a86b; margin-bottom: 15px;">Withdrawal Amount</h3>
      <div class="form-group">
        <label class="form-label">Enter Withdrawal Amount</label>
        <input type="number" class="form-input" id="withdrawalAmount" placeholder="Minimum ₹100" min="100" />
      </div>
      <button class="submit-btn" onclick="submitWithdrawal()">Request Withdrawal</button>
      <button class="history-btn" onclick="showWithdrawalHistoryPage()">📜 View Withdrawal History</button>
    </div>
  </div>

  <!-- Withdrawal History Page -->
  <div class="withdrawal-history-page" id="withdrawalHistoryPage">
    <button class="back-button" onclick="goBackToWithdrawal()">← Back</button>
    <div class="withdrawal-history-header">
      <h2 style="color: white; font-size: 2rem;">Withdrawal History</h2>
    </div>
    <div class="withdrawal-history-card">
      <div id="withdrawalHistoryContent">
        <div class="no-history">
          <p>Loading withdrawal history...</p>
        </div>
      </div>
    </div>
  </div>

  <!-- Account Page -->
  <div class="account-page" id="accountPage">
    <button class="back-button" onclick="goBackToHome()">← Back</button>
    <div class="account-header">
      <h2 style="color: white; font-size: 2rem;">My Account</h2>
    </div>
    <div class="profile-card">
      <div class="profile-avatar">👤</div>
      <div class="profile-phone" id="profilePhone">+91 **********</div>
      <div class="user-id-display">
        <strong>User ID:</strong> <span id="displayUserId">Loading...</span>
      </div>
    </div>
    <div class="account-options">
      <div class="account-option-item" onclick="showDepositPage()">
        <span>💳 Deposit</span>
        <span>→</span>
      </div>
      <div class="account-option-item" onclick="showWithdrawalPage()">
        <span>💰 Withdrawal</span>
        <span>→</span>
      </div>
    </div>
    <button class="logout-btn" onclick="logout()">Logout</button>
  </div>

  <!-- Activity Page -->
  <div class="activity-page" id="activityPage">
    <button class="back-button" onclick="goBackToHome()">← Back</button>
    <div class="activity-header">
      <h2 style="color: white; font-size: 2rem;">Activities & Rewards</h2>
    </div>
    <div class="gift-code-card">
      <div class="gift-code-title">🎁 Claim Gift Code</div>
      <div class="gift-code-input-group">
        <input type="text" class="form-input gift-code-input" id="giftCodeInput" placeholder="Enter gift code" />
        <button class="claim-btn" onclick="claimGiftCode()">Claim</button>
      </div>
    </div>
    <div class="rewards-card">
      <h3 style="color: #00a86b; margin-bottom: 20px;">Available Rewards</h3>
      <div class="reward-item">
        <div>🎁</div>
        <div style="flex: 1; margin-left: 15px;">
          <div style="font-weight: 600;">Daily Login Bonus</div>
        </div>
        <div style="color: #00a86b; font-weight: bold;">Coming Soon</div>
      </div>
    </div>
  </div>

  <!-- Bet Popup -->
  <div class="bet-popup" id="betPopup">
    <div class="bet-popup-content">
      <h3>Place Your Bet</h3>
      <div id="betSelection" style="font-size: 1.2rem; margin: 10px 0; font-weight: bold; color: #00a86b;">Selected: Red</div>
      <div class="bet-amount">
        <button class="amount-btn" onclick="changeAmount(-10)">-</button>
        <div class="amount-display" id="betAmount" onclick="openCustomAmount()">100</div>
        <button class="amount-btn" onclick="changeAmount(10)">+</button>
      </div>
      <div class="bet-info-row">
        <span>Multiplier:</span>
        <span id="multiplierDisplay" style="font-weight: bold; color: #00a86b;">1.96x</span>
      </div>
      <div class="bet-info-row">
        <span>Potential Win:</span>
        <span id="potentialWin" style="color: #00a86b; font-weight: bold;">₹196</span>
      </div>
      <div class="bet-actions">
        <button class="bet-action-btn cancel-btn" onclick="closeBetPopup()">Cancel</button>
        <button class="bet-action-btn place-bet-btn" onclick="placeBet()">Place Bet</button>
      </div>
    </div>
  </div>

  <!-- Custom Amount Modal -->
  <div class="custom-amount-modal" id="customAmountModal">
    <div class="custom-amount-content">
      <h3 style="color: #00a86b; margin-bottom: 10px;">Enter Custom Amount</h3>
      <input type="number" class="custom-amount-input" id="customAmountInput" placeholder="Enter amount" min="10" />
      <div class="custom-amount-actions">
        <button class="custom-amount-btn cancel-btn" onclick="closeCustomAmount()">Cancel</button>
        <button class="custom-amount-btn place-bet-btn" onclick="applyCustomAmount()">Apply</button>
      </div>
    </div>
  </div>

  <!-- Result Popup -->
  <div class="result-popup" id="resultPopup">
    <div class="result-popup-content">
      <div class="result-icon" id="resultIcon">🏆</div>
      <h3 id="resultTitle">Result</h3>
      <p id="resultMessage">Round completed!</p>
      <button class="popup-btn" onclick="closeResultPopup()">OK</button>
    </div>
  </div>

  <!-- Custom Success Popup -->
  <div class="custom-popup" id="successPopup">
    <div class="custom-popup-content">
      <div class="success-icon">✓</div>
      <h3 id="popupTitle">Success!</h3>
      <p id="popupMessage">Operation completed successfully</p>
      <button class="popup-btn" onclick="closeCustomPopup()">OK</button>
    </div>
  </div>

  <script>
    // ===========================
    // FIREBASE CONFIGURATION
    // ===========================
    const firebaseConfig = {
      apiKey: "AIzaSyCAHzv-VxvatsG9CFsCzbrNx9X6uaKRAa4",
      authDomain: "glowbet-1b2ce.firebaseapp.com",
      databaseURL: "https://glowbet-1b2ce-default-rtdb.firebaseio.com/",
      projectId: "glowbet-1b2ce",
      storageBucket: "glowbet-1b2ce.firebasestorage.app",
      messagingSenderId: "333266810255",
      appId: "1:333266810255:web:877010652ce46c8af687fa",
      measurementId: "G-53QM377N5M"
    };

    // Initialize Firebase
    firebase.initializeApp(firebaseConfig);
    const database = firebase.database();

    // ===========================
    // GLOBAL VARIABLES
    // ===========================
    let currentUser = null;
    let currentBet = null;
    let betAmount = 100;
    let countdown = 60;
    let countdownInterval = null;
    let currentPage = 1;
    const RESULTS_PER_PAGE = 10;
    let allResults = [];
    let isBettingLocked = false;
    let currentRoundId = null;
    let periodStartTime = null;

    // ===========================
    // ⚠️ FIX #1: TIMESTAMP-BASED PERIOD CALCULATION
    // ===========================
    function generateCurrentPeriod() {
      const now = new Date();
      const year = now.getFullYear();
      const month = String(now.getMonth() + 1).padStart(2, '0');
      const day = String(now.getDate()).padStart(2, '0');
      const minutesSinceStart = Math.floor((now.getHours() * 60 + now.getMinutes()));
      const periodNumber = minutesSinceStart + 1;
      return `${year}${month}${day}${String(periodNumber).padStart(4, '0')}`;
    }

    function getPeriodStartTime(period) {
      // Extract date and period number from period string
      const year = parseInt(period.substring(0, 4));
      const month = parseInt(period.substring(4, 6)) - 1;
      const day = parseInt(period.substring(6, 8));
      const periodNum = parseInt(period.substring(8, 12));
      
      // Calculate start time
      const date = new Date(year, month, day);
      date.setHours(0, 0, 0, 0);
      return date.getTime() + ((periodNum - 1) * 60 * 1000);
    }

    function getTimeLeftInPeriod() {
      const now = Date.now();
      const startTime = getPeriodStartTime(currentRoundId);
      const elapsed = now - startTime;
      const remaining = 60000 - (elapsed % 60000);
      return Math.floor(remaining / 1000);
    }

    // ===========================
    // INITIALIZE
    // ===========================
    checkAutoLogin();

    function checkAutoLogin() {
      const savedUser = localStorage.getItem('glowbet_user');
      if (savedUser) {
        currentUser = JSON.parse(savedUser);
        // Verify user still exists and check status
        const cleanPhone = currentUser.phone.replace(/[^0-9]/g, '');
        database.ref('users/' + cleanPhone).once('value').then(snapshot => {
          if (snapshot.exists()) {
            const userData = snapshot.val();
            if (userData.status === 'banned') {
              showBannedMessage();
              currentUser = null;
              localStorage.removeItem('glowbet_user');
            } else if (userData.status === 'suspended') {
              checkSuspensionExpiry(cleanPhone, userData);
            } else {
              // Update local data
              currentUser = userData;
              localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
              document.getElementById("loginPage").style.display = "none";
              document.getElementById("homePage").style.display = "block";
            }
          } else {
            currentUser = null;
            localStorage.removeItem('glowbet_user');
          }
        });
      } else {
        showLogin();
      }
    }

    function checkSuspensionExpiry(userKey, userData) {
      if (userData.unsuspendAt && Date.now() > userData.unsuspendAt) {
        // Auto-unsuspend
        database.ref('users/' + userKey + '/status').set('active').then(() => {
          database.ref('users/' + userKey + '/unsuspendAt').remove();
          currentUser.status = 'active';
          delete currentUser.unsuspendAt;
          localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
          document.getElementById("loginPage").style.display = "none";
          document.getElementById("homePage").style.display = "block";
        });
      } else {
        showSuspendedMessage(userData.unsuspendAt);
        currentUser = null;
        localStorage.removeItem('glowbet_user');
      }
    }

    // ===========================
    // UTILITY FUNCTIONS
    // ===========================
    function generateUserId() {
      return 'GB' + Date.now().toString().slice(-8) + Math.floor(Math.random() * 1000);
    }

    function generateDepositId() {
      return 'DEP' + Date.now().toString().slice(-10);
    }

    function generateWithdrawalId() {
      return 'WD' + Date.now().toString().slice(-10);
    }

    function formatDate(timestamp) {
      const date = new Date(timestamp);
      const day = String(date.getDate()).padStart(2, '0');
      const month = String(date.getMonth() + 1).padStart(2, '0');
      const year = date.getFullYear();
      const hours = String(date.getHours()).padStart(2, '0');
      const minutes = String(date.getMinutes()).padStart(2, '0');
      return `${day}/${month}/${year} ${hours}:${minutes}`;
    }

    // ===========================
    // AUTH FUNCTIONS
    // ===========================
    function showRegister() {
      document.getElementById("login-form").classList.add("hidden");
      document.getElementById("register-form").classList.remove("hidden");
    }
    
    function showLogin() {
      document.getElementById("register-form").classList.add("hidden");
      document.getElementById("login-form").classList.remove("hidden");
    }
    
    function register() {
      const phone = document.getElementById("reg-phone").value;
      const pass = document.getElementById("reg-pass").value;
      const confirm = document.getElementById("reg-confirm").value;
      
      if (!phone || !pass || !confirm) {
        showCustomPopup("Error", "Please fill all fields");
        return;
      }
      if (pass !== confirm) {
        showCustomPopup("Error", "Passwords do not match");
        return;
      }

      const userId = generateUserId();
      const registeredDate = new Date().toISOString();

      currentUser = { 
        phone, 
        password: pass, 
        balance: 0,
        userId: userId,
        registeredDate: registeredDate,
        status: 'active'
      };

      database.ref('users/' + phone.replace(/[^0-9]/g, '')).set({
        phone: phone,
        password: pass,
        balance: 0,
        userId: userId,
        registeredDate: registeredDate,
        status: 'active'
      }).then(() => {
        localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
        showCustomPopup("Success", "Registration successful! Your ID: " + userId);
        setTimeout(() => {
          document.getElementById("loginPage").style.display = "none";
          document.getElementById("homePage").style.display = "block";
        }, 2000);
      }).catch(error => {
        console.error("Registration error:", error);
        showCustomPopup("Error", "Registration failed. Please try again.");
      });
    }

    function login() {
      const phone = document.getElementById("login-phone").value;
      const pass = document.getElementById("login-password").value;
      
      if (!phone || !pass) {
        showCustomPopup("Error", "Please enter login details");
        return;
      }

      const cleanPhone = phone.replace(/[^0-9]/g, '');
      database.ref('users/' + cleanPhone).once('value').then(snapshot => {
        const userData = snapshot.val();
        if (userData && userData.password === pass) {
          
          // ⚠️ CHECK BAN STATUS
          if (userData.status === 'banned') {
            showBannedMessage();
            return;
          }

          // ⚠️ CHECK SUSPEND STATUS WITH EXPIRY
          if (userData.status === 'suspended') {
            if (userData.unsuspendAt && Date.now() > userData.unsuspendAt) {
              // Auto-unsuspend
              database.ref('users/' + cleanPhone + '/status').set('active').then(() => {
                database.ref('users/' + cleanPhone + '/unsuspendAt').remove();
                userData.status = 'active';
                delete userData.unsuspendAt;
                proceedLogin(userData);
              });
            } else {
              showSuspendedMessage(userData.unsuspendAt);
              return;
            }
          } else {
            proceedLogin(userData);
          }
        } else {
          showCustomPopup("Error", "Invalid credentials");
        }
      }).catch(error => {
        console.error("Login error:", error);
        showCustomPopup("Error", "Login failed. Please try again.");
      });
    }

    function proceedLogin(userData) {
      currentUser = userData;
      localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
      showCustomPopup("Success", "Login successful!");
      setTimeout(() => {
        document.getElementById("loginPage").style.display = "none";
        document.getElementById("homePage").style.display = "block";
      }, 1500);
    }

    // ⚠️ BAN MESSAGE
    function showBannedMessage() {
      const loginForm = document.getElementById("login-form");
      loginForm.innerHTML = `
        <div class="ban-icon">🚫</div>
        <div class="ban-message">
          <strong>YOUR ACCOUNT HAS BEEN BANNED</strong><br>
          Please contact customer support for assistance.
        </div>
        <a href="https://t.me/GlowBet_support" target="_blank" style="display: block; margin-top: 20px;">
          <button class="auth-button">Contact Support</button>
        </a>
        <div class="toggle-link" style="margin-top: 20px;">
          <span onclick="location.reload()">← Back to Login</span>
        </div>
      `;
    }

    // ⚠️ SUSPEND MESSAGE WITH TIME LEFT
    function showSuspendedMessage(unsuspendAt) {
      const loginForm = document.getElementById("login-form");
      const timeLeft = unsuspendAt - Date.now();
      const hoursLeft = Math.ceil(timeLeft / (1000 * 60 * 60));
      
      loginForm.innerHTML = `
        <div class="ban-icon">⏸️</div>
        <div class="suspend-message">
          <strong>YOUR ACCOUNT IS SUSPENDED</strong><br>
          Time remaining: ${hoursLeft} hours<br>
          Please contact support if you believe this is an error.
        </div>
        <a href="https://t.me/GlowBet_support" target="_blank" style="display: block; margin-top: 20px;">
          <button class="auth-button">Contact Support</button>
        </a>
        <div class="toggle-link" style="margin-top: 20px;">
          <span onclick="location.reload()">← Back to Login</span>
        </div>
      `;
    }

    function logout() {
      currentUser = null;
      localStorage.removeItem('glowbet_user');
      hideAllPages();
      document.getElementById("loginPage").style.display = "flex";
      showLogin();
      clearInterval(countdownInterval);
    }

    // ===========================
    // NAVIGATION FUNCTIONS
    // ===========================
    function showHome() {
      hideAllPages();
      document.getElementById('homePage').style.display = 'block';
      updateNavigation('home');
    }

    function showActivity() {
      hideAllPages();
      document.getElementById('activityPage').style.display = 'block';
      updateNavigation('activity');
    }

    function showWallet() {
      hideAllPages();
      document.getElementById('walletPage').style.display = 'block';
      updateNavigation('wallet');
      updateWalletBalance();
    }

    function showAccount() {
      hideAllPages();
      document.getElementById('accountPage').style.display = 'block';
      updateNavigation('account');
      if (currentUser) {
        document.getElementById('profilePhone').textContent = currentUser.phone;
        document.getElementById('displayUserId').textContent = currentUser.userId || 'N/A';
      }
    }

    function hideAllPages() {
      document.getElementById('homePage').style.display = 'none';
      document.getElementById('wingoPage').style.display = 'none';
      document.getElementById('walletPage').style.display = 'none';
      document.getElementById('depositPage').style.display = 'none';
      document.getElementById('withdrawalPage').style.display = 'none';
      document.getElementById('withdrawalHistoryPage').style.display = 'none';
      document.getElementById('accountPage').style.display = 'none';
      document.getElementById('activityPage').style.display = 'none';
    }

    function updateNavigation(active) {
      document.querySelectorAll('.nav-item').forEach(item => item.classList.remove('active'));
      const navItems = document.querySelectorAll('.nav-item');
      if(active === 'home') navItems[0].classList.add('active');
      else if(active === 'activity') navItems[1].classList.add('active');
      else if(active === 'wallet') navItems[2].classList.add('active');
      else if(active === 'account') navItems[3].classList.add('active');
    }

    function goBackToHome() {
      clearInterval(countdownInterval);
      showHome();
    }

    function goBackToWallet() {
      hideAllPages();
      showWallet();
    }

    function goBackToWithdrawal() {
      hideAllPages();
      showWithdrawalPage();
    }

    // ===========================
    // WINGO GAME FUNCTIONS
    // ===========================
    function openWingo() {
      hideAllPages();
      document.getElementById('wingoPage').style.display = 'block';
      initializeWingo();
    }

    function openLottery() {
      showCustomPopup("Info", "Lottery - Coming Soon!");
    }

    function initializeWingo() {
      updateWingoBalance();
      listenToFirebaseResults();
      checkPendingBets();  // ⚠️ NEW: Check for pending bets on load
      startCountdown();
    }

    // ⚠️ FIX #2: CHECK PENDING BETS ON LOAD (AUTO-CREDIT WINS)
    function checkPendingBets() {
      if (!currentUser) return;
      
      database.ref('user_bets/' + currentUser.userId).once('value').then(snapshot => {
        const userBets = snapshot.val();
        if (!userBets) return;
        
        console.log('🔍 Checking pending bets for user:', currentUser.userId);
        
        Object.entries(userBets).forEach(([roundId, betData]) => {
          if (betData.status === 'pending') {
            // Check if result exists
            database.ref('results/' + roundId).once('value').then(resultSnapshot => {
              if (resultSnapshot.exists()) {
                const result = resultSnapshot.val();
                console.log('📊 Found result for pending bet:', roundId);
                processPendingBet(betData, result, roundId);
              }
            });
          }
        });
      });
    }

    function processPendingBet(bet, result, roundId) {
      let won = false;
      let multiplier = 1.96;

      if (typeof bet.selection === 'number') {
        won = (bet.selection === result.number);
        multiplier = 8.96;
      } else if (bet.selection === 'red') {
        won = result.colors.includes('red');
      } else if (bet.selection === 'green') {
        won = result.colors.includes('green');
      } else if (bet.selection === 'violet') {
        won = result.colors.includes('violet');
        multiplier = 4.0;
      } else if (bet.selection === 'big') {
        won = (result.size === 'big');
      } else if (bet.selection === 'small') {
        won = (result.size === 'small');
      }

      if (won) {
        const winAmount = bet.amount * multiplier;
        const cleanPhone = currentUser.phone.replace(/[^0-9]/g, '');
        
        database.ref('users/' + cleanPhone).once('value').then(snapshot => {
          const userData = snapshot.val();
          const newBalance = (userData.balance || 0) + winAmount;
          
          database.ref('users/' + cleanPhone + '/balance').set(newBalance).then(() => {
            currentUser.balance = newBalance;
            localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
            updateWingoBalance();
            
            // Mark bet as processed
            database.ref('user_bets/' + currentUser.userId + '/' + roundId + '/status').set('won');
            
            console.log('✅ Auto-credited win:', winAmount);
            showCustomPopup("Win Credited!", `₹${winAmount.toFixed(2)} has been credited to your account!`);
          });
        });
      } else {
        // Mark bet as lost
        database.ref('user_bets/' + currentUser.userId + '/' + roundId + '/status').set('lost');
      }
    }

    // ⚠️ FIX #3: BACKGROUND-WORKING TIMER
    function startCountdown() {
      clearInterval(countdownInterval);
      
      currentRoundId = generateCurrentPeriod();
      periodStartTime = getPeriodStartTime(currentRoundId);
      
      countdown = getTimeLeftInPeriod();
      isBettingLocked = false;
      unlockBetting();
      
      updateRoundId();
      updateTimer();
      
      console.log('🎮 [USER] Round:', currentRoundId, '| Time left:', countdown);
      
      countdownInterval = setInterval(() => {
        // Recalculate from timestamp (background-safe)
        countdown = getTimeLeftInPeriod();
        
        // Check if period changed
        const newPeriod = generateCurrentPeriod();
        if (newPeriod !== currentRoundId) {
          console.log('🔄 Period changed, restarting...');
          clearInterval(countdownInterval);
          waitForResult(currentRoundId);
          return;
        }
        
        updateTimer();
        
        if (countdown <= 5 && !isBettingLocked) {
          lockBetting();
        }
        
        if (countdown <= 0) {
          clearInterval(countdownInterval);
          waitForResult(currentRoundId);
        }
      }, 1000);
    }

    function waitForResult(roundId) {
      console.log('⏳ Waiting for result:', roundId);
      
      let attempts = 0;
      const maxAttempts = 10;
      
      const checkResult = setInterval(() => {
        attempts++;
        
        database.ref('results/' + roundId).once('value').then(snapshot => {
          if (snapshot.exists()) {
            clearInterval(checkResult);
            const result = snapshot.val();
            console.log('✅ Result received:', result);
            
            checkUserBetsForRound(roundId, result);
            
            setTimeout(() => {
              startCountdown();
            }, 3000);
          } else if (attempts >= maxAttempts) {
            clearInterval(checkResult);
            console.log('⚠️ No result after 10 attempts, moving on');
            startCountdown();
          }
        });
      }, 1000);
    }

    function checkUserBetsForRound(roundId, result) {
      if (!currentUser) return;
      
      database.ref('user_bets/' + currentUser.userId + '/' + roundId).once('value').then(snapshot => {
        if (snapshot.exists()) {
          const betData = snapshot.val();
          if (betData.status === 'pending') {
            processPendingBet(betData, result, roundId);
          }
        }
      });
    }

    function lockBetting() {
      isBettingLocked = true;
      const bettingArea = document.getElementById('bettingArea');
      const timerDisplay = document.getElementById('countdownTimer');
      
      bettingArea.classList.add('locked');
      timerDisplay.classList.add('locked');
      
      document.querySelectorAll('.color-option, .number-cell, .size-option').forEach(el => {
        el.classList.add('disabled');
      });
    }

    function unlockBetting() {
      isBettingLocked = false;
      const bettingArea = document.getElementById('bettingArea');
      const timerDisplay = document.getElementById('countdownTimer');
      
      bettingArea.classList.remove('locked');
      timerDisplay.classList.remove('locked');
      
      document.querySelectorAll('.color-option, .number-cell, .size-option').forEach(el => {
        el.classList.remove('disabled');
      });
    }

    function updateRoundId() {
      const period = currentRoundId || generateCurrentPeriod();
      document.getElementById('currentRoundId').textContent = period.slice(-4);
    }

    function updateTimer() {
      document.getElementById('countdownTimer').textContent = countdown + 's';
    }

    function getColorForNumber(number) {
      if (number === 0) return ['red', 'violet'];
      if (number === 5) return ['green', 'violet'];
      if ([1, 3, 7, 9].includes(number)) return ['green'];
      return ['red'];
    }

    function listenToFirebaseResults() {
      database.ref('results').orderByChild('timestamp').limitToLast(500).on('value', (snapshot) => {
        allResults = [];
        snapshot.forEach((childSnapshot) => {
          const data = childSnapshot.val();
          if (data && data.period && data.number !== undefined) {
            allResults.push(data);
          }
        });
        
        allResults.sort((a, b) => b.timestamp - a.timestamp);
        
        currentPage = 1;
        displayResultsForPage(currentPage);
      });
    }

    function displayResultsForPage(pageNum) {
      const startIndex = (pageNum - 1) * RESULTS_PER_PAGE;
      const endIndex = startIndex + RESULTS_PER_PAGE;
      const pageResults = allResults.slice(startIndex, endIndex);
      
      const tbody = document.getElementById('historyTableBody');
      tbody.innerHTML = '';
      
      if (pageResults.length === 0) {
        tbody.innerHTML = '<tr><td colspan="4" style="text-align: center; padding: 20px;">No results yet</td></tr>';
      } else {
        pageResults.forEach(result => {
          const row = document.createElement('tr');
          
          const periodCell = document.createElement('td');
          periodCell.textContent = result.period.slice(-4);
          
          const numberCell = document.createElement('td');
          const numberSpan = document.createElement('span');
          numberSpan.className = `result-number result-number-${result.number}`;
          numberSpan.textContent = result.number;
          numberCell.appendChild(numberSpan);
          
          const sizeCell = document.createElement('td');
          sizeCell.textContent = result.size.toUpperCase();
          
          const colorCell = document.createElement('td');
          colorCell.className = 'result-colors';
          const colorEmojis = result.colors.map(c => {
            if (c === 'red') return '🔴';
            if (c === 'green') return '🟢';
            if (c === 'violet') return '🟣';
            return '';
          }).join(' ');
          colorCell.textContent = colorEmojis;
          
          row.appendChild(periodCell);
          row.appendChild(numberCell);
          row.appendChild(sizeCell);
          row.appendChild(colorCell);
          tbody.appendChild(row);
        });
      }
      
      const totalPages = Math.ceil(allResults.length / RESULTS_PER_PAGE) || 1;
      document.getElementById('currentPageNum').textContent = pageNum;
      document.getElementById('totalPagesNum').textContent = totalPages;
      
      document.getElementById('prevPageBtn').disabled = (pageNum === 1);
      document.getElementById('nextPageBtn').disabled = (pageNum >= totalPages);
    }

    function previousPage() {
      if (currentPage > 1) {
        currentPage--;
        displayResultsForPage(currentPage);
      }
    }

    function nextPage() {
      const totalPages = Math.ceil(allResults.length / RESULTS_PER_PAGE);
      if (currentPage < totalPages) {
        currentPage++;
        displayResultsForPage(currentPage);
      }
    }

    function showGameHistory() {
      document.querySelectorAll('.history-tab').forEach(tab => tab.classList.remove('active'));
      document.querySelectorAll('.history-tab')[0].classList.add('active');
      currentPage = 1;
      displayResultsForPage(currentPage);
    }

    function showMyHistory() {
      showCustomPopup("Info", "My History - Coming Soon!");
    }

    // ===========================
    // BETTING FUNCTIONS
    // ===========================
    function selectBet(selection) {
      if (isBettingLocked) {
        showCustomPopup("Error", "Betting is locked! Wait for next round.");
        return;
      }
      
      currentBet = selection;
      let displayText = selection;
      if (typeof selection === 'number') {
        displayText = `Number ${selection}`;
      } else {
        displayText = selection.charAt(0).toUpperCase() + selection.slice(1);
      }
      
      document.getElementById('betSelection').textContent = `Selected: ${displayText}`;
      calculatePotentialWin();
      document.getElementById('betPopup').style.display = 'flex';
    }

    function changeAmount(delta) {
      betAmount = Math.max(10, betAmount + delta);
      document.getElementById('betAmount').textContent = betAmount;
      calculatePotentialWin();
    }

    function openCustomAmount() {
      document.getElementById('customAmountModal').style.display = 'flex';
      document.getElementById('customAmountInput').value = betAmount;
      document.getElementById('customAmountInput').focus();
    }

    function closeCustomAmount() {
      document.getElementById('customAmountModal').style.display = 'none';
    }

    function applyCustomAmount() {
      const customAmount = parseInt(document.getElementById('customAmountInput').value);
      if (customAmount && customAmount >= 10) {
        betAmount = customAmount;
        document.getElementById('betAmount').textContent = betAmount;
        calculatePotentialWin();
        closeCustomAmount();
      } else {
        showCustomPopup("Error", "Minimum bet amount is ₹10");
      }
    }

    function calculatePotentialWin() {
      let winMultiplier = 1.96;
      
      if (typeof currentBet === 'number') {
        winMultiplier = 8.96;
      } else if (currentBet === 'violet') {
        winMultiplier = 4.0;
      } else if (currentBet === 'red' || currentBet === 'green' || currentBet === 'big' || currentBet === 'small') {
        winMultiplier = 1.96;
      }
      
      const potentialWin = betAmount * winMultiplier;
      document.getElementById('multiplierDisplay').textContent = `${winMultiplier}x`;
      document.getElementById('potentialWin').textContent = `₹${potentialWin.toFixed(2)}`;
    }

    function placeBet() {
      if (!currentUser) {
        showCustomPopup("Error", "Please login first");
        return;
      }
      
      if (isBettingLocked) {
        showCustomPopup("Error", "Betting is locked! Wait for next round.");
        closeBetPopup();
        return;
      }
      
      if (currentUser.balance < betAmount) {
        showCustomPopup("Error", "Insufficient balance!");
        return;
      }
      
      // Deduct balance
      currentUser.balance -= betAmount;
      
      const cleanPhone = currentUser.phone.replace(/[^0-9]/g, '');
      database.ref('users/' + cleanPhone + '/balance').set(currentUser.balance);
      localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
      
      // ⚠️ SAVE BET TO FIREBASE (PERSISTENT)
      const betData = {
        selection: currentBet,
        amount: betAmount,
        roundId: currentRoundId,
        userId: currentUser.userId,
        phone: currentUser.phone,
        timestamp: Date.now(),
        status: 'pending'
      };
      
      database.ref('user_bets/' + currentUser.userId + '/' + currentRoundId).set(betData);
      database.ref('bets/' + currentRoundId + '/' + Date.now()).set(betData);
      
      console.log('💰 [USER] Bet placed and saved:', betData);
      
      showCustomPopup("Success", `Bet placed! ₹${betAmount} on ${currentBet}`);
      closeBetPopup();
      updateWingoBalance();
      
      betAmount = 100;
      document.getElementById('betAmount').textContent = betAmount;
    }

    function closeBetPopup() {
      document.getElementById('betPopup').style.display = 'none';
    }

    function closeResultPopup() {
      document.getElementById('resultPopup').style.display = 'none';
    }

    // ===========================
    // BALANCE FUNCTIONS
    // ===========================
    function updateWingoBalance() {
      if (currentUser) {
        document.getElementById('wingoBalance').textContent = `₹${currentUser.balance.toFixed(2)}`;
      }
    }

    function refreshWingoBalance() {
      if (!currentUser) return;
      
      const cleanPhone = currentUser.phone.replace(/[^0-9]/g, '');
      database.ref('users/' + cleanPhone + '/balance').once('value').then(snapshot => {
        const balance = snapshot.val();
        if (balance !== null) {
          currentUser.balance = balance;
          localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
          updateWingoBalance();
          showCustomPopup("Success", "Balance refreshed!");
        }
      });
    }

    function updateWalletBalance() {
      if (currentUser) {
        document.getElementById('walletBalance').textContent = `₹${currentUser.balance.toFixed(2)}`;
      }
    }

    // ===========================
    // DEPOSIT FUNCTIONS
    // ===========================
    function showDepositPage() {
      hideAllPages();
      document.getElementById('depositPage').style.display = 'block';
      document.getElementById('paymentSection').style.display = 'none';
    }

    function proceedToPayment() {
      const amount = parseFloat(document.getElementById('depositAmount').value);
      if (!amount || amount < 80) {
        showCustomPopup("Error", "Minimum deposit amount is ₹80");
        return;
      }
      document.getElementById('displayAmount').textContent = `₹${amount}`;
      document.getElementById('paymentSection').style.display = 'block';
      document.getElementById('paymentSection').scrollIntoView({ behavior: 'smooth' });
    }

    function submitUTR() {
      const utr = document.getElementById('utrNumber').value;
      const amount = parseFloat(document.getElementById('depositAmount').value);
      
      if (!utr || utr.length < 10) {
        showCustomPopup("Error", "Please enter valid UTR number");
        return;
      }

      if (!currentUser) {
        showCustomPopup("Error", "Please login first");
        return;
      }

      const depositId = generateDepositId();
      const depositData = {
        depositId: depositId,
        userId: currentUser.userId,
        phone: currentUser.phone,
        amount: amount,
        utr: utr,
        status: 'pending',
        timestamp: Date.now(),
        date: new Date().toISOString()
      };

      database.ref('deposits/' + depositId).set(depositData).then(() => {
        showCustomPopup("Success", `Deposit request submitted! Your Deposit ID: ${depositId}`);
        setTimeout(() => {
          document.getElementById('depositAmount').value = '';
          document.getElementById('utrNumber').value = '';
          showWallet();
        }, 2500);
      }).catch(error => {
        console.error("Deposit error:", error);
        showCustomPopup("Error", "Failed to submit deposit request");
      });
    }

    // ===========================
    // WITHDRAWAL FUNCTIONS
    // ===========================
    function showWithdrawalPage() {
      hideAllPages();
      document.getElementById('withdrawalPage').style.display = 'block';
      
      if (currentUser && currentUser.bankDetails) {
        document.getElementById('savedBankDetails').style.display = 'block';
        document.getElementById('bankDetailsForm').style.display = 'none';
        document.getElementById('savedAccNumber').textContent = currentUser.bankDetails.accNumber;
      } else {
        document.getElementById('savedBankDetails').style.display = 'none';
        document.getElementById('bankDetailsForm').style.display = 'block';
      }
    }

    function saveBankDetails() {
      const accNumber = document.getElementById('accNumber').value;
      const ifsc = document.getElementById('ifscCode').value;
      
      if (!accNumber || !ifsc) {
        showCustomPopup("Error", "Please fill all bank details");
        return;
      }

      if (currentUser) {
        currentUser.bankDetails = { accNumber, ifsc };
        
        const cleanPhone = currentUser.phone.replace(/[^0-9]/g, '');
        database.ref('users/' + cleanPhone + '/bankDetails').set({ accNumber, ifsc });
        
        localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
        showCustomPopup("Success", "Bank details saved!");
        showWithdrawalPage();
      }
    }

    function editBankDetails() {
      document.getElementById('savedBankDetails').style.display = 'none';
      document.getElementById('bankDetailsForm').style.display = 'block';
      
      if (currentUser && currentUser.bankDetails) {
        document.getElementById('accNumber').value = currentUser.bankDetails.accNumber;
        document.getElementById('ifscCode').value = currentUser.bankDetails.ifsc;
      }
    }

    function submitWithdrawal() {
      if (!currentUser || !currentUser.bankDetails) {
        showCustomPopup("Error", "Please save bank details first");
        return;
      }

      const amount = parseFloat(document.getElementById('withdrawalAmount').value);
      if (!amount || amount < 100) {
        showCustomPopup("Error", "Minimum withdrawal amount is ₹100");
        return;
      }

      if (amount > currentUser.balance) {
        showCustomPopup("Error", "Insufficient balance!");
        return;
      }

      const withdrawalId = generateWithdrawalId();
      const withdrawalData = {
        withdrawalId: withdrawalId,
        userId: currentUser.userId,
        phone: currentUser.phone,
        amount: amount,
        bankDetails: currentUser.bankDetails,
        status: 'pending',
        timestamp: Date.now(),
        date: new Date().toISOString()
      };

      currentUser.balance -= amount;
      const cleanPhone = currentUser.phone.replace(/[^0-9]/g, '');
      
      database.ref('withdrawals/' + withdrawalId).set(withdrawalData);
      database.ref('users/' + cleanPhone + '/balance').set(currentUser.balance);
      
      localStorage.setItem('glowbet_user', JSON.stringify(currentUser));
      
      showCustomPopup("Success", `Withdrawal request submitted! ID: ${withdrawalId}`);
      document.getElementById('withdrawalAmount').value = '';
    }

    // ===========================
    // WITHDRAWAL HISTORY FUNCTIONS
    // ===========================
    function showWithdrawalHistoryPage() {
      if (!currentUser) {
        showCustomPopup("Error", "Please login first");
        return;
      }

      hideAllPages();
      document.getElementById('withdrawalHistoryPage').style.display = 'block';
      loadWithdrawalHistory();
    }

    function loadWithdrawalHistory() {
      const contentDiv = document.getElementById('withdrawalHistoryContent');
      contentDiv.innerHTML = '<div class="no-history"><p>Loading withdrawal history...</p></div>';

      database.ref('withdrawals').orderByChild('userId').equalTo(currentUser.userId).once('value')
        .then(snapshot => {
          contentDiv.innerHTML = '';
          
          if (!snapshot.exists()) {
            contentDiv.innerHTML = '<div class="no-history"><p>🔭 No withdrawal history found</p></div>';
            return;
          }

          const withdrawals = [];
          snapshot.forEach(childSnapshot => {
            withdrawals.push(childSnapshot.val());
          });

          withdrawals.sort((a, b) => b.timestamp - a.timestamp);

          withdrawals.forEach(withdrawal => {
            const card = document.createElement('div');
            card.className = 'withdrawal-detail-card';
            
            const statusBadgeClass = withdrawal.status === 'pending' ? 'status-pending' : 'status-completed';
            const statusText = withdrawal.status === 'pending' ? 'Pending' : 'Completed';
            
            card.innerHTML = `
              <div class="detail-row">
                <span class="detail-label">Withdrawal ID:</span>
                <span class="detail-value">${withdrawal.withdrawalId}</span>
              </div>
              <div class="detail-row">
                <span class="detail-label">User ID:</span>
                <span class="detail-value">${withdrawal.userId}</span>
              </div>
              <div class="detail-row">
                <span class="detail-label">Phone:</span>
                <span class="detail-value">${withdrawal.phone}</span>
              </div>
              <div class="detail-row">
                <span class="detail-label">Amount:</span>
                <span class="detail-value" style="color: #00a86b; font-weight: bold;">₹${withdrawal.amount.toFixed(2)}</span>
              </div>
              <div class="detail-row">
                <span class="detail-label">Date & Time:</span>
                <span class="detail-value">${formatDate(withdrawal.timestamp)}</span>
              </div>
              <div class="detail-row">
                <span class="detail-label">Status:</span>
                <span class="status-badge ${statusBadgeClass}">${statusText}</span>
              </div>
            `;
            
            contentDiv.appendChild(card);
          });
        })
        .catch(error => {
          console.error("Error loading withdrawal history:", error);
          contentDiv.innerHTML = '<div class="no-history"><p>❌ Failed to load withdrawal history</p></div>';
        });
    }

    // ===========================
    // ACTIVITY FUNCTIONS
    // ===========================
    function claimGiftCode() {
      const code = document.getElementById('giftCodeInput').value.trim();
      if (!code) {
        showCustomPopup("Error", "Please enter a gift code");
        return;
      }
      showCustomPopup("Error", "Invalid gift code!");
    }

    // ===========================
    // POPUP FUNCTIONS
    // ===========================
    function showCustomPopup(title, message) {
      document.getElementById('popupTitle').textContent = title;
      document.getElementById('popupMessage').textContent = message;
      document.getElementById('successPopup').style.display = 'flex';
    }

    function closeCustomPopup() {
      document.getElementById('successPopup').style.display = 'none';
    }
  </script>
</body>
</html>
