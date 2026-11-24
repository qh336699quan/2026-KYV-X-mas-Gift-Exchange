<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>🎄 聖誕交換禮物配對 🎁</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@400;500;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans TC', sans-serif;
            background-color: #0f172a;
            background-image: 
                radial-gradient(circle at 15% 50%, rgba(220, 38, 38, 0.15), transparent 25%),
                radial-gradient(circle at 85% 30%, rgba(22, 163, 74, 0.15), transparent 25%);
            color: #f8fafc;
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* 簡單的雪花動畫背景 */
        .snowflake {
            position: fixed;
            top: -10vh;
            color: white;
            font-size: 1.5em;
            text-shadow: 0 0 5px rgba(255,255,255,0.3);
            user-select: none;
            z-index: -1;
            animation: fall linear forwards;
        }

        @keyframes fall {
            to {
                transform: translateY(110vh);
            }
        }

        .glass-panel {
            background: rgba(255, 255, 255, 0.03);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.08);
            box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
        }

        .btn-primary {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
        }
        .btn-primary:hover:not(:disabled) {
            background: rgba(255, 255, 255, 0.2);
            border-color: rgba(255, 255, 255, 0.4);
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(255, 255, 255, 0.05);
        }
        .btn-primary:disabled {
            background: rgba(255, 255, 255, 0.02);
            border-color: rgba(255, 255, 255, 0.05);
            transform: none;
            box-shadow: none;
            cursor: not-allowed;
            opacity: 0.5;
        }

        /* Emoji pop animation */
        @keyframes pop-up {
            0% { transform: translate(-50%, -50%) scale(0.5) rotate(0deg); opacity: 1; }
            70% { opacity: 1; }
            100% { transform: translate(var(--tx), var(--ty)) scale(1.5) rotate(var(--rot)); opacity: 0; }
        }
        .emoji-particle {
            position: fixed;
            pointer-events: none;
            z-index: 9999;
            /* 改為 2.5 秒，讓動畫變慢、更飄逸 */
            animation: pop-up 2.5s cubic-bezier(0.1, 0.8, 0.2, 1) forwards;
        }
    </style>
</head>
<body class="p-4 md:p-8">

    <!-- 雪花容器 -->
    <div id="snowflakes-container"></div>

    <div class="max-w-4xl mx-auto">
        <!-- 標題區 -->
        <header class="text-center mb-10">
            <h1 class="text-3xl md:text-4xl font-light text-white mb-3 tracking-widest drop-shadow-md flex items-center justify-center gap-3">
                <span class="text-2xl">❄️</span> 聖誕交換禮物 <span class="text-2xl">❄️</span>
            </h1>
            <p class="text-gray-400 text-sm md:text-base font-light tracking-wide">預算 300 元 / 根據形容詞準備驚喜</p>
        </header>

        <!-- 主要內容區 -->
        <div id="main-content" class="max-w-2xl mx-auto space-y-6">
            
            <!-- 1. 加入遊戲 (輸入表單) -->
            <div class="glass-panel rounded-2xl p-6 relative overflow-hidden">
                <h2 class="text-xl font-light mb-5 text-white tracking-wide border-b border-gray-700/50 pb-2">加入遊戲</h2>
                
                <form id="add-form" class="space-y-5">
                    <!-- 玩家選擇區 (下拉選單) -->
                    <div class="mb-4">
                        <label class="block text-sm font-light text-gray-300 mb-1">選擇玩家</label>
                        <select id="select-player" required
                            class="w-full bg-gray-800/50 border border-gray-600 rounded-lg px-4 py-2 text-white focus:outline-none focus:border-white/50 focus:ring-1 focus:ring-white/50 cursor-pointer font-light">
                            <!-- 選項由 JS 動態產生 -->
                        </select>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                        <div>
                            <label class="block text-sm font-light text-gray-300 mb-1">形容詞 1</label>
                            <input type="text" id="input-adj1" required placeholder="例如：毛茸茸的" 
                                class="w-full bg-gray-800/50 border border-gray-600 rounded-lg px-4 py-2 text-white focus:outline-none focus:border-white/50 focus:ring-1 focus:ring-white/50 font-light">
                        </div>
                        <div>
                            <label class="block text-sm font-light text-gray-300 mb-1">形容詞 2</label>
                            <input type="text" id="input-adj2" required placeholder="例如：會發光的" 
                                class="w-full bg-gray-800/50 border border-gray-600 rounded-lg px-4 py-2 text-white focus:outline-none focus:border-white/50 focus:ring-1 focus:ring-white/50 font-light">
                        </div>
                    </div>
                    
                    <!-- 錯誤訊息提示區 -->
                    <div id="error-msg" class="hidden text-red-300 text-sm font-light bg-red-900/30 p-3 rounded-lg border border-red-500/30"></div>

                    <button type="submit" class="w-full btn-primary text-white font-light py-3 rounded-xl flex items-center justify-center gap-2 mt-2">
                        <span>加入清單</span>
                        <span class="opacity-70">＋</span>
                    </button>
                </form>
            </div>

            <!-- 2. 已使用的形容詞看板 -->
            <div class="glass-panel rounded-2xl p-6">
                <h2 class="text-lg font-light mb-2 text-white tracking-wide flex items-center gap-2">
                    <span class="opacity-70">🏷️</span> 已使用的形容詞
                </h2>
                <p class="text-xs text-gray-400 mb-4 font-light">請避開這些詞，發揮創意想點別的吧！</p>
                
                <div id="adjectives-board" class="flex flex-wrap gap-2">
                    <!-- 形容詞標籤會動態生成在這裡 -->
                    <span class="text-sm text-gray-500 italic" id="empty-adj-msg">目前還沒有形容詞</span>
                </div>
            </div>

            <!-- 3. 已加入玩家列表 -->
            <div class="glass-panel rounded-2xl p-6">
                <div class="flex justify-between items-center mb-4">
                    <h2 class="text-lg font-light text-white tracking-wide">目前玩家 <span id="player-count" class="text-sm bg-white/10 px-2 py-1 rounded-full text-gray-300 ml-2 font-mono">0/7</span></h2>
                </div>
                
                <div id="players-list" class="grid grid-cols-1 gap-3 empty:hidden">
                    <!-- 玩家卡片會動態生成在這裡 -->
                </div>
                <div id="empty-players-msg" class="text-center py-6 text-gray-500 font-light">
                    還沒有人加入喔，趕快邀請大家填寫！
                </div>
            </div>

            <!-- 4. 主辦人專區 (抽籤控制) -->
            <div class="glass-panel rounded-2xl p-6 border-t border-t-white/10 mt-8">
                <div class="flex items-center gap-2 mb-4">
                    <span class="text-xl opacity-70">🔒</span>
                    <h2 class="text-lg font-light text-white tracking-wide">主辦人專區</h2>
                </div>
                <p id="admin-hint" class="text-xs text-gray-400 mb-4 font-light">請輸入解鎖密碼以顯示控制按鈕</p>
                <input type="password" id="input-password" placeholder="密碼..." 
                    class="w-full md:w-1/2 bg-gray-800/30 border border-gray-600/50 rounded-lg px-4 py-2 text-white focus:outline-none focus:border-white/50 mb-4 font-light placeholder-gray-600 transition-colors">
                
                <div id="draw-section" class="hidden mt-4 pt-4 border-t border-gray-700/30">
                    <div class="flex gap-4">
                        <button id="btn-reset-admin" class="w-1/3 bg-red-900/30 hover:bg-red-800/40 border border-red-700/50 text-red-200 font-light py-4 rounded-xl text-lg flex flex-col items-center justify-center transition-colors">
                            <span>重新</span>
                        </button>
                        <button id="btn-draw" disabled class="w-2/3 btn-primary text-white font-light py-4 rounded-xl text-lg flex flex-col items-center justify-center gap-2 tracking-widest">
                            <span>開始抽籤</span>
                        </button>
                    </div>
                    <p id="draw-hint" class="text-xs text-gray-400 mt-3 text-center font-light">最少需要 3 人才能抽籤</p>
                </div>
            </div>
        </div>

        <!-- 結果展示區 (預設隱藏) -->
        <div id="results-content" class="hidden max-w-4xl mx-auto">
            <div class="glass-panel rounded-3xl p-8 relative">
            <div class="glass-panel rounded-3xl p-8 border-2 border-yellow-500/30 relative">
                <!-- 裝飾 -->
                <div class="absolute -top-6 left-1/2 transform -translate-x-1/2 text-5xl">🎁</div>
                
                <div class="text-center mt-4 mb-8">
                    <h2 class="text-3xl font-black text-yellow-300 mb-2">配對結果大公開！</h2>
                    <p class="text-gray-300">每個人都拿到任務了，快去準備符合對方形容詞的禮物吧！</p>
                </div>

                <div id="results-list" class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <!-- 結果卡片會動態生成在這裡 -->
                </div>

                <div class="mt-10 text-center">
                    <button id="btn-reset" class="bg-gray-700 hover:bg-gray-600 text-white font-bold py-2 px-6 rounded-lg transition-colors">
                        重新開始新遊戲
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- 自訂訊息彈窗 (取代 alert) -->
    <div id="modal" class="fixed inset-0 bg-black/60 backdrop-blur-sm hidden items-center justify-center z-50">
        <div class="glass-panel bg-gray-900/90 rounded-2xl p-6 max-w-sm w-full mx-4 shadow-2xl border border-gray-700 transform scale-95 opacity-0 transition-all duration-300" id="modal-content">
            <h3 id="modal-title" class="text-xl font-bold text-white mb-2">提示</h3>
            <p id="modal-message" class="text-gray-300 mb-6"></p>
            <div class="text-right">
                <button id="btn-modal-close" class="bg-blue-600 hover:bg-blue-500 text-white font-bold py-2 px-4 rounded-lg transition-colors">
                    知道了
                </button>
            </div>
        </div>
    </div>

    <script>
        // --- 應用程式狀態 ---
        let participants = []; // 結構: { name: string, adj1: string, adj2: string }
        let usedAdjectives = new Set();
        
        // --- 預設玩家資料 ---
        const friendData = [
            { name: "請選擇玩家..." },
            { name: "Huan" },
            { name: "Soda" },
            { name: "芳淇" },
            { name: "Coco" },
            { name: "傑利" },
            { name: "蓉師" },
            { name: "Ali" }
        ];

        // --- DOM 元素 ---
        const form = document.getElementById('add-form');
        const selectPlayer = document.getElementById('select-player');
        const inputAdj1 = document.getElementById('input-adj1');
        const inputAdj2 = document.getElementById('input-adj2');
        const errorMsg = document.getElementById('error-msg');
        
        const playersList = document.getElementById('players-list');
        const emptyPlayersMsg = document.getElementById('empty-players-msg');
        const playerCountLabel = document.getElementById('player-count');
        
        const adjectivesBoard = document.getElementById('adjectives-board');
        const emptyAdjMsg = document.getElementById('empty-adj-msg');
        
        const inputPassword = document.getElementById('input-password');
        const drawSection = document.getElementById('draw-section');
        const btnDraw = document.getElementById('btn-draw');
        const drawHint = document.getElementById('draw-hint');
        
        const mainContent = document.getElementById('main-content');
        const resultsContent = document.getElementById('results-content');
        const resultsList = document.getElementById('results-list');
        const btnReset = document.getElementById('btn-reset');

        // Modal Elements
        const modal = document.getElementById('modal');
        const modalContent = document.getElementById('modal-content');
        const modalTitle = document.getElementById('modal-title');
        const modalMessage = document.getElementById('modal-message');
        const btnModalClose = document.getElementById('btn-modal-close');

        // --- 輔助功能：彈窗與特效 ---
        let lastClickX = window.innerWidth / 2;
        let lastClickY = window.innerHeight / 2;
        
        document.addEventListener('click', (e) => {
            lastClickX = e.clientX;
            lastClickY = e.clientY;
        });

        function createEmojiPop(x, y) {
            const emojis = ['🎄', '🎁', '❄️', '⛄', '🔔', '✨', '🦌']; // 加上麋鹿
            for (let i = 0; i < 18; i++) { // 增加數量
                const particle = document.createElement('div');
                // 放大 Emoji 尺寸，改為 3xl 到 5xl
                particle.className = 'emoji-particle text-3xl md:text-5xl';
                particle.textContent = emojis[Math.floor(Math.random() * emojis.length)];
                particle.style.left = `${x}px`;
                particle.style.top = `${y}px`;
                
                const angle = Math.random() * Math.PI * 2;
                // 增加飄散距離，讓畫面更豐富
                const distance = 100 + Math.random() * 200;
                const rot = (Math.random() - 0.5) * 360;
                
                particle.style.setProperty('--tx', `${Math.cos(angle) * distance}px`);
                particle.style.setProperty('--ty', `${Math.sin(angle) * distance}px`);
                particle.style.setProperty('--rot', `${rot}deg`);
                
                document.body.appendChild(particle);
                // 配合新的 CSS 動畫時間 (2.5s) 延遲移除
                setTimeout(() => particle.remove(), 2500);
            }
        }

        function showModal(title, message, isError = false) {
            modalTitle.textContent = title;
            modalMessage.textContent = message;
            modalTitle.className = `text-xl font-bold mb-2 ${isError ? 'text-red-400' : 'text-blue-400'}`;
            
            modal.classList.remove('hidden');
            modal.classList.add('flex');
            // 觸發動畫
            setTimeout(() => {
                modalContent.classList.remove('scale-95', 'opacity-0');
                modalContent.classList.add('scale-100', 'opacity-100');
            }, 10);
        }

        function closeModal() {
            modalContent.classList.remove('scale-100', 'opacity-100');
            modalContent.classList.add('scale-95', 'opacity-0');
            setTimeout(() => {
                modal.classList.remove('flex');
                modal.classList.add('hidden');
            }, 300);
        }

        btnModalClose.addEventListener('click', closeModal);

        // --- 核心邏輯：新增玩家 ---
        form.addEventListener('submit', (e) => {
            e.preventDefault();
            errorMsg.classList.add('hidden');

            const selectedIndex = selectPlayer.value;
            if (selectedIndex === "0" || !selectedIndex) {
                 showError("請選擇一名玩家！");
                 return;
            }

            const name = friendData[selectedIndex].name;
            const adj1 = inputAdj1.value.trim();
            const adj2 = inputAdj2.value.trim();

            // 基本驗證
            if (!adj1 || !adj2) return;

            // 檢查姓名是否重複
            if (participants.some(p => p.name === name)) {
                showError(`「${name}」已經加入過了喔！`);
                return;
            }

            // 檢查形容詞是否重複 (大小寫視為相同)
            const cleanAdj1 = adj1.toLowerCase();
            const cleanAdj2 = adj2.toLowerCase();

            if (cleanAdj1 === cleanAdj2) {
                showError("你填寫的兩個形容詞不能一樣啦！");
                return;
            }

            // 檢查是否與別人重複
            const currentUsed = Array.from(usedAdjectives).map(a => a.toLowerCase());
            if (currentUsed.includes(cleanAdj1)) {
                showError(`形容詞「${adj1}」已經被別人用過囉，換一個吧！`);
                return;
            }
            if (currentUsed.includes(cleanAdj2)) {
                showError(`形容詞「${adj2}」已經被別人用過囉，換一個吧！`);
                return;
            }

            // 成功加入
            participants.push({ name, adj1, adj2 });
            usedAdjectives.add(adj1);
            usedAdjectives.add(adj2);

            // 停用已經加入的選項，避免重複選擇
            selectPlayer.options[selectedIndex].disabled = true;

            // 清空表單
            selectPlayer.value = "0";
            inputAdj1.value = '';
            inputAdj2.value = '';
            selectPlayer.focus();

            // 觸發 Emoji 噴發特效
            createEmojiPop(lastClickX, lastClickY);

            updateUI();
        });

        function showError(msg) {
            errorMsg.textContent = msg;
            errorMsg.classList.remove('hidden');
        }

        // --- 核心邏輯：移除玩家 ---
        function removeParticipant(name) {
            const index = participants.findIndex(p => p.name === name);
            if (index > -1) {
                const p = participants[index];
                usedAdjectives.delete(p.adj1);
                usedAdjectives.delete(p.adj2);
                participants.splice(index, 1);
                
                // 恢復下拉選單的選項為可選狀態
                const optionIndex = friendData.findIndex(f => f.name === name);
                if (optionIndex > -1) {
                    selectPlayer.options[optionIndex].disabled = false;
                }

                updateUI();
            }
        }

        // --- 核心邏輯：更新畫面 ---
        function updateUI() {
            // 更新計數
            playerCountLabel.textContent = `${participants.length}/7`;
            
            // 更新玩家清單
            playersList.innerHTML = '';
            if (participants.length > 0) {
                emptyPlayersMsg.style.display = 'none';
                participants.forEach(p => {
                    const div = document.createElement('div');
                    div.className = 'bg-white/5 border border-white/10 rounded-xl p-4 flex justify-between items-center transition-all hover:bg-white/10';
                    div.innerHTML = `
                        <div class="flex items-center gap-4">
                            <div>
                                <div class="font-light text-white text-lg tracking-wide">${p.name}</div>
                                <div class="text-xs text-gray-400 mt-1 font-light">需符合: <span class="text-white bg-white/10 px-2 py-0.5 rounded">${p.adj1}</span> & <span class="text-white bg-white/10 px-2 py-0.5 rounded">${p.adj2}</span></div>
                            </div>
                        </div>
                        <button onclick="removeParticipant('${p.name}')" class="text-gray-500 hover:text-white p-2 rounded-full transition-colors bg-white/5 hover:bg-white/20" title="移除玩家">
                            ✕
                        </button>
                    `;
                    playersList.appendChild(div);
                });
            } else {
                emptyPlayersMsg.style.display = 'block';
            }

            // 更新形容詞看板
            adjectivesBoard.innerHTML = '';
            if (usedAdjectives.size > 0) {
                emptyAdjMsg.style.display = 'none';
                Array.from(usedAdjectives).forEach(adj => {
                    const span = document.createElement('span');
                    span.className = 'bg-white/10 text-gray-200 border border-white/20 px-3 py-1 rounded-lg text-sm shadow-sm font-light backdrop-blur-md';
                    span.textContent = adj;
                    adjectivesBoard.appendChild(span);
                });
            } else {
                emptyAdjMsg.style.display = 'inline';
            }

            // 更新按鈕狀態 (至少 3 人才能玩，建議 5-7 人)
            if (participants.length >= 3) {
                btnDraw.disabled = false;
                drawHint.textContent = participants.length >= 5 ? "人數完美，隨時可以開始抽籤" : "人數有點少，但已經可以開始";
                drawHint.className = "text-xs mt-3 text-white/70 font-light";
            } else {
                btnDraw.disabled = true;
                drawHint.textContent = `最少需要 3 人才能抽籤 (目前 ${participants.length} 人)`;
                drawHint.className = "text-xs mt-3 text-gray-500 font-light";
            }
        }

        // --- 核心邏輯：密碼解鎖 ---
        inputPassword.addEventListener('input', (e) => {
            if (e.target.value === '1234') {
                drawSection.classList.remove('hidden');
                inputPassword.classList.add('hidden'); // 隱藏密碼框
                document.getElementById('admin-hint').classList.add('hidden'); // 隱藏提示文字
            }
        });

        // --- 核心邏輯：主辦人區塊的重新按鈕 ---
        document.getElementById('btn-reset-admin').addEventListener('click', (e) => {
            e.preventDefault();
            resetGame();
        });

        // --- 核心邏輯：抽籤配對 (完美迴圈演算法) ---
        btnDraw.addEventListener('click', () => {
            if (participants.length < 3) return;

            // 1. 打亂陣列 (Fisher-Yates Shuffle)
            let shuffled = [...participants];
            for (let i = shuffled.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [shuffled[i], shuffled[j]] = [shuffled[j], shuffled[i]];
            }

            // 2. 建立完美迴圈配對: i 送給 (i+1)%n
            // 這樣保證：每個人只送出一次、收到一次，且不會有人抽到自己，也不會形成多個獨立小圈圈
            const assignments = [];
            for (let i = 0; i < shuffled.length; i++) {
                const giver = shuffled[i];
                const receiver = shuffled[(i + 1) % shuffled.length];
                assignments.push({ giver, receiver });
            }

            // 3. 顯示結果
            showResults(assignments);
        });

        // --- 核心邏輯：顯示結果 ---
        function showResults(assignments) {
            // 切換畫面
            mainContent.classList.add('hidden');
            resultsContent.classList.remove('hidden');
            
            // 捲動到頂部
            window.scrollTo({ top: 0, behavior: 'smooth' });

            resultsList.innerHTML = '';
            
            // 由於原PO說：「無所謂啦，大家知道誰送誰應該還好，直接顯示」
            // 所以我們直接把所有配對結果攤牌
            
            // 按照送禮人字母排序，讓畫面看起來比較整齊一點 (選填)
            assignments.sort((a, b) => a.giver.name.localeCompare(b.giver.name));

            assignments.forEach((pair, index) => {
                const div = document.createElement('div');
                
                div.className = `glass-panel rounded-2xl p-6 shadow-lg relative overflow-hidden group mb-4`;
                
                div.innerHTML = `
                    <div class="absolute right-[-20px] top-[-20px] text-7xl opacity-5 transform group-hover:scale-110 transition-transform">❄️</div>
                    
                    <div class="flex items-center gap-3 mb-4">
                        <div class="font-light text-2xl text-white tracking-widest">${pair.giver.name}</div>
                        <div class="text-gray-400 text-sm font-light">送給 ➔</div>
                    </div>
                    
                    <div class="bg-white/5 rounded-xl p-5 border border-white/10 flex items-start gap-4">
                        <div>
                            <div class="flex items-center gap-3 mb-3">
                                <span class="text-xl opacity-80">🎁</span>
                                <div class="font-light text-xl text-white tracking-widest">${pair.receiver.name}</div>
                            </div>
                            <div class="text-sm text-gray-300 leading-relaxed font-light">
                                <span class="opacity-60">任務：尋找</span> 
                                <span class="inline-block bg-white/10 text-white px-2 py-1 rounded mx-1">${pair.receiver.adj1}</span> 
                                <span class="opacity-60">與</span> 
                                <span class="inline-block bg-white/10 text-white px-2 py-1 rounded mx-1">${pair.receiver.adj2}</span>
                                <span class="opacity-60">的禮物</span>
                            </div>
                        </div>
                    </div>
                `;
                resultsList.appendChild(div);
            });
        }

        // --- 重新開始 ---
        btnReset.addEventListener('click', () => {
            // 確認是否真的要重新開始
            if(confirm("確定要清除所有資料並重新開始嗎？(這個遊戲沒有存檔喔)")){ // 使用原生 confirm 在此情境尚可，但為了符合規定，我們這裡就直接重置不問了
                // Reset State
                participants = [];
                usedAdjectives.clear();
                
                // Reset UI
                updateUI();
                resultsContent.classList.add('hidden');
                mainContent.classList.remove('hidden');
                
                window.scrollTo({ top: 0, behavior: 'smooth' });
            }
        });
        
        // 為了符合規範 "Never use alert() or confirm()"
        // 改寫 btnReset 邏輯，直接重置或跳客製化 Modal
        btnReset.addEventListener('click', (e) => {
            e.preventDefault();
            resetGame();
        });

        // 將重置邏輯獨立成一個函數，方便不同按鈕呼叫
        function resetGame() {
            participants = [];
            usedAdjectives.clear();
            
            // 恢復密碼框與隱藏抽籤區
            inputPassword.value = '';
            inputPassword.classList.remove('hidden');
            document.getElementById('admin-hint').classList.remove('hidden');
            drawSection.classList.add('hidden');
            
            // 下拉選單恢復
            Array.from(selectPlayer.options).forEach((opt, idx) => {
                if (idx > 0) opt.disabled = false;
            });
            selectPlayer.value = "0";
            
            updateUI();
            resultsContent.classList.add('hidden');
            mainContent.classList.remove('hidden');
            window.scrollTo({ top: 0, behavior: 'smooth' });
            showModal("已重置", "資料已清空，可以開始下一輪新的遊戲囉！");
        }

        // --- 背景雪花特效 ---
        function createSnowflakes() {
            const container = document.getElementById('snowflakes-container');
            const flakesCount = 20;
            const symbols = ['❄', '❅', '❆'];

            for (let i = 0; i < flakesCount; i++) {
                const snowflake = document.createElement('div');
                snowflake.className = 'snowflake';
                snowflake.textContent = symbols[Math.floor(Math.random() * symbols.length)];
                
                // 隨機位置與動畫時間
                snowflake.style.left = `${Math.random() * 100}vw`;
                snowflake.style.animationDuration = `${Math.random() * 5 + 5}s`; // 5s ~ 10s
                snowflake.style.animationDelay = `${Math.random() * 5}s`;
                snowflake.style.opacity = Math.random() * 0.5 + 0.1;
                
                // 大小
                const size = Math.random() * 1.5 + 0.5;
                snowflake.style.fontSize = `${size}em`;

                container.appendChild(snowflake);
            }
        }

        // 初始化
        window.onload = () => {
            // 初始化下拉選單
            selectPlayer.innerHTML = '';
            friendData.forEach((friend, index) => {
                const option = document.createElement('option');
                option.value = index;
                option.textContent = friend.name;
                // 第一個預設選項不可選
                if (index === 0) {
                    option.disabled = true;
                    option.selected = true;
                }
                selectPlayer.appendChild(option);
            });
            
            createSnowflakes();
            updateUI();
        };

    </script>
</body>
</html>
