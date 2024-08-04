
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>ABOT SAHEER</title>

  <link rel="stylesheet" href="styles.css">

    <script <script src="https://cdn.jsdelivr.net/npm/tesseract.js@2.1.1/dist/tesseract.min.js"></script>

   

    <style>

        body {

            font-family: Arial, sans-serif;

            display: flex;

            justify-content: center;

            align-items: flex-start;

            padding: 20px;

        }

        .container {

            max-width: 800px;

            width: 100%;

        }

        .flex-container {

            display: flex;

            gap: 20px;

        }

        .column {

            display: flex;

            flex-direction: column;

            gap: 10px;

        }

        #chatbox {

            width: 60%;

            height: 400px;

            border: 1px solid #ccc;

            padding: 10px;

            overflow-y: auto;

            resize: both;

        }

        .user-list {

            width: 200px;

        }

        .chat-controls {

            display: flex;

            align-items: center;

            gap: 10px;

        }

        .chat-container {

            display: flex;

        }

        .emoji-list {

            display: flex;

            flex-wrap: wrap;

            gap: 5px;

        }

        .emoji-item {

            cursor: pointer;

            font-size: 24px;

        }

        .green {

            color: green;

        }

        .darkgreen {

            color: darkgreen;

        }

        .role-creator {

            color: red;

        }

        .role-owner {

            color: blue;

        }

        .role-admin {

            color: purple;

        }

        .role-member {

            color: black;

        }

        .role-none {

            color: grey;

        }

    </style>

</head>

<body>

    <div class="container">

        <div class="column">

            <div class="flex-container">

                <div>

                    <label for="username">الاسم المستخدم:</label>

                    <input type="text" id="s-bot-s">

                </div>

                <div>

                    <label for="password">الباسورد:</label>

                    <input type="password" id="qaz12345zaq">

                </div>

                <button id="loginButton">اتصال</button>

            </div>



            <div id="status"></div>



            <div class="flex-container">

                <div>

                    <label for="room">الغرفة:</label>

                    <input type="text" id="العقول💞الراقيه">

                    <button id="joinRoomButton">دخول الغرفة</button>

                    <button id="leaveRoomButton">خروج من الغرفة</button>

                    <select id="roomListbox"></select>



                    <div id="joinlog"></div>

 

                </div>

            </div>

            

            <div>

                <input type="text" id="master" placeholder="Bot owner here(Ex. syntax-error)">

                <label for="welcomeCheckbox">تشغيل للترحيب</label>

                <input type="checkbox" id="welcomeCheckbox">

                <label for="spinCheckbox">spin</label>

                <input type="checkbox" id="spinCheckbox">

            </div>

            <div>   

 <input type="checkbox" id="activateQuizCheckbox">

                <label for="activateQuizCheckbox">تشغيل المسابقة</label>              

            </div>

              

 

<form id="quizForm">

     

    <textarea id="questionAnswerInput"placeholder="edit your question here. question format Start With 'p'~paper#Start With 'p'~power# ." rows="5" cols="50"></textarea>



</form>















  

   

            <div class="chat-container">

                <div id="chatbox"></div>

                <div class="user-list">

                    <div id="count"></div>

                    

                    <select id="userListbox" size="10" multiple></select>

                    <ul id="roomlistbox"></ul>

                </div>

            </div>



        <div class="chat-controls">

        <input type="text" id="message" placeholder="Type your message here...">

        <button id="sendMessageButton">Send Message</button>

     

   

     

    </div>



            <div>

                <input type="text" id="target" placeholder="Type your target username here...">

                <button id="banButton">Ban</button>

                <button id="kickButton">Kick</button>

                <button id="memButton">Member</button>

                <button id="adminButton">Admin</button>

                <button id="ownerButton">Owner</button>

                <button id="noneButton">None</button>

            </div>

           <div id="emojiList">

        <!-- Smileys & People -->

        <span class="emoji-item">😀</span>

        <span class="emoji-item">😁</span>

        <span class="emoji-item">😂</span>

        <span class="emoji-item">🤣</span>

        <span class="emoji-item">😃</span>

        <span class="emoji-item">😄</span>

        <span class="emoji-item">😅</span>

        <span class="emoji-item">😆</span>

        <span class="emoji-item">😉</span>

        <span class="emoji-item">😊</span>

        <span class="emoji-item">😋</span>

        <span class="emoji-item">😎</span>

        <span class="emoji-item">😍</span>

        <span class="emoji-item">😘</span>

        <span class="emoji-item">😗</span>

        <span class="emoji-item">😙</span>

        <span class="emoji-item">😚</span>

        <span class="emoji-item">🙂</span>

        <span class="emoji-item">🤗</span>

        <span class="emoji-item">🤔</span>

        <span class="emoji-item">😐</span>

        <span class="emoji-item">😑</span>

        <span class="emoji-item">😶</span>

        <span class="emoji-item">🙄</span>

        <span class="emoji-item">😏</span>

        <span class="emoji-item">😣</span>

        <span class="emoji-item">😥</span>

        <span class="emoji-item">😮</span>

        <span class="emoji-item">🤐</span>

        <span class="emoji-item">😯</span>

        <span class="emoji-item">😪</span>

        <span class="emoji-item">😫</span>

        <span class="emoji-item">😴</span>

        <span class="emoji-item">😌</span>

        <span class="emoji-item">😛</span>

        <span class="emoji-item">😜</span>

        <span class="emoji-item">😝</span>

        <span class="emoji-item">🤤</span>

        <span class="emoji-item">😒</span>

        <span class="emoji-item">😓</span>

        <span class="emoji-item">😔</span>

        <span class="emoji-item">😕</span>

        <span class="emoji-item">🙃</span>

        <span class="emoji-item">🤑</span>

        <span class="emoji-item">😲</span>

        <span class="emoji-item">☹️</span>

        <span class="emoji-item">🙁</span>

        <span class="emoji-item">😖</span>

        <span class="emoji-item">😞</span>

        <span class="emoji-item">😟</span>

        <span class="emoji-item">😤</span>

        <span class="emoji-item">😢</span>

        <span class="emoji-item">😭</span>

        <span class="emoji-item">😦</span>

        <span class="emoji-item">😧</span>

        <span class="emoji-item">😨</span>

        <span class="emoji-item">😩</span>

        <span class="emoji-item">😬</span>

        <span class="emoji-item">😰</span>

        <span class="emoji-item">😱</span>

        <span class="emoji-item">😳</span>

        <span class="emoji-item">😵</span>

        <span class="emoji-item">😡</span>

        <span class="emoji-item">😠</span>

        <span class="emoji-item">😷</span>

        <span class="emoji-item">🤒</span>

        <span class="emoji-item">🤕</span>

        <span class="emoji-item">🤢</span>

        <span class="emoji-item">🤧</span>

        <span class="emoji-item">😇</span>

        <span class="emoji-item">🤠</span>

        <span class="emoji-item">🤡</span>

        <span class="emoji-item">🤥</span>

        <span class="emoji-item">🤓</span>

        <span class="emoji-item">👿</span>

        <span class="emoji-item">👹</span>

        <span class="emoji-item">👺</span>

        <span class="emoji-item">💀</span>

        <span class="emoji-item">👻</span>

        <span class="emoji-item">👽</span>

        <span class="emoji-item">👾</span>

        <span class="emoji-item">🤖</span>



        <!-- Animals & Nature -->

        <span class="emoji-item">🐶</span>

        <span class="emoji-item">🐱</span>

        <span class="emoji-item">🐭</span>

        <span class="emoji-item">🐹</span>

        <span class="emoji-item">🐰</span>

        <span class="emoji-item">🦊</span>

        <span class="emoji-item">🐻</span>

        <span class="emoji-item">🐼</span>

        <span class="emoji-item">🐨</span>

        <span class="emoji-item">🐯</span>

        <span class="emoji-item">🦁</span>

        <span class="emoji-item">🐮</span>

        <span class="emoji-item">🐷</span>

        <span class="emoji-item">🐽</span>

        <span class="emoji-item">🐸</span>

        <span class="emoji-item">🐵</span>

        <span class="emoji-item">🙈</span>

        <span class="emoji-item">🙉</span>

        <span class="emoji-item">🙊</span>

        <span class="emoji-item">🐒</span>

        <span class="emoji-item">🐔</span>

        <span class="emoji-item">🐧</span>

        <span class="emoji-item">🐦</span>

        <span class="emoji-item">🐤</span>

        <span class="emoji-item">🐣</span>

        <span class="emoji-item">🐥</span>

        <span class="emoji-item">🦆</span>

        <span class="emoji-item">🦅</span>

        <span class="emoji-item">🦉</span>

        <span class="emoji-item">🦇</span>

        <span class="emoji-item">🐺</span>

        <span class="emoji-item">🐗</span>

        <span class="emoji-item">🐴</span>

        <span class="emoji-item">🦄</span>

        <span class="emoji-item">🐝</span>

        <span class="emoji-item">🐛</span>

        <span class="emoji-item">🦋</span>

        <span class="emoji-item">🐌</span>

        <span class="emoji-item">🐞</span>

        <span class="emoji-item">🐜</span>

        <span class="emoji-item">🦟</span>

        <span class="emoji-item">🦗</span>

        <span class="emoji-item">🕷️</span>

        <span class="emoji-item">🕸️</span>

        <span class="emoji-item">🐢</span>

        <span class="emoji-item">🐍</span>

        <span class="emoji-item">🦎</span>

        <span class="emoji-item">🦖</span>

        <span class="emoji-item">🦕</span>

        <span class="emoji-item">🐙</span>

        <span class="emoji-item">🦑</span>

        <span class="emoji-item">🦐</span>

        <span class="emoji-item">🦞</span>

        <span class="emoji-item">🦀</span>

        <span class="emoji-item">🐡</span>

        <span class="emoji-item">🐠</span>

        <span class="emoji-item">🐟</span>

        <span class="emoji-item">🐬</span>

        <span class="emoji-item">🐳</span>

        <span class="emoji-item">🐋</span>

        <span class="emoji-item">🦈</span>

        <span class="emoji-item">🐊</span>

        <span class="emoji-item">🐅</span>

        <span class="emoji-item">🐆</span>

        <span class="emoji-item">🦓</span>

        <span class="emoji-item">🦍</span>

        <span class="emoji-item">🐘</span>

        <span class="emoji-item">🦏</span>

        <span class="emoji-item">🦛</span>

        <span class="emoji-item">🐪</span>

        <span class="emoji-item">🐫</span>

        <span class="emoji-item">🦙</span>

        <span class="emoji-item">🦒</span>

        <span class="emoji-item">🐃</span>

        <span class="emoji-item">🐂</span>

        <span class="emoji-item">🐄</span>

        <span class="emoji-item">🐎</span>

        <span class="emoji-item">🐖</span>

        <span class="emoji-item">🐏</span>

        <span class="emoji-item">🐑</span>

        <span class="emoji-item">🐐</span>

        <span class="emoji-item">🦌</span>

        <span class="emoji-item">🐕</span>

        <span class="emoji-item">🐩</span>

        <span class="emoji-item">🦮</span>

        <span class="emoji-item">🐕‍🦺</span>

        <span class="emoji-item">🐈</span>

        <span class="emoji-item">🐈‍⬛</span>

        <span class="emoji-item">🦢</span>

        <span class="emoji-item">🐓</span>

        <span class="emoji-item">🦃</span>

        <span class="emoji-item">🦚</span>

        <span class="emoji-item">🦜</span>

        <span class="emoji-item">🦢</span>

        <span class="emoji-item">🦩</span>

        <span class="emoji-item">🦝</span>

        <span class="emoji-item">🦨</span>

        <span class="emoji-item">🦡</span>

        <span class="emoji-item">🦦</span>

        <span class="emoji-item">🦥</span>

        <span class="emoji-item">🐁</span>

        <span class="emoji-item">🐀</span>

        <span class="emoji-item">🐿️</span>

        <span class="emoji-item">🦔</span>

        <span class="emoji-item">🌵</span>

        <span class="emoji-item">🎄</span>

        <span class="emoji-item">🌲</span>

        <span class="emoji-item">🌳</span>

        <span class="emoji-item">🌴</span>

        <span class="emoji-item">🪵</span>

        <span class="emoji-item">🌱</span>

        <span class="emoji-item">🌿</span>

        <span class="emoji-item">☘️</span>

        <span class="emoji-item">🍀</span>

        <span class="emoji-item">🎍</span>

        <span class="emoji-item">🪴</span>

        <span class="emoji-item">🎋</span>

        <span class="emoji-item">🍃</span>

        <span class="emoji-item">🍂</span>

        <span class="emoji-item">🍁</span>

        <span class="emoji-item">🍄</span>

        <span class="emoji-item">🐚</span>

        <span class="emoji-item">🪨</span>

        <span class="emoji-item">🌾</span>

        <span class="emoji-item">💐</span>

        <span class="emoji-item">🌷</span>

        <span class="emoji-item">🌹</span>

        <span class="emoji-item">🥀</span>

        <span class="emoji-item">🌺</span>

        <span class="emoji-item">🌸</span>

        <span class="emoji-item">🌼</span>

        <span class="emoji-item">🌻</span>

        <span class="emoji-item">🌞</span>

        <span class="emoji-item">🌝</span>

        <span class="emoji-item">🌛</span>

        <span class="emoji-item">🌜</span>

        <span class="emoji-item">🌚</span>

        <span class="emoji-item">🌕</span>

        <span class="emoji-item">🌖</span>

        <span class="emoji-item">🌗</span>

        <span class="emoji-item">🌘</span>

        <span class="emoji-item">🌑</span>

        <span class="emoji-item">🌒</span>

        <span class="emoji-item">🌓</span>

        <span class="emoji-item">🌔</span>

        <span class="emoji-item">🌙</span>

        <span class="emoji-item">🌎</span>

        <span class="emoji-item">🌍</span>

        <span class="emoji-item">🌏</span>

        <span class="emoji-item">🪐</span>

        <span class="emoji-item">💫</span>

        <span class="emoji-item">⭐</span>

        <span class="emoji-item">🌟</span>

        <span class="emoji-item">✨</span>

        <span class="emoji-item">⚡</span>

        <span class="emoji-item">☄️</span>

        <span class="emoji-item">💥</span>

        <span class="emoji-item">🔥</span>

        <span class="emoji-item">🌪️</span>

        <span class="emoji-item">🌈</span>

        <span class="emoji-item">☀️</span>

        <span class="emoji-item">🌤️</span>

        <span class="emoji-item">⛅</span>

        <span class="emoji-item">🌥️</span>

        <span class="emoji-item">☁️</span>

        <span class="emoji-item">🌦️</span>

        <span class="emoji-item">🌧️</span>

        <span class="emoji-item">⛈️</span>

        <span class="emoji-item">🌩️</span>

        <span class="emoji-item">🌨️</span>

        <span class="emoji-item">❄️</span>

        <span class="emoji-item">☃️</span>

        <span class="emoji-item">⛄</span>

        <span class="emoji-item">🌬️</span>

        <span class="emoji-item">💨</span>

        <span class="emoji-item">💧</span>

        <span class="emoji-item">💦</span>

        <span class="emoji-item">☔</span>

        <span class="emoji-item">☂️</span>

        <span class="emoji-item">🌊</span>

        <span class="emoji-item">🌫️</span>



       <!-- Food & Drink -->

<span class="emoji-item">🍇</span>

<span class="emoji-item">🍈</span>

<span class="emoji-item">🍉</span>

<span class="emoji-item">🍊</span>

<span class="emoji-item">🍋</span>

<span class="emoji-item">🍌</span>

<span class="emoji-item">🍍</span>

<span class="emoji-item">🥭</span>

<span class="emoji-item">🍎</span>

<span class="emoji-item">🍏</span>

<span class="emoji-item">🍐</span>

<span class="emoji-item">🍑</span>

<span class="emoji-item">🍒</span>

<span class="emoji-item">🍓</span>

<span class="emoji-item">🫐</span>

<span class="emoji-item">🥝</span>

<span class="emoji-item">🍅</span>

<span class="emoji-item">🫒</span>

<span class="emoji-item">🥥</span>

<span class="emoji-item">🥑</span>

<span class="emoji-item">🍆</span>

<span class="emoji-item">🥔</span>

<span class="emoji-item">🥕</span>

<span class="emoji-item">🌽</span>

<span class="emoji-item">🌶️</span>

<span class="emoji-item">🫑</span>

<span class="emoji-item">🥒</span>

<span class="emoji-item">🥬</span>

<span class="emoji-item">🥦</span>

<span class="emoji-item">🧄</span>

<span class="emoji-item">🧅</span>

<span class="emoji-item">🍄</span>

<span class="emoji-item">🥜</span>

<span class="emoji-item">🌰</span>

<span class="emoji-item">🍞</span>

<span class="emoji-item">🥐</span>

<span class="emoji-item">🥖</span>

<span class="emoji-item">🫓</span>

<span class="emoji-item">🥨</span>

<span class="emoji-item">🥯</span>

<span class="emoji-item">🥞</span>

<span class="emoji-item">🧇</span>

<span class="emoji-item">🧀</span>

<span class="emoji-item">🍖</span>

<span class="emoji-item">🍗</span>

<span class="emoji-item">🥩</span>

<span class="emoji-item">🥓</span>

<span class="emoji-item">🍔</span>

<span class="emoji-item">🍟</span>

<span class="emoji-item">🍕</span>

<span class="emoji-item">🌭</span>

<span class="emoji-item">🥪</span>

<span class="emoji-item">🌮</span>

<span class="emoji-item">🌯</span>

<span class="emoji-item">🫔</span>

<span class="emoji-item">🥙</span>

<span class="emoji-item">🧆</span>

<span class="emoji-item">🥚</span>

<span class="emoji-item">🍳</span>

<span class="emoji-item">🥘</span>

<span class="emoji-item">🍲</span>

<span class="emoji-item">🫕</span>

<span class="emoji-item">🥣</span>

<span class="emoji-item">🥗</span>

<span class="emoji-item">🍿</span>

<span class="emoji-item">🧈</span>

<span class="emoji-item">🧂</span>

<span class="emoji-item">🥫</span>

<span class="emoji-item">🍱</span>

<span class="emoji-item">🍘</span>

<span class="emoji-item">🍙</span>

<span class="emoji-item">🍚</span>

<span class="emoji-item">🍛</span>

<span class="emoji-item">🍜</span>

<span class="emoji-item">🍝</span>

<span class="emoji-item">🍠</span>

<span class="emoji-item">🍢</span>

<span class="emoji-item">🍣</span>

<span class="emoji-item">🍤</span>

<span class="emoji-item">🍥</span>

<span class="emoji-item">🥮</span>

<span class="emoji-item">🍡</span>

<span class="emoji-item">🥟</span>

<span class="emoji-item">🥠</span>

<span class="emoji-item">🥡</span>

<span class="emoji-item">🦪</span>

<span class="emoji-item">🍦</span>

<span class="emoji-item">🍧</span>

<span class="emoji-item">🍨</span>

<span class="emoji-item">🍩</span>

<span class="emoji-item">🍪</span>

<span class="emoji-item">🎂</span>

<span class="emoji-item">🍰</span>

<span class="emoji-item">🧁</span>

<span class="emoji-item">🥧</span>

<span class="emoji-item">🍫</span>

<span class="emoji-item">🍬</span>

<span class="emoji-item">🍭</span>

<span class="emoji-item">🍮</span>

<span class="emoji-item">🍯</span>

<span class="emoji-item">🍼</span>

<span class="emoji-item">🥛</span>

<span class="emoji-item">☕</span>

<span class="emoji-item">🫖</span>

<span class="emoji-item">🍵</span>

<span class="emoji-item">🍶</span>

<span class="emoji-item">🍾</span>

<span class="emoji-item">🍷</span>

<span class="emoji-item">🍸</span>

<span class="emoji-item">🍹</span>

<span class="emoji-item">🍺</span>

<span class="emoji-item">🍻</span>

<span class="emoji-item">🥂</span>

<span class="emoji-item">🥃</span>

<span class="emoji-item">🥤</span>

<span class="emoji-item">🧃</span>

<span class="emoji-item">🧉</span>

<span class="emoji-item">🧊</span>



<!-- Travel & Places -->

<span class="emoji-item">🛖</span>

<span class="emoji-item">🏠</span>

<span class="emoji-item">🏡</span>

<span class="emoji-item">🏢</span>

<span class="emoji-item">🏣</span>

<span class="emoji-item">🏤</span>

<span class="emoji-item">🏥</span>

<span class="emoji-item">🏦</span>

<span class="emoji-item">🏨</span>

<span class="emoji-item">🏩</span>

<span class="emoji-item">🏪</span>

<span

<!-- Travel & Places (continued) -->

<span class="emoji-item">🏫</span>

<span class="emoji-item">🏬</span>

<span class="emoji-item">🏭</span>

<span class="emoji-item">🏯</span>

<span class="emoji-item">🏰</span>

<span class="emoji-item">💒</span>

<span class="emoji-item">🗼</span>

<span class="emoji-item">🗽</span>

<span class="emoji-item">⛪</span>

<span class="emoji-item">🕌</span>

<span class="emoji-item">🛕</span>

<span class="emoji-item">🕍</span>

<span class="emoji-item">⛩️</span>

<span class="emoji-item">🕋</span>

<span class="emoji-item">⛲</span>

<span class="emoji-item">⛺</span>

<span class="emoji-item">🌁</span>

<span class="emoji-item">🌃</span>

<span class="emoji-item">🏙️</span>

<span class="emoji-item">🌄</span>

<span class="emoji-item">🌅</span>

<span class="emoji-item">🌆</span>

<span class="emoji-item">🌇</span>

<span class="emoji-item">🌉</span>

<span class="emoji-item">♨️</span>

<span class="emoji-item">🎠</span>

<span class="emoji-item">🎡</span>

<span class="emoji-item">🎢</span>

<span class="emoji-item">💈</span>

<span class="emoji-item">🎪</span>

<span class="emoji-item">🚂</span>

<span class="emoji-item">🚃</span>

<span class="emoji-item">🚄</span>

<span class="emoji-item">🚅</span>

<span class="emoji-item">🚆</span>

<span class="emoji-item">🚇</span>

<span class="emoji-item">🚈</span>

<span class="emoji-item">🚉</span>

<span class="emoji-item">🚊</span>

<span class="emoji-item">🚝</span>

<span class="emoji-item">🚞</span>

<span class="emoji-item">🚋</span>

<span class="emoji-item">🚌</span>

<span class="emoji-item">🚍</span>

<span class="emoji-item">🚎</span>

<span class="emoji-item">🚐</span>

<span class="emoji-item">🚑</span>

<span class="emoji-item">🚒</span>

<span class="emoji-item">🚓</span>

<span class="emoji-item">🚔</span>

<span class="emoji-item">🚕</span>

<span class="emoji-item">🚖</span>

<span class="emoji-item">🚗</span>

<span class="emoji-item">🚘</span>

<span class="emoji-item">🚙</span>

<span class="emoji-item">🚚</span>

<span class="emoji-item">🚛</span>

<span class="emoji-item">🚜</span>

<span class="emoji-item">🏎️</span>

<span class="emoji-item">🏍️</span>

<span class="emoji-item">🛵</span>

<span class="emoji-item">🦽</span>

<span class="emoji-item">🦼</span>

<span class="emoji-item">🛺</span>

<span class="emoji-item">🚲</span>

<span class="emoji-item">🛴</span>

<span class="emoji-item">🛹</span>

<span class="emoji-item">🛼</span>

<span class="emoji-item">🚏</span>

<span class="emoji-item">🛣️</span>

<span class="emoji-item">🛤️</span>

<span class="emoji-item">🛢️</span>

<span class="emoji-item">⛽</span>

<span class="emoji-item">🚨</span>

<span class="emoji-item">🚥</span>

<span class="emoji-item">🚦</span>

<span class="emoji-item">🛑</span>

<span class="emoji-item">🚧</span>

<span class="emoji-item">⚓</span>

<span class="emoji-item">⛵</span>

<span class="emoji-item">🛶</span>

<span class="emoji-item">🚤</span>

<span class="emoji-item">🛳️</span>

<span class="emoji-item">⛴️

<!-- Travel & Places (continued) -->

<span class="emoji-item">⛴️</span>

<span class="emoji-item">🛥️</span>

<span class="emoji-item">🚢</span>

<span class="emoji-item">✈️</span>

<span class="emoji-item">🛩️</span>

<span class="emoji-item">🛫</span>

<span class="emoji-item">🛬</span>

<span class="emoji-item">🪂</span>

<span class="emoji-item">🪁</span>

<span class="emoji-item">🚁</span>

<span class="emoji-item">🛰️</span>

<span class="emoji-item">🚀</span>

<span class="emoji-item">🛸</span>

<span class="emoji-item">🌠</span>

<span class="emoji-item">🌌</span>

<span class="emoji-item">🎇</span>

<span class="emoji-item">🎆</span>

<span class="emoji-item">🌈</span>

<span class="emoji-item">🌅</span>

<span class="emoji-item">🌄</span>

<span class="emoji-item">🌠</span>

<span class="emoji-item">🌟</span>













    

    </div>











       

            <div>

                <label for="debugBox">Debug Messages:</label>

                <textarea id="debugBox" rows="10" cols="50" readonly></textarea>

            </div>

        </div>

    </div>

    <script src="app.js"></script>

</body>

</html>

