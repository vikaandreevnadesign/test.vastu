<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Васту-компас • Проверь своё пространство</title>

    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&family=Inter:wght@300;400;500&display=swap" rel="stylesheet">

    <style>
        :root {
            --milk: #F2EBDD;
            --emerald: #0F4F3F;
            --emerald-light: #1a6b55;
            --gold: #D4A24C;
            --gold-dark: #b8862c;
            --graphite: #2B2D2E;
            --bordo: #6B1E2A;
            --olive: #4A5A35;
            --sand: #E8D4A2;
            --white: #FFFDF9;
            --border-subtle: rgba(15, 79, 63, 0.12);
            --text-main: #2B2D2E;
            --text-soft: rgba(43, 45, 46, 0.65);
            --card-bg: rgba(255, 253, 249, 0.85);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--milk);
            font-family: 'Inter', sans-serif;
            color: var(--text-main);
            min-height: 100vh;
            padding: 20px;
            -webkit-tap-highlight-color: transparent;
            position: relative;
            overflow-x: hidden;
        }

        /* Архитектурный фон — сетка планировки */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
            opacity: 0.04;
            background-image:
                linear-gradient(var(--emerald) 0.5px, transparent 0.5px),
                linear-gradient(90deg, var(--emerald) 0.5px, transparent 0.5px);
            background-size: 40px 40px;
        }

        /* Архитектурные акценты — крупные линии */
        body::after {
            content: '';
            position: fixed;
            top: -100px;
            right: -150px;
            width: 600px;
            height: 800px;
            pointer-events: none;
            z-index: 0;
            opacity: 0.03;
            border: 2px solid var(--emerald);
            border-radius: 8px;
            transform: rotate(15deg);
        }

        .container {
            max-width: 780px;
            margin: 0 auto;
            background: var(--card-bg);
            border-radius: 24px;
            padding: 44px;
            border: 1px solid var(--border-subtle);
            box-shadow: 0 8px 40px rgba(43, 45, 46, 0.08), 0 2px 8px rgba(43, 45, 46, 0.04);
            position: relative;
            z-index: 2;
            backdrop-filter: blur(10px);
        }

        /* Декоративный уголок */
        .corner-accent {
            position: absolute;
            top: 24px;
            right: 24px;
            width: 48px;
            height: 48px;
            border-top: 2px solid var(--gold);
            border-right: 2px solid var(--gold);
            opacity: 0.4;
            pointer-events: none;
        }

        .screen {
            display: none;
        }
        .screen.active {
            display: block;
        }

        .subtitle {
            font-size: 12px;
            text-transform: uppercase;
            letter-spacing: 3px;
            color: var(--gold-dark);
            margin-bottom: 8px;
            font-weight: 500;
        }

        h1 {
            font-family: 'Playfair Display', serif;
            font-size: 34px;
            font-weight: 700;
            color: var(--text-main);
            margin-bottom: 10px;
            line-height: 1.2;
        }

        .accent-text {
            color: var(--emerald);
            font-style: italic;
        }

        .description {
            font-size: 15px;
            color: var(--text-soft);
            margin-bottom: 24px;
            line-height: 1.7;
        }

        .btn {
            display: inline-block;
            padding: 16px 36px;
            font-family: 'Inter', sans-serif;
            font-size: 14px;
            font-weight: 500;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1.5px;
            text-decoration: none;
            touch-action: manipulation;
            -webkit-appearance: none;
            position: relative;
            z-index: 10;
        }

        .btn-primary {
            background-color: var(--emerald);
            color: var(--white);
        }
        .btn-primary:hover {
            background-color: var(--emerald-light);
            transform: translateY(-2px);
            box-shadow: 0 12px 28px rgba(15, 79, 63, 0.25);
        }
        .btn-primary:active {
            transform: translateY(0);
            box-shadow: none;
        }

        .btn-gold {
            background-color: transparent;
            border: 1.5px solid var(--gold);
            color: var(--gold-dark);
            font-weight: 600;
        }
        .btn-gold:hover {
            background-color: rgba(212, 162, 76, 0.08);
            transform: translateY(-2px);
        }
        .btn-gold:active {
            transform: translateY(0);
        }

        .btn-outline {
            background: transparent;
            border: 1.5px solid var(--emerald);
            color: var(--emerald);
            font-weight: 600;
        }
        .btn-outline:hover {
            background-color: rgba(15, 79, 63, 0.06);
            transform: translateY(-2px);
        }

        .btn:disabled,
        .btn[disabled] {
            opacity: 0.35;
            cursor: not-allowed;
            pointer-events: none;
        }

        /* Шаги */
        .step-indicator {
            display: flex;
            gap: 8px;
            margin-bottom: 28px;
            align-items: center;
        }
        .step-dot {
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: rgba(15, 79, 63, 0.15);
            transition: all 0.3s ease;
        }
        .step-dot.active {
            background-color: var(--emerald);
            box-shadow: 0 0 0 4px rgba(15, 79, 63, 0.1);
        }
        .step-dot.done {
            background-color: var(--gold);
        }
        .step-line {
            flex: 1;
            height: 1px;
            background-color: rgba(15, 79, 63, 0.1);
            max-width: 30px;
        }
        .step-label {
            font-size: 11px;
            color: var(--text-soft);
            letter-spacing: 1px;
            text-transform: uppercase;
            margin-left: 4px;
        }

        /* Загрузка планировки */
        .upload-zone {
            border: 2px dashed rgba(15, 79, 63, 0.25);
            border-radius: 16px;
            padding: 50px 30px;
            text-align: center;
            cursor: pointer;
            transition: all 0.3s ease;
            background-color: rgba(242, 235, 221, 0.4);
            margin-bottom: 20px;
            position: relative;
        }
        .upload-zone:hover {
            border-color: var(--emerald);
            background-color: rgba(15, 79, 63, 0.03);
        }
        .upload-zone.has-image {
            border-style: solid;
            border-color: var(--emerald);
            padding: 16px;
        }
        .upload-icon {
            font-size: 48px;
            margin-bottom: 12px;
            opacity: 0.6;
        }
        .upload-text {
            font-size: 14px;
            color: var(--text-soft);
            margin-bottom: 4px;
        }
        .upload-hint {
            font-size: 12px;
            color: rgba(43, 45, 46, 0.35);
        }
        .upload-zone input {
            display: none;
        }
        .upload-preview {
            max-width: 100%;
            max-height: 350px;
            border-radius: 8px;
            display: none;
        }
        .upload-zone.has-image .upload-preview {
            display: block;
            margin: 0 auto;
        }
        .upload-zone.has-image .upload-placeholder {
            display: none;
        }

        /* Компас */
        .compass-section {
            text-align: center;
            margin: 20px 0;
        }
        .compass-label {
            font-size: 13px;
            color: var(--text-soft);
            margin-bottom: 12px;
            letter-spacing: 1px;
            text-transform: uppercase;
        }
        .compass-control {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 16px;
        }
        .compass-rotate-btn {
            width: 44px;
            height: 44px;
            border-radius: 50%;
            border: 1.5px solid var(--emerald);
            background: transparent;
            color: var(--emerald);
            font-size: 20px;
            cursor: pointer;
            transition: all 0.2s ease;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .compass-rotate-btn:hover {
            background: rgba(15, 79, 63, 0.06);
        }
        .compass-visual {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 2px solid var(--gold);
            position: relative;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(212, 162, 76, 0.04);
            transition: transform 0.3s ease;
        }
        .compass-arrow {
            font-size: 36px;
            color: var(--bordo);
        }
        .compass-n {
            position: absolute;
            top: -24px;
            font-size: 13px;
            font-weight: 700;
            color: var(--bordo);
            letter-spacing: 1px;
        }
        .compass-degree {
            font-size: 14px;
            color: var(--text-soft);
            margin-top: 8px;
        }

        /* Сетка */
        .grid-overlay-wrap {
            position: relative;
            margin: 24px 0;
            border-radius: 12px;
            overflow: hidden;
            border: 1px solid rgba(15, 79, 63, 0.1);
            background: rgba(242, 235, 221, 0.3);
            min-height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .grid-overlay-wrap.no-image {
            background: rgba(242, 235, 221, 0.5);
            padding: 40px;
            text-align: center;
            color: var(--text-soft);
            font-size: 14px;
        }
        .grid-canvas-wrap {
            position: relative;
            display: inline-block;
            line-height: 0;
        }
        .grid-canvas-wrap img {
            max-width: 100%;
            max-height: 450px;
            border-radius: 4px;
            display: block;
        }
        .grid-svg {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        .grid-zone {
            position: absolute;
            cursor: pointer;
            pointer-events: auto;
            transition: all 0.2s ease;
            background-color: transparent;
        }
        .grid-zone:hover {
            background-color: rgba(15, 79, 63, 0.12) !important;
            z-index: 5;
        }
        .grid-zone.marked {
            background-color: rgba(107, 30, 42, 0.15) !important;
            border: 1.5px solid rgba(107, 30, 42, 0.5) !important;
        }
        .grid-zone-label {
            position: absolute;
            pointer-events: none;
            font-size: 10px;
            font-weight: 600;
            color: var(--text-main);
            text-align: center;
            opacity: 0.7;
            letter-spacing: 0.5px;
            text-transform: uppercase;
            line-height: 1.3;
        }

        /* Подсказка */
        .zone-tooltip {
            background: var(--white);
            border: 1px solid rgba(15, 79, 63, 0.2);
            border-radius: 12px;
            padding: 18px 20px;
            box-shadow: 0 12px 36px rgba(43, 45, 46, 0.12);
            font-size: 13px;
            line-height: 1.7;
            color: var(--text-main);
            margin-top: 16px;
            display: none;
            animation: fadeIn 0.25s ease;
        }
        .zone-tooltip.active {
            display: block;
        }
        .zone-tooltip .zone-name {
            font-family: 'Playfair Display', serif;
            font-size: 18px;
            font-weight: 700;
            color: var(--emerald);
            margin-bottom: 6px;
        }
        .zone-tooltip .zone-good {
            color: var(--emerald);
            margin-top: 8px;
        }
        .zone-tooltip .zone-bad {
            color: var(--bordo);
            margin-top: 4px;
        }
        .zone-tooltip .btn-mark {
            margin-top: 10px;
            font-size: 12px;
            padding: 10px 20px;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(-6px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Результат */
        .result-card {
            background: rgba(242, 235, 221, 0.5);
            border-radius: 14px;
            padding: 20px;
            margin-bottom: 12px;
            border-left: 3px solid var(--bordo);
        }
        .result-card.resolved {
            border-left-color: var(--emerald);
            opacity: 0.6;
        }
        .result-card .zone-title {
            font-weight: 600;
            color: var(--text-main);
            margin-bottom: 4px;
        }
        .result-card .zone-issue {
            font-size: 13px;
            color: var(--text-soft);
            line-height: 1.5;
        }
        .summary-count {
            font-family: 'Playfair Display', serif;
            font-size: 48px;
            font-weight: 700;
            color: var(--bordo);
            text-align: center;
            margin: 16px 0 4px;
        }
        .summary-text {
            text-align: center;
            color: var(--text-soft);
            font-size: 14px;
            margin-bottom: 20px;
        }

        .actions-row {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 20px;
        }

        .send-block {
            margin-top: 24px;
            padding-top: 20px;
            border-top: 1px solid rgba(15, 79, 63, 0.1);
            text-align: center;
        }
        .send-block p {
            font-size: 13px;
            color: var(--text-soft);
            margin-bottom: 12px;
        }
        .send-block input {
            width: 100%;
            padding: 14px 16px;
            background: rgba(242, 235, 221, 0.6);
            border: 1px solid rgba(15, 79, 63, 0.15);
            border-radius: 10px;
            color: var(--text-main);
            font-family: 'Inter', sans-serif;
            font-size: 14px;
            margin-bottom: 10px;
            outline: none;
            transition: border-color 0.2s ease;
        }
        .send-block input:focus {
            border-color: var(--gold);
            background: var(--white);
        }
        .send-block input::placeholder {
            color: rgba(43, 45, 46, 0.3);
        }
        .send-success {
            color: var(--emerald);
            font-size: 14px;
            margin-top: 10px;
            display: none;
            font-weight: 500;
        }

        .footer-note {
            text-align: center;
            margin-top: 28px;
            font-size: 11px;
            color: rgba(43, 45, 46, 0.3);
            letter-spacing: 1px;
        }

        @media (max-width: 600px) {
            .container {
                padding: 24px 16px;
                border-radius: 16px;
            }
            h1 {
                font-size: 26px;
            }
            .upload-zone {
                padding: 30px 16px;
            }
            .grid-overlay-wrap {
                min-height: 200px;
            }
            .compass-visual {
                width: 72px;
                height: 72px;
            }
            .corner-accent {
                display: none;
            }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="corner-accent"></div>

    <!-- ============ ЭКРАН 1: СТАРТ + ЗАГРУЗКА ============ -->
    <div id="screenUpload" class="screen active">
        <div class="subtitle">Блок 2 • Васту-компас</div>
        <h1>Где <span class="accent-text">твоя</span><br>точка опоры</h1>
        <p class="description">
            Пространство либо работает на тебя, либо высасывает силы.
            Загрузи план своей квартиры и проверь, что находится в каждой зоне Васту.
            Это не гадание — это архитектура твоей жизни.
        </p>

        <div class="step-indicator">
            <span class="step-dot active"></span>
            <span class="step-line"></span>
            <span class="step-dot"></span>
            <span class="step-line"></span>
            <span class="step-dot"></span>
            <span class="step-label">шаг 1 из 3</span>
        </div>

        <div class="upload-zone" id="uploadZone">
            <div class="upload-placeholder">
                <div class="upload-icon">📐</div>
                <div class="upload-text">Загрузи план квартиры</div>
                <div class="upload-hint">Скрин, фото схемы, рисунок от руки • JPG, PNG, WEBP</div>
            </div>
            <input type="file" id="fileInput" accept="image/*">
            <img class="upload-preview" id="uploadPreview" alt="План квартиры">
        </div>

        <button type="button" class="btn btn-outline" id="btnSkipUpload" style="margin-right: 8px;">НЕТ ПЛАНА</button>
        <button type="button" class="btn btn-primary" id="btnToCompass" disabled>ДАЛЕЕ: НАСТРОИТЬ КОМПАС</button>
    </div>

    <!-- ============ ЭКРАН 2: КОМПАС + СЕТКА ============ -->
    <div id="screenCompass" class="screen">
        <div class="subtitle">Блок 2 • Васту-компас</div>
        <h1>Направь <span class="accent-text">север</span></h1>
        <p class="description">
            Поверни компас так, чтобы стрелка указывала на север в твоей квартире.
            Не знаешь где север? Открой компас в телефоне, встань лицом к входной двери и посмотри.
        </p>

        <div class="step-indicator">
            <span class="step-dot done"></span>
            <span class="step-line"></span>
            <span class="step-dot active"></span>
            <span class="step-line"></span>
            <span class="step-dot"></span>
            <span class="step-label">шаг 2 из 3</span>
        </div>

        <div class="compass-section">
            <div class="compass-label">Поверни компас — укажи направление севера</div>
            <div class="compass-control">
                <button type="button" class="compass-rotate-btn" id="btnRotateLeft">↺</button>
                <div class="compass-visual" id="compassVisual">
                    <span class="compass-n">N</span>
                    <span class="compass-arrow">↑</span>
                </div>
                <button type="button" class="compass-rotate-btn" id="btnRotateRight">↻</button>
            </div>
            <div class="compass-degree" id="compassDegree">Север: 0°</div>
        </div>

        <div class="grid-overlay-wrap" id="gridWrap">
            <div class="grid-canvas-wrap" id="gridCanvasWrap">
                <img id="gridImage" alt="План" style="display:none;">
                <svg class="grid-svg" id="gridSvg"></svg>
            </div>
        </div>

        <!-- Подсказка по зоне -->
        <div class="zone-tooltip" id="zoneTooltip">
            <div class="zone-name" id="tooltipName"></div>
            <div id="tooltipBody"></div>
            <div class="zone-good" id="tooltipGood"></div>
            <div class="zone-bad" id="tooltipBad"></div>
            <button type="button" class="btn btn-gold btn-mark" id="btnMarkZone">ОТМЕТИТЬ КАК ПРОБЛЕМНУЮ</button>
        </div>

        <div class="actions-row" style="margin-top: 20px;">
            <button type="button" class="btn btn-outline" id="btnBackUpload">← НАЗАД</button>
            <button type="button" class="btn btn-primary" id="btnToResult">ДАЛЕЕ: РЕЗУЛЬТАТ</button>
        </div>
    </div>

    <!-- ============ ЭКРАН 3: РЕЗУЛЬТАТ ============ -->
    <div id="screenResult" class="screen">
        <div class="subtitle">Блок 2 • Результат проверки</div>
        <h1>Твой <span class="accent-text">Васту-разбор</span></h1>
        <p class="description">
            Ты проверил своё пространство через Васту-компас. Вот что получилось.
            Красным отмечены зоны, которые требуют внимания.
        </p>

        <div class="step-indicator">
            <span class="step-dot done"></span>
            <span class="step-line"></span>
            <span class="step-dot done"></span>
            <span class="step-line"></span>
            <span class="step-dot active"></span>
            <span class="step-label">результат</span>
        </div>

        <div class="summary-count" id="summaryCount">0</div>
        <div class="summary-text">проблемных зон из 9</div>

        <div id="resultZonesList"></div>

        <div class="send-block">
            <p>Хочешь полную диагностику и корректировку пространства? Оставь ник — свяжусь и разберём всё детально.</p>
            <input type="text" id="sendNick" placeholder="@твой_ник_в_телеграм">
            <button type="button" class="btn btn-primary" id="btnSend">ОТПРАВИТЬ НА ДИАГНОСТИКУ</button>
            <div class="send-success" id="sendOk">✓ Отправлено! Я напишу тебе в ближайшее время.</div>
        </div>

        <div class="actions-row">
            <button type="button" class="btn btn-outline" id="btnBackCompass">← НАЗАД К КОМПАСУ</button>
            <button type="button" class="btn btn-gold" id="btnRestart">НАЧАТЬ ЗАНОВО</button>
        </div>
    </div>

    <div class="footer-note">Метод «Точка сборки» • Виктория Кокурина</div>
</div>

<script>
    (function() {
        // ===== ДАННЫЕ ЗОН ВАСТУ =====
        const zoneData = {
            'north': {
                name: 'Север',
                title: 'Север — зона финансов и денег',
                good: 'Должно быть: чистота, вода (фонтан, картина с водой), зеркало, зелень, сейф.',
                bad: 'Не должно быть: туалет, мусор, кладовка, хлам, спальня, тёмные углы.'
            },
            'northeast': {
                name: 'Северо-восток',
                title: 'Северо-восток — зона мудрости и ясности',
                good: 'Должно быть: комната для медитации, алтарь, книги, чистота, свет, вода.',
                bad: 'Не должно быть: туалет, спальня, кухня, тяжёлая мебель, мусор.'
            },
            'east': {
                name: 'Восток',
                title: 'Восток — зона здоровья и социального статуса',
                good: 'Должно быть: окна, свет, открытое пространство, зелень, минимум мебели.',
                bad: 'Не должно быть: туалет, кладовка, спальня, входная дверь, тяжёлые шкафы.'
            },
            'southeast': {
                name: 'Юго-восток',
                title: 'Юго-восток — зона энергии и денежного потока',
                good: 'Должно быть: кухня, огонь, плита, свечи, активность, деньги.',
                bad: 'Не должно быть: туалет, вода (раковина отдельно от плиты — ок), спальня, ванная.'
            },
            'south': {
                name: 'Юг',
                title: 'Юг — зона славы, признания и уверенности',
                good: 'Должно быть: гостиная, awards, дипломы, красный цвет, свет, активность.',
                bad: 'Не должно быть: туалет, ванная, кладовка, тёмные помещения, спальня.'
            },
            'southwest': {
                name: 'Юго-запад',
                title: 'Юго-запад — зона стабильности и защиты',
                good: 'Должно быть: спальня хозяев, тяжёлая мебель, закрытое пространство, земляные тона.',
                bad: 'Не должно быть: туалет, входная дверь, кухня, детская комната.'
            },
            'west': {
                name: 'Запад',
                title: 'Запад — зона обучения, творчества и детей',
                good: 'Должно быть: детская, кабинет, мастерская, книги, инструменты.',
                bad: 'Не должно быть: туалет, спальня хозяев, ванная, кладовка.'
            },
            'northwest': {
                name: 'Северо-запад',
                title: 'Северо-запад — зона поддержки, связей и путешествий',
                good: 'Должно быть: гостевая комната, коридор, прихожая, место для встреч.',
                bad: 'Не должно быть: туалет, кухня, спальня хозяев, кладовка.'
            },
            'center': {
                name: 'Центр',
                title: 'Центр — зона баланса и здоровья всей семьи',
                good: 'Должно быть: свободное пространство, свет, воздух, ничего лишнего.',
                bad: 'Не должно быть: туалет, лестница, колонны, тяжёлая мебель, стены, кладовка.'
            }
        };

        const zoneKeys = ['north', 'northeast', 'east', 'southeast', 'south', 'southwest', 'west', 'northwest', 'center'];
        let markedZones = {};  // key -> true
        let compassAngle = 0;  // градусы
        let uploadedImage = null;
        let currentTooltipZone = null;

        // Инициализация
        zoneKeys.forEach(function(k) { markedZones[k] = false; });

        // ===== DOM =====
        const screens = {
            upload: document.getElementById('screenUpload'),
            compass: document.getElementById('screenCompass'),
            result: document.getElementById('screenResult')
        };

        function showScreen(id) {
            Object.values(screens).forEach(function(s) { s.classList.remove('active'); });
            screens[id].classList.add('active');
        }

        // ===== ЭКРАН 1: ЗАГРУЗКА =====
        const uploadZone = document.getElementById('uploadZone');
        const fileInput = document.getElementById('fileInput');
        const uploadPreview = document.getElementById('uploadPreview');
        const btnToCompass = document.getElementById('btnToCompass');
        const btnSkipUpload = document.getElementById('btnSkipUpload');

        uploadZone.addEventListener('click', function(e) {
            if (e.target !== fileInput) fileInput.click();
        });
        uploadZone.addEventListener('touchend', function(e) {
            if (e.target !== fileInput) {
                e.preventDefault();
                fileInput.click();
            }
        });

        fileInput.addEventListener('change', function() {
            const file = fileInput.files[0];
            if (!file) return;
            const reader = new FileReader();
            reader.onload = function(ev) {
                uploadedImage = ev.target.result;
                uploadPreview.src = uploadedImage;
                uploadZone.classList.add('has-image');
                btnToCompass.disabled = false;
                btnToCompass.removeAttribute('disabled');
            };
            reader.readAsDataURL(file);
        });

        btnToCompass.addEventListener('click', function() { goToCompass(); });
        btnToCompass.addEventListener('touchend', function(e) { e.preventDefault(); goToCompass(); });

        btnSkipUpload.addEventListener('click', function() { goToCompass(); });
        btnSkipUpload.addEventListener('touchend', function(e) { e.preventDefault(); goToCompass(); });

        function goToCompass() {
            renderCompassGrid();
            showScreen('compass');
        }

        // ===== ЭКРАН 2: КОМПАС + СЕТКА =====
        const compassVisual = document.getElementById('compassVisual');
        const compassDegree = document.getElementById('compassDegree');
        const gridImage = document.getElementById('gridImage');
        const gridSvg = document.getElementById('gridSvg');
        const gridCanvasWrap = document.getElementById('gridCanvasWrap');
        const gridWrap = document.getElementById('gridWrap');
        const zoneTooltip = document.getElementById('zoneTooltip');
        const tooltipName = document.getElementById('tooltipName');
        const tooltipBody = document.getElementById('tooltipBody');
        const tooltipGood = document.getElementById('tooltipGood');
        const tooltipBad = document.getElementById('tooltipBad');
        const btnMarkZone = document.getElementById('btnMarkZone');

        function updateCompassVisual() {
            compassVisual.style.transform = 'rotate(' + compassAngle + 'deg)';
            compassDegree.textContent = 'Север: ' + compassAngle + '°';
        }

        document.getElementById('btnRotateLeft').addEventListener('click', function() {
            compassAngle = (compassAngle - 15 + 360) % 360;
            updateCompassVisual();
            renderGrid();
        });
        document.getElementById('btnRotateRight').addEventListener('click', function() {
            compassAngle = (compassAngle + 15) % 360;
            updateCompassVisual();
            renderGrid();
        });
        // Touch
        document.getElementById('btnRotateLeft').addEventListener('touchend', function(e) {
            e.preventDefault();
            compassAngle = (compassAngle - 15 + 360) % 360;
            updateCompassVisual();
            renderGrid();
        });
        document.getElementById('btnRotateRight').addEventListener('touchend', function(e) {
            e.preventDefault();
            compassAngle = (compassAngle + 15) % 360;
            updateCompassVisual();
            renderGrid();
        });

        function renderCompassGrid() {
            if (uploadedImage) {
                gridImage.src = uploadedImage;
                gridImage.style.display = 'block';
                gridWrap.classList.remove('no-image');
            } else {
                gridImage.style.display = 'none';
                gridWrap.classList.add('no-image');
                gridWrap.innerHTML = '<div style="padding:60px;text-align:center;color:var(--text-soft);font-size:14px;">'
                    + '<div style="font-size:48px;margin-bottom:12px;">🏠</div>'
                    + 'Без плана — работаем по сетке.<br>Представь свою квартиру и сверяй зоны мысленно.</div>';
            }
            updateCompassVisual();
            renderGrid();
        }

        function renderGrid() {
            // Очищаем старые зоны
            gridSvg.innerHTML = '';
            const oldZones = gridCanvasWrap.querySelectorAll('.grid-zone, .grid-zone-label');
            oldZones.forEach(function(el) { el.remove(); });

            if (!uploadedImage) {
                zoneTooltip.classList.remove('active');
                return;
            }

            // Ждём рендера изображения
            var imgEl = gridImage;
            var w = imgEl.clientWidth || imgEl.naturalWidth || 400;
            var h = imgEl.clientHeight || imgEl.naturalHeight || 300;

            var cols = 3;
            var rows = 3;
            var cellW = w / cols;
            var cellH = h / rows;

            // Сетка зон: массив [key, col, row]
            // При угле 0: север сверху. col 0=запад, col 2=восток; row 0=север, row 2=юг
            var gridMap = [
                { key: 'northwest', col: 0, row: 0 },
                { key: 'north', col: 1, row: 0 },
                { key: 'northeast', col: 2, row: 0 },
                { key: 'west', col: 0, row: 1 },
                { key: 'center', col: 1, row: 1 },
                { key: 'east', col: 2, row: 1 },
                { key: 'southwest', col: 0, row: 2 },
                { key: 'south', col: 1, row: 2 },
                { key: 'southeast', col: 2, row: 2 }
            ];

            // Рисуем SVG сетку
            var svgLines = '';
            for (var i = 1; i < cols; i++) {
                svgLines += '<line x1="' + (i * cellW) + '" y1="0" x2="' + (i * cellW) + '" y2="' + h + '" stroke="rgba(15,79,63,0.2)" stroke-width="1" stroke-dasharray="6,4"/>';
            }
            for (var j = 1; j < rows; j++) {
                svgLines += '<line x1="0" y1="' + (j * cellH) + '" x2="' + w + '" y2="' + (j * cellH) + '" stroke="rgba(15,79,63,0.2)" stroke-width="1" stroke-dasharray="6,4"/>';
            }
            gridSvg.innerHTML = svgLines;

            // Создаём кликабельные зоны
            gridMap.forEach(function(item) {
                var zone = document.createElement('div');
                zone.className = 'grid-zone';
                if (markedZones[item.key]) zone.classList.add('marked');
                zone.style.left = (item.col * cellW) + 'px';
                zone.style.top = (item.row * cellH) + 'px';
                zone.style.width = cellW + 'px';
                zone.style.height = cellH + 'px';
                zone.setAttribute('data-zone', item.key);

                zone.addEventListener('click', function(e) {
                    e.stopPropagation();
                    showTooltip(item.key);
                });
                zone.addEventListener('touchend', function(e) {
                    e.stopPropagation();
                    e.preventDefault();
                    showTooltip(item.key);
                });

                gridCanvasWrap.appendChild(zone);

                // Подпись
                var label = document.createElement('div');
                label.className = 'grid-zone-label';
                label.textContent = zoneData[item.key].name;
                label.style.left = (item.col * cellW + 4) + 'px';
                label.style.top = (item.row * cellH + 4) + 'px';
                label.style.width = (cellW - 8) + 'px';
                gridCanvasWrap.appendChild(label);
            });

            zoneTooltip.classList.remove('active');
        }

        function showTooltip(key) {
            currentTooltipZone = key;
            var data = zoneData[key];
            tooltipName.textContent = data.title;
            tooltipBody.textContent = '';
            tooltipGood.textContent = data.good;
            tooltipBad.textContent = data.bad;

            if (markedZones[key]) {
                btnMarkZone.textContent = '✓ ОТМЕЧЕНО КАК ПРОБЛЕМНАЯ';
                btnMarkZone.style.borderColor = 'var(--bordo)';
                btnMarkZone.style.color = 'var(--bordo)';
            } else {
                btnMarkZone.textContent = 'ОТМЕТИТЬ КАК ПРОБЛЕМНУЮ';
                btnMarkZone.style.borderColor = 'var(--gold)';
                btnMarkZone.style.color = 'var(--gold-dark)';
            }

            zoneTooltip.classList.add('active');
        }

        btnMarkZone.addEventListener('click', function() {
            if (!currentTooltipZone) return;
            markedZones[currentTooltipZone] = !markedZones[currentTooltipZone];
            // Обновить визуал сетки
            renderGrid();
            // Обновить тултип
            showTooltip(currentTooltipZone);
        });
        btnMarkZone.addEventListener('touchend', function(e) {
            e.preventDefault();
            if (!currentTooltipZone) return;
            markedZones[currentTooltipZone] = !markedZones[currentTooltipZone];
            renderGrid();
            showTooltip(currentTooltipZone);
        });

        document.getElementById('btnToResult').addEventListener('click', function() { showResultScreen(); });
        document.getElementById('btnToResult').addEventListener('touchend', function(e) { e.preventDefault(); showResultScreen(); });

        document.getElementById('btnBackUpload').addEventListener('click', function() { showScreen('upload'); });
        document.getElementById('btnBackUpload').addEventListener('touchend', function(e) { e.preventDefault(); showScreen('upload'); });

        // ===== ЭКРАН 3: РЕЗУЛЬТАТ =====
        function showResultScreen() {
            var problemCount = 0;
            zoneKeys.forEach(function(k) { if (markedZones[k]) problemCount++; });

            document.getElementById('summaryCount').textContent = problemCount;

            var html = '';
            zoneKeys.forEach(function(k) {
                if (markedZones[k]) {
                    var d = zoneData[k];
                    html += '<div class="result-card">' +
                        '<div class="zone-title">⚠ ' + d.name + '</div>' +
                        '<div class="zone-issue">' + d.bad.replace('Не должно быть: ', '') + '</div>' +
                        '</div>';
                }
            });
            if (problemCount === 0) {
                html = '<div class="result-card resolved">' +
                    '<div class="zone-title">✓ Всё чисто</div>' +
                    '<div class="zone-issue">Ты не отметил ни одной проблемной зоны. Либо твоё пространство в гармонии, либо стоит перепроверить внимательнее.</div>' +
                    '</div>';
            }
            document.getElementById('resultZonesList').innerHTML = html;
            document.getElementById('sendOk').style.display = 'none';
            document.getElementById('sendNick').value = '';

            showScreen('result');
        }

        document.getElementById('btnBackCompass').addEventListener('click', function() { showScreen('compass'); });
        document.getElementById('btnBackCompass').addEventListener('touchend', function(e) { e.preventDefault(); showScreen('compass'); });

        document.getElementById('btnRestart').addEventListener('click', function() {
            zoneKeys.forEach(function(k) { markedZones[k] = false; });
            compassAngle = 0;
            uploadedImage = null;
            uploadPreview.src = '';
            uploadZone.classList.remove('has-image');
            btnToCompass.disabled = true;
            btnToCompass.setAttribute('disabled', 'disabled');
            fileInput.value = '';
            gridImage.style.display = 'none';
            gridSvg.innerHTML = '';
            var old = gridCanvasWrap.querySelectorAll('.grid-zone, .grid-zone-label');
            old.forEach(function(el) { el.remove(); });
            zoneTooltip.classList.remove('active');
            document.getElementById('gridWrap').classList.remove('no-image');
            document.getElementById('gridWrap').innerHTML = '<div class="grid-canvas-wrap" id="gridCanvasWrap">' +
                '<img id="gridImage" alt="План" style="display:none;">' +
                '<svg class="grid-svg" id="gridSvg"></svg></div>';
            showScreen('upload');
        });
        document.getElementById('btnRestart').addEventListener('touchend', function(e) { e.preventDefault();
            document.getElementById('btnRestart').click();
        });

        // ===== ОТПРАВКА =====
        document.getElementById('btnSend').addEventListener('click', sendResult);
        document.getElementById('btnSend').addEventListener('touchend', function(e) { e.preventDefault(); sendResult(); });

        function sendResult() {
            var nick = document.getElementById('sendNick').value.trim();
            if (!nick) nick = 'не указан';

            var problemList = [];
            zoneKeys.forEach(function(k) {
                if (markedZones[k]) problemList.push(zoneData[k].name);
            });
            var problemStr = problemList.length > 0 ? problemList.join(', ') : 'нет';

            var formData = new FormData();
            formData.append('Тест', 'Васту-компас');
            formData.append('Проблемные зоны', problemStr);
            formData.append('Количество проблем', problemList.length + ' из 9');
            formData.append('Угол севера', compassAngle + '°');
            formData.append('Ник в Telegram', nick);
            formData.append('Приветственное сообщение', '🔥 НОВЫЙ ЛИД С ВАСТУ-КОМПАСА');

            fetch('https://formspree.io/f/xwvygpnq', {
                method: 'POST',
                body: formData,
                headers: { 'Accept': 'application/json' }
            })
            .then(function(response) {
                if (response.ok) {
                    document.getElementById('sendOk').style.display = 'block';
                    document.getElementById('sendNick').value = '';
                } else {
                    alert('Не удалось. Напиши вручную: @kowiktori');
                }
            })
            .catch(function() {
                alert('Не удалось. Напиши вручную: @kowiktori');
            });
        }

        // ===== ИНИЦИАЛИЗАЦИЯ =====
        updateCompassVisual();
    })();
</script>

</body>
</html>
