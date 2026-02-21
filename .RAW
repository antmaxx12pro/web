<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Antmaxx12 - Latino Y Castellano</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Helvetica Neue', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #000;
            color: white;
            min-height: 100vh;
            overflow-x: hidden;
        }

        /* Hero Section */
        .hero-section {
            position: relative;
            width: 100%;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: flex-start;
            overflow: hidden;
        }

        .hero-video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: -2;
        }

        .hero-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(
                90deg,
                rgba(0, 0, 0, 0.9) 0%,
                rgba(0, 0, 0, 0.7) 40%,
                rgba(0, 0, 0, 0.5) 60%,
                rgba(0, 0, 0, 0.3) 80%,
                transparent 100%
            ),
            linear-gradient(
                180deg,
                transparent 0%,
                rgba(0, 0, 0, 0.3) 50%,
                rgba(0, 0, 0, 0.8) 100%
            );
            z-index: -1;
        }

        .hero-content {
            max-width: 1800px;
            width: 100%;
            padding: 0 4%;
            z-index: 1;
        }

        .hero-badge {
            display: inline-block;
            background: linear-gradient(45deg, #e50914, #ff4757);
            padding: 8px 20px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
            margin-bottom: 1rem;
            letter-spacing: 1px;
            text-transform: uppercase;
            box-shadow: 0 4px 15px rgba(229, 9, 20, 0.4);
            animation: pulse 2s ease-in-out infinite;
        }

        @keyframes pulse {
            0%, 100% {
                transform: scale(1);
                box-shadow: 0 4px 15px rgba(229, 9, 20, 0.4);
            }
            50% {
                transform: scale(1.05);
                box-shadow: 0 6px 20px rgba(229, 9, 20, 0.6);
            }
        }

        .hero-title {
            font-size: 4.5rem;
            font-weight: 900;
            margin-bottom: 1rem;
            line-height: 1.1;
            background: linear-gradient(120deg, #ffffff 0%, #ff6b6b 50%, #e50914 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            filter: drop-shadow(0 4px 20px rgba(229, 9, 20, 0.3));
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .hero-subtitle {
            font-size: 1.3rem;
            color: #e5e5e5;
            margin-bottom: 2rem;
            max-width: 600px;
            line-height: 1.5;
            font-weight: 300;
        }

        .hero-buttons {
            display: flex;
            gap: 1rem;
            align-items: center;
        }

        .btn-play {
            display: flex;
            align-items: center;
            gap: 0.8rem;
            background: linear-gradient(45deg, #e50914, #ff4757);
            color: white;
            padding: 1rem 2.5rem;
            border: none;
            border-radius: 8px;
            font-size: 1.1rem;
            font-weight: 700;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            box-shadow: 0 4px 20px rgba(229, 9, 20, 0.4);
        }

        .btn-play:hover {
            background: linear-gradient(45deg, #c8070f, #e63946);
            transform: translateY(-2px);
            box-shadow: 0 8px 30px rgba(229, 9, 20, 0.6);
        }

        .btn-info {
            display: flex;
            align-items: center;
            gap: 0.8rem;
            background: rgba(255, 255, 255, 0.2);
            color: white;
            padding: 1rem 2rem;
            border: 2px solid rgba(255, 255, 255, 0.3);
            border-radius: 8px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            backdrop-filter: blur(10px);
        }

        .btn-info:hover {
            background: rgba(255, 255, 255, 0.3);
            border-color: rgba(255, 255, 255, 0.5);
            transform: translateY(-2px);
        }

        .play-icon, .info-icon {
            width: 24px;
            height: 24px;
            fill: currentColor;
        }

        /* Header */
        .netflix-header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 999;
            background: linear-gradient(180deg, rgba(0,0,0,0.8) 10%, transparent);
            padding: 20px 4%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: all 0.4s ease;
        }

        .netflix-header.scrolled {
            background: rgba(20, 20, 20, 0.95);
            backdrop-filter: blur(15px);
        }

        .netflix-logo {
            font-size: 1.8em;
            font-weight: bold;
            color: #e50914;
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .logo-icon {
            width: 32px;
            height: 32px;
            background: linear-gradient(45deg, #e50914, #ff4757);
            border-radius: 8px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
        }

        .header-nav {
            display: flex;
            align-items: center;
            gap: 2em;
        }

        .nav-links {
            display: flex;
            gap: 1.5em;
            list-style: none;
        }

        .nav-links a {
            color: #e5e5e5;
            text-decoration: none;
            font-size: 0.95em;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 0.5rem 1rem;
            border-radius: 20px;
        }

        .nav-links a:hover,
        .nav-links a.active {
            color: white;
            background: rgba(255, 255, 255, 0.1);
        }

        .profile-button {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            color: white;
            padding: 0.6rem 1.2rem;
            border-radius: 20px;
            cursor: pointer;
            font-size: 0.9rem;
            font-weight: 500;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .profile-button:hover {
            background: rgba(255, 255, 255, 0.2);
            border-color: rgba(255, 255, 255, 0.4);
        }

        /* Main Content - Hidden initially */
        .main-content {
            display: none;
            min-height: 100vh;
            background: linear-gradient(135deg, #0f0f0f 0%, #1a1a1a 50%, #2d2d2d 100%);
        }

        .main-content.active {
            display: block;
        }

        .container {
            max-width: 1800px;
            margin: 0 auto;
            padding: 100px 20px 20px;
        }

        .section-header {
            text-align: center;
            margin-bottom: 2rem;
            padding: 3rem 0;
            background: linear-gradient(135deg, rgba(229, 9, 20, 0.1) 0%, rgba(0, 0, 0, 0.3) 100%);
            border-radius: 15px;
            position: relative;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .section-title {
            font-size: 3.5rem;
            font-weight: 900;
            text-transform: uppercase;
            letter-spacing: 4px;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, #e50914, #ff6b6b, #e50914);
            background-size: 200% auto;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: shimmer 3s linear infinite;
            position: relative;
            z-index: 1;
        }

        @keyframes shimmer {
            0% {
                background-position: 0% center;
            }
            100% {
                background-position: 200% center;
            }
        }

        .section-subtitle {
            font-size: 1.2rem;
            opacity: 0.8;
            font-weight: 300;
        }

        .search-bar {
            display: flex;
            gap: 20px;
            margin: 30px auto;
            max-width: 900px;
            padding: 0 20px;
        }

        #search-input {
            flex-grow: 1;
            padding: 16px 24px;
            border: none;
            border-radius: 30px;
            font-size: 16px;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }

        #search-input:focus {
            outline: none;
            box-shadow: 0 6px 30px rgba(229, 9, 20, 0.3);
            transform: translateY(-2px);
        }

        #sort-select {
            padding: 16px 24px;
            border: none;
            border-radius: 30px;
            font-size: 16px;
            background: rgba(255, 255, 255, 0.95);
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }

        .filter-tabs {
            display: flex;
            gap: 1rem;
            margin: 2rem 0;
            justify-content: center;
            flex-wrap: wrap;
        }

        .filter-tab {
            padding: 0.8rem 1.5rem;
            background: rgba(255, 255, 255, 0.1);
            border: none;
            border-radius: 25px;
            color: white;
            cursor: pointer;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .filter-tab.active {
            background: linear-gradient(45deg, #e50914, #ff4757);
            transform: translateY(-2px);
        }

        .filter-tab:hover {
            background: rgba(255, 255, 255, 0.2);
        }

        #results {
            display: grid;
            gap: 25px;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            padding: 20px;
        }

        .anime-card {
            background: linear-gradient(145deg, rgba(255, 255, 255, 0.98) 0%, rgba(245, 245, 245, 0.95) 100%);
            border-radius: 20px;
            overflow: hidden;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.15);
            display: flex;
            flex-direction: column;
            position: relative;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .anime-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 20px 40px rgba(229, 9, 20, 0.3), 0 0 60px rgba(229, 9, 20, 0.1);
            border: 1px solid rgba(229, 9, 20, 0.3);
        }

        .anime-number {
            position: absolute;
            top: 15px;
            left: 15px;
            background: linear-gradient(45deg, rgba(0, 0, 0, 0.9), rgba(0, 0, 0, 0.7));
            color: white;
            padding: 8px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: bold;
            z-index: 2;
        }

        .anime-card.premium::before {
            content: '🔒 Premium';
            position: absolute;
            top: 15px;
            right: 15px;
            background: linear-gradient(45deg, rgba(255, 215, 0, 0.9), rgba(255, 165, 0, 0.9));
            padding: 8px 12px;
            border-radius: 20px;
            color: #000;
            font-size: 0.8rem;
            font-weight: bold;
            z-index: 2;
        }

        .anime-image-container {
            width: 100%;
            padding-top: 140%;
            position: relative;
            overflow: hidden;
        }

        .anime-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.4s ease;
        }

        .anime-card:hover .anime-image {
            transform: scale(1.1);
        }

        .anime-info {
            padding: 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            background: linear-gradient(180deg, rgba(255, 255, 255, 0.95) 0%, rgba(250, 250, 250, 0.95) 100%);
        }

        .anime-title {
            font-size: 1.1rem;
            color: #333;
            margin-bottom: 8px;
            font-weight: 700;
            overflow: hidden;
            text-overflow: ellipsis;
            white-space: nowrap;
            line-height: 1.3;
        }

        .anime-description {
            color: #666;
            font-size: 0.9rem;
            flex-grow: 1;
            overflow: hidden;
            text-overflow: ellipsis;
            display: -webkit-box;
            -webkit-line-clamp: 2;
            -webkit-box-orient: vertical;
            line-height: 1.4;
            margin-bottom: 15px;
        }

        .anime-actions {
            display: flex;
            gap: 0.5rem;
        }

        .watch-button {
            flex: 1;
            padding: 12px;
            background: linear-gradient(45deg, #e50914, #ff4757);
            color: white;
            text-align: center;
            text-decoration: none;
            border-radius: 25px;
            font-weight: bold;
            transition: all 0.3s ease;
            font-size: 0.95rem;
            box-shadow: 0 4px 15px rgba(229, 9, 20, 0.3);
            border: none;
            cursor: pointer;
        }

        .watch-button:hover {
            background: linear-gradient(45deg, #c8070f, #e63946);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(229, 9, 20, 0.4);
        }

        .favorite-button {
            padding: 12px;
            background: rgba(255, 255, 255, 0.2);
            border: 2px solid rgba(229, 9, 20, 0.3);
            border-radius: 25px;
            cursor: pointer;
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
        }

        .favorite-button.active {
            background: linear-gradient(45deg, #e50914, #ff4757);
            border-color: #e50914;
        }

        /* Profile Setup Modal */
        .profile-modal {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            z-index: 9999;
            display: none;
            align-items: center;
            justify-content: center;
            backdrop-filter: blur(10px);
        }

        .profile-modal.active {
            display: flex;
        }

        .profile-modal-content {
            background: linear-gradient(145deg, #1a1a1a, #2d2d2d);
            padding: 3rem;
            border-radius: 20px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            max-width: 500px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
        }

        .modal-close {
            position: absolute;
            top: 1rem;
            right: 1rem;
            background: none;
            border: none;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            transition: background 0.3s ease;
        }

        .modal-close:hover {
            background: rgba(255, 255, 255, 0.1);
        }

        .form-group {
            margin-bottom: 1.5rem;
            text-align: left;
        }

        .form-label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 400;
            color: #e5e5e5;
        }

        .form-input {
            width: 100%;
            padding: 0.75rem;
            border: 1px solid #333;
            border-radius: 10px;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 1rem;
        }

        .form-input:focus {
            outline: none;
            border-color: #e50914;
            box-shadow: 0 0 10px rgba(229, 9, 20, 0.3);
        }

        .avatar-selection {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            gap: 1rem;
            margin-top: 1rem;
        }

        .avatar-option {
            width: 100%;
            aspect-ratio: 1;
            border-radius: 10px;
            cursor: pointer;
            border: 2px solid transparent;
            transition: border-color 0.3s ease;
            object-fit: cover;
        }

        .avatar-option.selected {
            border-color: #e50914;
            box-shadow: 0 0 15px rgba(229, 9, 20, 0.5);
        }

        .checkbox-container {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .checkbox {
            width: 18px;
            height: 18px;
            accent-color: #e50914;
        }

        .btn-primary {
            background: linear-gradient(45deg, #e50914, #ff4757);
            color: white;
            border: none;
            padding: 0.75rem 2rem;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            font-weight: bold;
            transition: all 0.3s ease;
            width: 100%;
        }

        .btn-primary:hover {
            background: linear-gradient(45deg, #c8070f, #e63946);
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(229, 9, 20, 0.4);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-title {
                font-size: 2.8rem;
            }

            .hero-subtitle {
                font-size: 1.1rem;
            }

            .hero-buttons {
                flex-direction: column;
                align-items: stretch;
            }

            .btn-play, .btn-info {
                justify-content: center;
            }

            .nav-links {
                display: none;
            }

            .search-bar {
                flex-direction: column;
                gap: 15px;
            }

            #results {
                grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
                gap: 20px;
            }
        }

        @media (max-width: 480px) {
            .hero-content {
                padding: 0 5%;
            }

            .hero-title {
                font-size: 2.2rem;
            }

            .profile-modal-content {
                padding: 2rem;
            }

            .avatar-selection {
                grid-template-columns: repeat(3, 1fr);
            }
        }

        /* Loading animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .hero-content > * {
            animation: fadeInUp 0.8s ease-out;
        }

        .hero-title {
            animation-delay: 0.2s;
        }

        .hero-subtitle {
            animation-delay: 0.4s;
        }

        .hero-buttons {
            animation-delay: 0.6s;
        }

        /* Scrollbar Styling */
        ::-webkit-scrollbar {
            width: 8px;
        }

        ::-webkit-scrollbar-track {
            background: rgba(255, 255, 255, 0.1);
        }

        ::-webkit-scrollbar-thumb {
            background: linear-gradient(45deg, #e50914, #ff4757);
            border-radius: 4px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: linear-gradient(45deg, #c8070f, #e63946);
        }

        mark {
            background: linear-gradient(45deg, #ffd700, #ffed4e);
            padding: 2px 4px;
            border-radius: 4px;
            color: #333;
        }

        .hero-video {
            filter: brightness(0.9) contrast(1.1);
        }

        .section-header {
            position: relative;
            overflow: hidden;
        }

        .section-header::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(229, 9, 20, 0.1) 0%, transparent 70%);
            animation: rotate 20s linear infinite;
        }

        @keyframes rotate {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }

        .anime-image {
            filter: brightness(1.05) saturate(1.1);
        }

        .anime-card:hover .anime-image {
            filter: brightness(1.1) saturate(1.2);
        }

        .btn-play, .btn-info, .watch-button, .filter-tab {
            position: relative;
            overflow: hidden;
        }

        .btn-play::before, .btn-info::before, .watch-button::before, .filter-tab::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.3);
            transform: translate(-50%, -50%);
            transition: width 0.6s, height 0.6s;
        }

        .btn-play:hover::before, .btn-info:hover::before,
        .watch-button:hover::before, .filter-tab:hover::before {
            width: 300px;
            height: 300px;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="netflix-header" id="netflix-header">
        <a href="#" class="netflix-logo" onclick="showHero()">
            <div class="logo-icon">A</div>
            Antmaxx12 
        </a>
        
        <nav class="header-nav">
            <ul class="nav-links">
                <li><a href="#" onclick="showAnimeSection()">Inicio</a></li>
                <li><a href="#" onclick="showAnimeSection()">Series</a></li>
                <li><a href="#" onclick="showAnimeSection()">Películas</a></li>
                <li><a href="#" onclick="showAnimeSection()">Novedades</a></li>
                <li><a href="#" onclick="setFilter('favorites'); showAnimeSection()">Mi lista</a></li>
            </ul>
            
            <button class="profile-button" onclick="openProfileModal()">
                👤 Perfil
            </button>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="hero-section" class="hero-section">
        <video id="hero-video" class="hero-video" autoplay loop playsinline>
            <source src="https://uiparadox.co.uk/templates/animetube/v2/assets/media/videos/hero_banner.mp4" type="video/mp4">
            <!-- Fallback to a placeholder if video doesn't load -->
        </video>
        
        <div class="hero-overlay"></div>
        
        <div class="hero-content">
            <div class="hero-badge">Nuevo Lanzamiento</div>
            <h1 class="hero-title">Naruto Clein</h1>
            <p class="hero-subtitle">
                Únete a la aventura épica del ninja más poderoso. 
                Descubre miles de episodios de anime en latino y castellano.
                Sumérgete en un mundo de acción, aventura y emociones sin límites.
            </p>
            <div class="hero-buttons">
                <button class="btn-play" onclick="startWatching()">
                    <svg class="play-icon" viewBox="0 0 24 24">
                        <path d="M8 5v14l11-7z"/>
                    </svg>
                    Play Now
                </button>
                <button class="btn-info" onclick="showMoreInfo()">
                    <svg class="info-icon" viewBox="0 0 24 24">
                        <circle cx="12" cy="12" r="10"/>
                        <path d="M12 16v-4"/>
                        <path d="M12 8h.01"/>
                    </svg>
                    More Info
                </button>
            </div>
        </div>
    </section>

    <!-- Main Content -->
    <div id="main-content" class="main-content">
        <div class="container">
            <header class="section-header">
                <h1 class="section-title">Anime</h1>
                <p class="section-subtitle">Latino y Castellano</p>
            </header>

            <div class="filter-tabs">
                <button class="filter-tab active" onclick="setFilter('all')">Todos</button>
                <button class="filter-tab" onclick="setFilter('favorites')">Favoritos</button>
                <button class="filter-tab" onclick="setFilter('recent')">Recientes</button>
                <button class="filter-tab" onclick="setFilter('action')">Acción</button>
                <button class="filter-tab" onclick="setFilter('romance')">Romance</button>
                <button class="filter-tab" onclick="setFilter('comedy')">Comedia</button>
            </div>

            <div class="search-bar">
                <input type="text" id="search-input" placeholder="Buscar anime..." aria-label="Buscar anime">
                <select id="sort-select" aria-label="Ordenar anime">
                    <option value="asc">A-Z</option>
                    <option value="desc">Z-A</option>
                    <option value="rating">Mejor Valorados</option>
                    <option value="recent">Más Recientes</option>
                </select>
            </div>

            <div id="results" role="list" aria-label="Lista de anime"></div>
        </div>
    </div>

    <!-- Profile Setup Modal -->
    <div id="profile-modal" class="profile-modal">
        <div class="profile-modal-content">
            <button class="modal-close" onclick="closeProfileModal()">&times;</button>
            <h2 style="margin-bottom: 1rem; text-align: center; font-size: 2rem;">Configurar Perfil</h2>
            
            <form id="profile-form" onsubmit="createProfile(event)">
                <div class="form-group">
                    <label class="form-label">Tu nombre</label>
                    <input type="text" id="profile-name-input" class="form-input" placeholder="Ingresa tu nombre" required maxlength="15">
                </div>
                
                <div class="form-group">
                    <label class="form-label">Elige tu avatar</label>
                    <div class="avatar-selection" id="avatar-selection">
                        <!-- Avatar options will be loaded here -->
                    </div>
                </div>
                
                <div class="form-group">
                    <div class="checkbox-container">
                        <input type="checkbox" id="kids-profile" class="checkbox">
                        <label for="kids-profile" class="form-label">Perfil para niños (contenido filtrado)</label>
                    </div>
                </div>
                
                <button type="submit" class="btn-primary">Guardar Perfil</button>
            </form>
        </div>
    </div>

    <script>
        const PREMIUM_KEY = "35326911poderoso200";

        // Global variables
        let userProfile = null;
        let premiumUnlocked = false;
        let currentFilter = 'all';
        let selectedAvatar = null;
        let xKeyPressCount = 0;

        // Netflix profile avatars
        const avatars = [
            'https://occ-0-2794-2219.1.nflxso.net/dnm/api/v6/K6hjPJd6cR6FpVELC5Pd6ovHRSk/AAAABdpkabKqQAxyWzo6QW_ZnPz1IZLqlmNfK-t4L1VIeV1DY00JhLo_LMVFp936keDxj-V5UELAVJrU--iUUY2MaDxQSSO-0qw.png?r=e6e',
            'https://occ-0-2794-2219.1.nflxso.net/dnm/api/v6/K6hjPJd6cR6FpVELC5Pd6ovHRSk/AAAABbme8JMz4rEKFJhtzpOKWFJ_6qX-0y5wwWyYvBhWS0VKFLa289dZ5zvRBfdisU1KuFBVxBRfMdxZstRNaTmmyJuBdBVZ_8t5NoDaLRnWyODSeed8UlKVEhAvVnhTAdHm5Q.png?r=1d4',
            'https://occ-0-2794-2219.1.nflxso.net/dnm/api/v6/K6hjPJd6cR6FpVELC5Pd6ovHRSk/AAAABWpIYvZ9cNtfMxaJfnfEKsLHgKGdmgZvRDt_WZ3NmqQpel8lcuLdHHoKHm6qM-NjRpDOqBTOZkIzXNm_heEjWQXDdAmfIhXh1jl_x7zt2dQQwevqaQBoLVRqRMd5EnuIkQ.png?r=bd7',
            'https://occ-0-2794-2219.1.nflxso.net/dnm/api/v6/K6hjPJd6cR6FpVELC5Pd6ovHRSk/AAAABfNXUMVXGhnCZwPI1kxKOqeeeTls1fIl3JNIy7rOZRov0-6VLzjMZx8soYHdF0yxWqxdufp1rP_GzjZG_EBt4dUitGXOzxhMpA.png?r=a41',
            'https://occ-0-2794-2219.1.nflxso.net/dnm/api/v6/K6hjPJd6cR6FpVELC5Pd6ovHRSk/AAAAFZ_p0__2ljGVCEoNMnlgCaFbZVTnNcNcoJoQCHD_SUkCEP6xzGHI5ZnDJYUBwpdnJd9LcGVQOisdkobe9TF3J3mmeLVjbkUMaA.png?r=229',
            'https://via.placeholder.com/150/e50914/fff?text=😊',
            'https://via.placeholder.com/150/ff6b6b/fff?text=🎭',
            'https://via.placeholder.com/150/4ecdc4/fff?text=🎨'
        ];

        const animeList = [
            

 ["Isekai Mokushiroku Mynoghra: Hametsu no Bunmei de Hajimeru Sekai Seifuku", "       ", "https://imgs.search.brave.com/BnAmbSRoISd-BpDvaAOnZzT0r1IAUbaxXUY3LjcjQ0o/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9hbmlt/ZXNnYW1lcy5jYy93/cC1jb250ZW50L3Vw/bG9hZHMvMjAyNS8w/Ny9hc3Npc3Rpci1p/c2VrYWktbW9rdXNo/aXJva3UtbXlub2do/cmEtaGFtZXRzdS1u/by1idW5tZWktZGUt/aGFqaW1lcnUtc2Vr/YWktc2VpZnVrdS10/b2Rvcy1vcy1lcGlz/b2Rpb3MtbGVnZW5k/YWRvLWFuaW1lcy1n/YW1lcy1zY2FsZWQu/anBn", "https://mega.nz/folder/BWMnyQgT#4X1SbDuuC_Rg2CuR45inZA"],
  ["Kimi to Boku no Saigo no Senjou, Aruiwa Sekai ga Hajimaru Seisen", "       ", "https://i.pinimg.com/736x/01/3f/78/013f78ba09c5b17c2d5c27d1a3b46ea4.jpg", "https://mega.nz/folder/BWMnyQgT#4X1SbDuuC_Rg2CuR45inZA"],
  ["Saikyou no Ousama, Nidome no Jinsei wa Nani wo Suru", "       ", "https://i.pinimg.com/736x/01/3f/78/013f78ba09c5b17c2d5c27d1a3b46ea4.jpg", "https://mega.nz/folder/BWMnyQgT#4X1SbDuuC_Rg2CuR45inZA"],
            ["Black Clover", "Temporada Completa", "https://is.gd/lz5XnW", "https://mega.nz/folder/hS9mVSSS#chDvUqfPEcw_55b6vDGhYQ"],
            ["Tokyo Ghoul", "Serie Completa", "https://is.gd/jqGXTP", "https://mega.nz/folder/JKNRRJrS#XmfCqAsF4NIAhlEf5YAMMw"],
            ["Rimuru Tempest", "Tensei Shitara Slime", "https://i.pinimg.com/736x/b1/6c/2b/b16c2b3d71be24d403d8b90f3b7f74f9.jpg", "https://mega.nz/folder/ELMDAbJR#RPSBlJUNwHS2mHEHh9UNRA"],
            ["Hunter x Hunter", "Serie Completa", "https://is.gd/bu92x3", "https://mega.nz/folder/BWMnyQgT#4X1SbDuuC_Rg2CuR45inZA"],
            ["Sword Art Online", "Temporada Completa", "https://is.gd/yYyKtq", "https://mega.nz/folder/EGNT0SqI#12ypspR4SDYi-sPDbG9W4w"],
            ["Overlord", "Serie Completa", "https://is.gd/eaJ7MO", "https://mega.nz/folder/kHkXmQrK#vHitrWaLdS4wQ0BLLy5IdQ"],
            ["Kimetsu no Yaiba", "Demon Slayer", "https://is.gd/SssjZM", "https://mega.nz/folder/leUkGRQQ#fUSQI8sXTKTxVG2FYf_wvg"],
            ["Jigokuraku", "Serie Completa", "https://is.gd/SjvrQo", "https://mega.nz/folder/8aEiFKKK#87IvL5hnqFSVmnGmOcbGNQ"],
            ["Mob Psycho 100", "Temporadas Completas", "https://is.gd/4vjQLm", "https://mega.nz/folder/JPNQxDCJ#2RmH8KPao9jTbZiRCdzhrg"],
            ["Akuma Kun", "Serie 2023", "https://is.gd/kulvxj", "https://mega.nz/folder/BaNFBCoQ#iGagSrJjsO9qJWlkroK7kA"],
            ["Date live", "no", "  https://i.pinimg.com/736x/d5/e7/98/d5e7981a104e9c3a605e76a0eab5d86e.jpg                                                                                                  ", "https://mega.nz/folder/dHMQwJKK#34ZI_UG6nJ-Ka6dWqfV-_g"],
            ["Dr Stone", "Todas las temporadas", "https://is.gd/Wltpsa", "https://mega.nz/folder/NOkVTQKa#2btJH6-Sb69gJtAt5p1dMQ"],
            ["Edens Zero", "ㅤㅤ", "https://is.gd/JnTnz6", "https://mega.nz/folder/QP0CiTxD#3hiJUVGqiJt4AaJmPPQchQ"],
            ["Damachi", "ㅤㅤ", "https://is.gd/2ipX33", "https://mega.nz/folder/Af1hUb7Q#cucJL5BmJ87exshk1Tk_MQ"],
            ["Jujutsu Kaisen", "ㅤㅤ", "https://i.pinimg.com/736x/76/e8/38/76e838db7bb8687c195512565900102b.jpg", "https://mega.nz/folder/BPEkSBTD#dgMjb8DLf7vilHt4WkiUSg"],
            ["Tokyo Revengers", "ㅤㅤ", "https://is.gd/NpeGy7", "https://mega.nz/folder/FblywYyQ#guUqEeZOS_cGaABTBxHDJw"],
            ["Kenja no mago", "ㅤㅤ", "https://is.gd/DliFwp", "https://mega.nz/folder/gH9AFaLB#4kWdrEu-XesW4zaGqSuayw"],
            ["ReMonster", "ㅤㅤ", "https://is.gd/WNd0FD", "https://mega.nz/folder/pHNHSaSA#RCdwTnJXID3Hxq-6Kloavw"],
            ["No Game No Life", "ㅤㅤ", "https://is.gd/saubSg", "https://mega.nz/folder/tS8wyZCL#LzyEhYOET9dGTIgHh3uRqQ"],
            ["Akame ga Kill!", "ㅤㅤ", "https://i.pinimg.com/736x/e7/2e/fc/e72efc3928d7b4e3d3a53918860d7c23.jpg", "https://mega.nz/folder/1bckyISJ#9YvVcBdXpi_BidrPeQmVZQ"],
            ["Noragami", "ㅤㅤ", "https://is.gd/1rIv1a", "https://mega.nz/folder/1PVQ2KbT#Bl6MEWYFkxUOVgUEzSDWRw"],
            ["Dungeon Mesh", "ㅤㅤ", "https://is.gd/m93I1e", "https://mega.nz/folder/BGEx3KBS#B-AXN8ZoCgVqUUOEnnLlOQ"],
            ["Komi-san wa, Komyushou desu", "ㅤㅤ", "https://is.gd/c7KnyU", "https://mega.nz/folder/5e8kwZJT#s_jToWTYFZQjof7hdjP9rw"],
            ["RADIANT ", "ㅤㅤ", "https://is.gd/K3NTgn", "https://mega.nz/folder/pKVxTKAI#biCI7fzxDibGHJ6pOwspaw"],
            ["Tower of God (Kami no Tou) ", "ㅤㅤ", "https://is.gd/4OUJ1S", "https://mega.nz/folder/sfMgHKjR#Wj4ceIa09QpGT5KPbW4R5g"],
            ["Seirei Gensouki  ", "ㅤㅤ", "https://is.gd/2WXCxQ", "https://mega.nz/folder/MWEmhJha#TdEK6jplWNGWMWf7sksglA"],
            ["BASTARD‼ Heavy Metal, Dark Fantasyㅤ  ", "ㅤㅤ", "https://is.gd/G9yrGX", "https://mega.nz/folder/kTEjDa6D#5n-7JtNVVg3zL5Lx-VatFw"],
            ["Level 1 dakedo Unique  Skill de Saikyou desuㅤ ", "ㅤㅤ", "https://i.pinimg.com/736x/e9/3d/37/e93d37dcaa4df00bd332b5140d3066d8.jpg", "https://mega.nz/folder/YecACJYT#ugw2RfB4NodTOYTsLST7ag"],
            ["  Solo Levelingㅤ ", "ㅤㅤ", "https://is.gd/cnPgEO", "https://mega.nz/folder/ceEG3bxC#Gujt_YOPnVD-m20xf5JUfw"],
            ["  ReZero kara Hajimeru Isekai ", "ㅤㅤ", "https://is.gd/hFV9d6", "https://mega.nz/folder/tWcX2JSJ#XmZwW-pHajhsOk9ihlAhUQ"],
            ["  Ansatsu Kizoku BD Latin.", "ㅤㅤ"," https://is.gd/4sJ4F9", "https://mega.nz/folder/oON1mByb#zQZXQx7zC77GiHAQa0dllg"],
            ["  Wind Breaker ", "ㅤㅤ"," https://is.gd/CJpUMw", "https://mega.nz/folder/dD0DRBwb#2hMpcgUSxzHLns8G7YaTiQ"],
            ["  The Misfit of Demon King Academy ", "ㅤㅤ"," https://is.gd/quEhZJ ", "https://mega.nz/folder/Ab9FXTxa#hfSvFtQZ7A3wWwMU8mxm0A"],
            [" Kami-tachi ni  Hirowareta Otoko ", "ㅤㅤ"," https://is.gd/6Tsj1B", "https://mega.nz/folder/UD9j2Spb#1dw4wcY1IAa0ra3gqsD6lg"],
            ["  Mairimashita! Iruma-kun ", "ㅤㅤ","https://is.gd/CRqopD", "https://mega.nz/folder/VGtFRRrL#YE1cMSsCgly9emZZXehC9g"],
            ["  Yamishibai  ", "ㅤㅤ","https://is.gd/kpb171", "https://mega.nz/folder/BGlGiJyC#S7_OGw9tY-T8aAT0Maa9rw"],
            ["  Atack titan  ", "ㅤㅤ","https://is.gd/jUZoqT", "https://mega.nz/folder/8PVh3YwA#pz0Hjp09BLdONTtdS7pB6Q"],
            ["  Kemono Jihen  ", "ㅤㅤ","https://is.gd/gBz0dB", "https://mega.nz/folder/saF32TBD#KXJfNoOVEghk5qgiGUWYIQ"],
            ["  Log Horizon  ", "ㅤㅤ","https://i.pinimg.com/736x/09/a1/93/09a193455d8865e3e138f32a611fdfd7.jpg", "https://mega.nz/folder/ZLFSHAaI#0edVE9pEzRV1aoq3bJnMlQ"],
            ["  Jigen no Ririsa   ", "ㅤㅤ","https://is.gd/VXy9Fs", "https://mega.nz/folder/5as1ULBb#CeY-nMFGHtJxSnqiX4kv6Q"],
            ["  Sekai Saikou no Ansatsusha, Isekai Kizoku ni Tensei suru   ", "ㅤㅤ","https://is.gd/sEka0a", "https://mega.nz/folder/xS0k3QxQ#BBYXW4UBihfTkNauyBwyHg"],
            ["  Isekai wa Smartphone to Tomo ni  ", "ㅤㅤ","https://is.gd/wNmMBK", "https://mega.nz/folder/ILsxRQDT#d5eGIAihFXg-1F_5JBMOVA"],
            ["  Isekai de Cheat Skill wo Te ni Shita Ore wa ", "ㅤㅤ","https://i.pinimg.com/736x/ce/f7/09/cef7090e8ead61efbaeb633f8e4cca5f.jpg", "https://mega.nz/folder/VbFTnZSC#D0UkRfZePoDnF1OY2-wIfQ"],
            ["  Otome Game Sekai wa Mob ni Kibishii Sekai desu", "ㅤㅤ","https://is.gd/A5cnCV", "https://mega.nz/folder/EXEiiaZD#YBugatu5tqMaxD94BFbP8g"],
            ["  Sousou no Frieren", "ㅤㅤ","https://is.gd/2xq1wP", "https://mega.nz/folder/Ee0hgCpS#ToDDqemPLrbmU9qEAzX5Iw"],
            ["  SPY×FAMILY ", "ㅤㅤ","https://is.gd/NbW3Ro", "https://mega.nz/folder/kT8lSbiD#lWO594-9SPpK37-SCf6uLQ"],
            ["  Fumetsu no Anata e ", "ㅤㅤ","https://is.gd/9mxY4I", "https://mega.nz/folder/ELM2VYTZ#CVQMEanw5N4NDR8x5TLzGw"],
            ["  Plunderer", "ㅤㅤ","https://i.postimg.cc/V6f8LWy9/1KGr66.jpg", "https://mega.nz/folder/MS83lSJI#5HizYZRMkpAx3Mmz5aLO6w"],
            ["  Ore dake Haireru Kakushi Dungeon Kossori Kitaete Sekai Saikyou", "ㅤㅤ","https://is.gd/ZyP8IL", "https://mega.nz/folder/UO8AjTKb#p_vv0LqNSIxvpq0uHc5zRw"],
            ["  Sword Gai The Animation", "ㅤㅤ","https://is.gd/vgQXcL", "https://mega.nz/folder/VOcRnZZS#-3rCFbwbHgng33dTiAucdw"],
            ["   Chiyu Mahou no Machigatta", "ㅤㅤ","https://is.gd/kB6vLj", "https://mega.nz/folder/NaUAAarZ#BVc1G4c_mPONMN-pZ-j0dQ"],
            ["  darling in the franxx", "ㅤㅤ","https://is.gd/BHxcq8", "https://mega.nz/folder/oOFhjagR#db0AY6up3AcSZxeOXm_png"],
            ["  Hakushaku to Yōsei", "ㅤㅤ","https://i.pinimg.com/736x/48/2c/60/482c6076eb0aa59cf3f4699909c40e3b.jpg", "https://mega.nz/folder/Zbkk0Q4Z#tUZWt2C0XybdXrc-XZL_pA"],
            ["  Kono Subarashii Sekai", "ㅤㅤ","https://is.gd/i0KhHE", "https://mega.nz/folder/xWsGDIBT#KtcklXCkiR52WLKwoJkuTw"],
            ["  Tsue to Tsurugi no Wistoria", "ㅤㅤ","https://is.gd/xkmcl7", "https://mega.nz/folder/8Oc0BCpA#TZ-epkfT8JUky3IhJjlpoQ"],
            ["  Tsuki ga Michibiku Isekai Douchuu", "ㅤㅤ","https://is.gd/atVZmg", "https://mega.nz/folder/8Oc0BCpA#TZ-epkfT8JUky3IhJjlpoQ"],
            [" Isekai Ookami to Koushinryou", "ㅤㅤ","https://eapi.pcloud.com/getpubthumb?code=7glotalK&linkpassword=&size=1024x1024&crop=0&type=auto", "https://mega.nz/folder/1KFSWZZY#J7YILutmd2vBDDnjOuFn5g"],
            [" Death March kara Hajimaru Isekai Kyousoukyoku", "ㅤㅤ","https://is.gd/6LINo9", "https://mega.nz/folder/1PF2UKZL#Y3CQN6SNcEsCnu7vg_KmlQ"],
            [" Goblin Slayer BD Latino", "ㅤㅤ","https://is.gd/SjABxq", "https://mega.nz/folder/dTVlGTLS#mLhXZp4kl7gjsYxnJpdjmg"],
            [" Nube Kekkon suru tte, Hontou desu", "ㅤㅤ","https://is.gd/XmEduO", "https://mega.nz/folder/VCUUnDSI#iG1vhNE-ldrAxrEAX9QPzQ"],
            [" Saitama  ", "ㅤㅤ","https://is.gd/58dhXG", "https://mega.nz/folder/oLEC1QwD#SegbBEVbTiIxPYhlDEmD-g"],
            [" Aharen-san wa Hakarenai  ", "ㅤㅤ","https://is.gd/DFLqtN", "https://mega.nz/folder/sCNGkCgY#b04fu3ohRb7xYsnsvU9UyQ"],
            [" Demon Lord 2099  ", "ㅤㅤ","https://i.pinimg.com/736x/91/0a/42/910a423cd0d75ec594efb59f67e3e13e.jpg", "https://mega.nz/folder/5KcF3L5D#XigX-1eFxoeagxx4gxK-HQ"],
            [" Sentouin, Hakenshimasu  ", "ㅤㅤ","https://is.gd/u2bQjw", "https://mega.nz/folder/lH0lyBCD#aqHEHj-uWfdwXgl35CRJ9Q"],
            [" Tate no Yuusha no Nariagari ", "ㅤㅤ","https://is.gd/Go8z8a", "https://mega.nz/folder/ZOF0DRjZ#rzoKeDkpYBY0_2BUp3c_wg"],
            [" Bye Bye, Earth ", "ㅤㅤ","https://is.gd/78h29M", "https://mega.nz/folder/4W9nnaoT#bQxxfz77dU4rPQjhGPLMyQ"],
            [" Arifureta Shokugyou de Sekai Saikyouh ", "ㅤㅤ","https://is.gd/VObirK", "https://mega.nz/folder/hf90DAJK#kNXKjnybpJzeWQtKNCHZ-w"],
            ["Shangri-La Frontier: Kusoge Hunter, Kamige ni Idoman to su ", "ㅤㅤ","https://is.gd/HfWoCm", "https://mega.nz/folder/BGsw1bwT#6uHAwx0CZi_c5OApMhgUWA"],
            ["  Sengoku Night Blood ", "ㅤㅤ","https://is.gd/vbt1ZG", "https://mega.nz/folder/0SEHzYoB#dz-4I4LXl9MNewgvILx4VQ"],
            [" Mushoku Tensei Isekai Ittara Honki Dasu  ", "ㅤㅤ","https://is.gd/PLupUB", "https://mega.nz/folder/pWVXAARY#MXcBoezxuhR08oyv-5behQ"],
            [" Genjitsu Shugi Yuusha no Oukoku Saikenki  ", "ㅤㅤ","https://is.gd/S720Hy", "https://mega.nz/folder/VS9Emb4J#C6ZWPU-nu_XcN9gjePwZgg"],
            [" Blue Lock  ", "ㅤㅤ","https://is.gd/dqWKj1", "https://mega.nz/folder/cWdHjKrR#l5QKeokUSosqufOecf9uuw"],
            [" Amagami-san Chi no Enmusubi  ", "ㅤㅤ","https://is.gd/wNmMBK", "https://mega.nz/folder/FfkWXbKD#bcOBIqhKEv5dXpCUccs8kw"],
            [" Monster DVD Castellano  ", "ㅤㅤ","https://is.gd/6xWhUh", "https://mega.nz/folder/VS8DGJbA#g8jMqe3lHsF5fOBKJoOTbQ"],
            [" Yozakura-san Chi no Daisakusen  ", "ㅤㅤ","https://is.gd/CK57ct", "https://mega.nz/folder/4G1A1bLQ#uITLC9mmOIMVZ-HYfuulAA"],
            [" Magic Maker: Isekai Mahou no Tsukurikata  ", "ㅤㅤ","https://is.gd/G9zJOX", "https://mega.nz/folder/MHMGnaBb#FTwKScJWVvgEbtz1MLsNqg"],
            [" Rurouni Kenshin -Meiji Kenkaku Romantan-  ", "ㅤㅤ","https://is.gd/jch65J", "https://mega.nz/folder/sK0CgKaa#J8XBU6VqF3TlH0GNhPmDBQ"],
            [" Sakamoto Days  ", "ㅤㅤ","https://is.gd/2um2Ln", "https://mega.nz/folder/Ie0TzKDa#4USvriupvxQw9qRG8Tmd3A"],
            [" Castlevania Nocturne ", "ㅤㅤ","https://is.gd/qYyouw", "https://mega.nz/folder/ULdSURAQ#sIomgXHPIiyszZFBARhBqQ"],
            [" Medalist ", "ㅤㅤ","https://is.gd/TJZD69", "https://mega.nz/folder/5bM0nCgS#Ua3ApMSpG-W262jqZUyk4g"],
            [" Tokidoki Bosotto Russia-go de Dereru Tonari no Alya-san ", "ㅤㅤ","https://is.gd/jI73Jd", "https://mega.nz/folder/4KtU3RAQ#SQ9nkcbNPaHK1dAlhlN5PQ"],
            ["One Piece (Latino)", "ㅤㅤ","https://is.gd/uRE8Uj", "https://mega.nz/folder/4KtU3RAQ"],
            ["100-man BD Latino", "ㅤㅤ","https://is.gd/oMi2cd", "https://mega.nz/folder/4XdChLwS#1rY-p2vkWAaETMP7yyCvcQ"],
            ["Nanatsu no Taizai", "ㅤㅤ","https://is.gd/faNYgM", "https://mega.nz/folder/oacnFSyB#A5M0PgaXJseLlWvR65Gb0A"],
            ["Shikkakumon no Saikyokenja", "ㅤㅤ","https://is.gd/lIGCjn", "https://mega.nz/folder/VTFRwIRJ#ABTrRvfjtypeWCJMKFkcpA"],
            ["Isekai Yururi Kikou Kosodateshinagara Boukensha Shimasu", "ㅤㅤ","https://is.gd/EjLhds", "https://mega.nz/folder/lPlQRD7I#ARFonF9b2jJRDuxVI6yuhQ"],
            ["Pandora Hearts", "ㅤㅤ","https://i.pinimg.com/736x/40/be/e8/40bee8b60ebaf148c8c2d91c5c13b362.jpg", "https://mega.nz/folder/1e1WETSA#yV3kLMMVrb-hAFpSzGYGmQ"],
            [" Todas las temporadas De Baki", "ㅤㅤ","https://is.gd/CRxI4w", "https://mega.nz/folder/0K0AGIJK#gCghlE4nTBqGXTy2GTnEeg"],
            ["Kaiju No", "ㅤㅤ","https://is.gd/8A3WRT", "https://mega.nz/folder/YflW1QyT#tKZ2bMUc_Rl5Rni-ZdkUTA"],
            ["Mashle Magic and Muscles", "ㅤㅤ","https://is.gd/REYB6R", "https://mega.nz/folder/NHNEhbRC#Ro_P91X-SCm25UrbZ3a3hw"],
            [" Zenshuu", "ㅤㅤ","https://is.gd/tFbnaz", "https://mega.nz/folder/5blh2CBK#HF2JtvJXqOe68h9JD8Yo_Q"],
            [" Kimi to Boku no Saigo no Senjou, Aruiwa Sekai ga Hajimaru Seisen", "ㅤㅤ","https://is.gd/jzmPJm", "https://mega.nz/folder/Jbt1ibqD#gv6d-sbR2S95ot71HRTmgw"],
            [" Akuyaku Reijou nanode Last Boss wo Kattemimashita", "ㅤㅤ","https://is.gd/gFrd9k", "https://mega.nz/folder/dDEyCDpB#iAKT3lj1ZLXWu7BnNCDePQ"], 
            ["Dorohedoro", "ㅤㅤ","https://is.gd/6DRHlY", "https://mega.nz/folder/obsFnajC#GlI-JiOnnd6cHgmGy0vFrg"],
           ["Hoshizora e Kakaru Hashi", "ㅤㅤ","https://is.gd/Ak7goD", "https://mega.nz/folder/hO0WgARD#aMchCvfF4eU2nIsv5Mj05g"],
           [" Ranma (1989) ", "ㅤㅤ","https://is.gd/oPAsCT", "https://mega.nz/folder/1b9WiB6R#52sghOcowY5HV86dBEh_Yg"],
          ["    Ranma 12 (2024)     ", "ㅤㅤ","https://is.gd/IrfBiq", "https://mega.nz/folder/ofMAjQaI#wJ8Owr2T1rjaA2PzIjEBUg"],
         ["    Myself; Yourself    ", "ㅤㅤ","https://is.gd/x7MjZ9", "https://mega.nz/folder/wDlj2D5C#2tzTMbzUKSn5pvyjS_7hAw"],
        ["   Jibaku Shonen Hanako-kun ", "ㅤㅤ","https://is.gd/FR2nTr", "https://mega.nz/folder/tCc2xLZD#CqgzncvftR2EN6FHucbOEw"],
        ["    Hentai Ouji to Warawanai Neko ", "ㅤㅤ","https://is.gd/eQp2F1", "https://mega.nz/folder/0fNA1KhS#TW5q9wk5KtajtNLdgdvH_A"],
       ["    Ningen Fushin no Boukenshatachi ga Sekai wo Sukuu Youdesu  ", "ㅤㅤ","https://is.gd/ZzSuOR", "https://mega.nz/folder/IesUyR7C#ZpALFTR9m27-9MIy_FCzfg"],
      ["    Subete ga F ni Naru ", "ㅤㅤ","https://is.gd/HMpNi9", "https://mega.nz/folder/8HFFFQiC#9-qpOu_hZY9R_pY7-QsEbA"],
     ["    VTuber nanda ga Haishin Kiri Wasuretara Densetsu ni Natteta ", "ㅤㅤ","https://is.gd/NKyyYL", "https://mega.nz/folder/QO0WjIqQ#TBzBmNghlCPuAI_qbA4CBQ"],
     ["    Watashi no Shiawase na Kekkon  ", "ㅤㅤ","https://is.gd/UYBzQo", "https://mega.nz/folder/Ffc1VKCZ#XxjxbCNk_ZqisVA-yW8uGw"],
     ["   Übel Blatt ", "ㅤㅤ","https://is.gd/j3E6Xv", "https://mega.nz/folder/Ffc1VKCZ#XxjxbCNk_ZqisVA-yW8uGw"],
     ["  Bleach ", "ㅤㅤ","https://i.pinimg.com/736x/b5/d4/ad/b5d4ad33e564e3fbc87fa7449c572b43.jpg", ""],
     [" Zero no Tsukaima ", "ㅤㅤ","https://is.gd/ozEFNK", ""],
      [" Peach Boy Riverside ", "ㅤㅤ","https://is.gd/mD2yIM", ""],
      [" Isshun de Chiryou Shiteita no ni Yakutatazu to Tsuihou Sareta Tensai Chiyushi, Yami Healer Toshite Tanoshiku Ikiru ", "ㅤㅤ","https://is.gd/Kb3l0e", ""],
      [" Katainaka no Ossan, Kensei ni Naru ", "ㅤㅤ","https://is.gd/9ESWKX", ""],
      [" Kuroshitsuji ", "ㅤㅤ","https://is.gd/oXoir4", ""],
      [" Eiyuu Kyoushitsu ", "ㅤㅤ","https://is.gd/k18j7O", ""],
      [" Enen no Shouboutai", "ㅤㅤ","https://is.gd/vtMsWm", "https://mega.nz/folder/1LdBmQwJ#Tq7uLoe8u0CRl-VJY2w4Jw"],
      [" my hero academia  ", "ㅤㅤ","https://is.gd/zosOBG", ""],
      [" Ousama Ranking  ", "ㅤㅤ","https://i.pinimg.com/736x/b6/a1/75/b6a1751beb10880b0c4cb8e4254abd13.jpg", ""],
      [" TO BE HERO X  ", "ㅤㅤ","https://i.pinimg.com/736x/d9/83/78/d9837884079ac9493e859df4223dfce5.jpg", ""],
      [" Kanchigai no Atelier Meister Eiyuu Party no Moto Zatsuyougakari ga, Jitsu wa Sentou Igai ga SSS Rank Datta to Iu Yoku Aru Hanashi  ", "ㅤㅤ","https://i.pinimg.com/736x/05/16/8b/05168bcc5efc924af1553d6df0977e07.jpg", ""], 
      [" Hazure Skill “Kinomi Master”: Skill no Mi (Tabetara Shinu) wo Mugen ni Taberareru You ni Natta Ken ni Tsuite   ", "ㅤㅤ","https://i.pinimg.com/736x/5a/7c/5a/5a7c5ae3108deecbdfd99678fc4c4ca9.jpg", ""],  
      [" Izure Saikyou no Renkinjutsushi   ", "ㅤㅤ","https://i.pinimg.com/736x/34/8b/90/348b90c46a8ba6b24d00fee73c318f42.jpg", ""],  
      [" Rising Impact Temporada 1 y 2   ", "ㅤㅤ","https://i.pinimg.com/736x/6e/97/8e/6e978e866428cd136c1c9735ffc7c7f9.jpg", "https://mega.nz/folder/wbtyWQhZ#Hdq8N38YgZoaZI6mFVQ5ug"],  
      [" Kimi wa Meido-sama.  ", "ㅤㅤ","https://i.pinimg.com/736x/1f/54/8d/1f548d2dd088e694e99f392b4857d001.jpg", ""],  
      [" Isekai Shikkaku  ", "ㅤㅤ","https://i.pinimg.com/736x/29/da/f1/29daf101c04f7df663d0c43ee0a05f58.jpg", "https://mega.nz/folder/0XEmVIiS#LsbIjsZu4VipNshcvpoO7Q"],  
      [" Lv2 kara Cheat datta Motoyuusha Kouho no Mattari Isekai Life ", "ㅤㅤ","https://i.pinimg.com/736x/98/44/d4/9844d4870cf2e8a70be6753b13a3d165.jpg", "https://mega.nz/folder/tPcmzYIB#9mEBwcKXzju4ucvQUkbmcA"],  
      [" Tensei Kizoku no Isekai Boukenroku ", "ㅤㅤ","https://i.pinimg.com/736x/48/a7/7e/48a77ede4b73cbcfd25f165c15778ac4.jpg", "https://mega.nz/folder/1OUmRbjI#JTB_0_EfTFc_qf8GBSTVMA"],
      [" NieRAutomata  ", "ㅤㅤ","https://i.pinimg.com/736x/3e/25/cf/3e25cfe45682a2cb617ddc50515fd8f4.jpg", "https://mega.nz/folder/IedzyQJC#twr4KGDZDjdfCMKgszOdSA"],
      [" Code Geass Dakkan no Rozé  ", "ㅤㅤ","https://pm1.narvii.com/5670/cb9098c8dbdbc55bdf805700cf53b2322a465ba2_hq.jpg", "https://mega.nz/folder/sedACbIZ#rqcB07s1sKkySSP7mqX4RA"], 
      [" chiban Ushiro no Daimaou ", "ㅤㅤ","https://i.pinimg.com/736x/7c/e7/69/7ce769ffd531eed0c661ad2f6666f8a5.jpg", "https://mega.nz/folder/0bd3lL6Y#yREx36wlS1n8edU6l8LkNQ"],
      [" Bocchi the Rock!  ", "ㅤㅤ","https://i.pinimg.com/736x/90/fd/f6/90fdf689531500ef2cdc2b05492763e8.jpg", "https://mega.nz/folder/0Sd0WbyL#KxEzf8IbJHg1I6rZSZWFLg"],
      [" Dandadan  ", "ㅤㅤ","https://i.pinimg.com/736x/ea/3a/26/ea3a26e74477ddabcac48078f712bb4b.jpg", "https://mega.nz/folder/oHMSmQbK#rLmM2YIheWUchTRegSwOWg"],
      [" Eat-Man   ", "ㅤㅤ","https://i.pinimg.com/736x/69/0f/ca/690fcae06f6a5616c464cf85a17b80a1.jpg", "https://mega.nz/folder/oD0EjaSa#g4olsusEK44zFSv7UhRd2w"],
      [" Hajimete no Gal   ", "ㅤㅤ","https://i.pinimg.com/736x/41/19/c6/4119c69db115fe67281f9d5d65841e1b.jpg", "https://mega.nz/folder/UGExnAYZ#3JzFPrjWxmX-wdV2e5fw2Q"],
      [" Rakudai Kishi no Cavalry   ", "ㅤㅤ","https://i.pinimg.com/736x/61/4d/31/614d3178444e51d543a289874406d0c0.jpg", "https://mega.nz/folder/EH9HWK6Q#j0M6YKXRADCPecoPmysnHg"], 
      [" Summer Time Render  ", "ㅤㅤ","https://i.pinimg.com/736x/09/de/af/09deaf395dc0a084fedd12698a6adc3b.jpg", "https://mega.nz/folder/de1UEaqJ#euo80ZqFyp4PL6avNAHJmw"], 
      [" Fuguushoku “Kanteishi” ga Jitsu wa Saikyou Datta  ", "ㅤㅤ","https://static.zerochan.net/Fuguushoku.Kanteishi.ga.Jitsu.wa.Saikyou.Datta.1024.4327717.webp", ""],
      
      [" Slime Taoshite 300-nen, Shiranai Uchi ni Level Max ni Nattemashita  ", "ㅤㅤ","https://aztlan.fciencias.unam.mx/pensadero/posts-images/2024/07/slime-300.jpg", ""],
      [" Hyouken no Majutsushi ga Sekai wo Suberu  ", "ㅤㅤ","https://i.pinimg.com/736x/18/82/44/188244bb8402d6695fb6162d91112df4.jpg", ""],    
      ["  Gaikotsu Kishi-sama, Tadaima Isekai e Odekake-chuu     ", "ㅤㅤ","https://i.pinimg.com/736x/07/a7/ed/07a7ed9a57ac51dc3b9ad9014c7b3707.jpg", ""],    
      [" Jidouhanbaiki ni Umarekawatta Ore wa Meikyuu ni Samayou     ", "ㅤㅤ","https://i.pinimg.com/736x/b7/21/6e/b7216e11bf0b9b25f5e76cf4e281cbf9.jpg", ""], 
      ["  Leviathan     ", "ㅤㅤ","https://i.pinimg.com/736x/e0/68/d5/e068d53468c1a6f46f7f63af8ab78b3e.jpg", ""],
      ["  Ao no Exorcist    ", "ㅤㅤ","https://i.pinimg.com/736x/06/9f/91/069f918b014f48c53ed43e15c208a413.jpg", ""],
      ["  Kumichou Musume to Seiwagakari   ", "ㅤㅤ","https://i.pinimg.com/1200x/d6/a7/7a/d6a77a77724905f79f71577e5773edd4.jpg", ""],
      ["  Yuusha Party wo Tsuihou Sareta Beast Tamer, Saikyoushu no Nekomimi Shoujo to Deau  ", "ㅤㅤ","https://i.pinimg.com/1200x/e7/ec/84/e7ec845e8c0d9bcdfb167ce267382dd5.jpg", ""],
      ["  Dungeon Meshi  ", "ㅤㅤ","https://i.pinimg.com/736x/a6/64/83/a664833387ca165394260c71bdf36539.jpg", ""],
      [" Oshi no Ko ", "ㅤㅤ","https://i.pinimg.com/736x/c2/80/66/c280662dbb98eb2ae3258e25f28cc6c0.jpg", ""],
      [" Mono  ", "ㅤㅤ","https://i.pinimg.com/736x/0c/dc/da/0cdcda4162f0c2d8a482b0675d9e6528.jpg", ""],
      [" Gachiakuta  ", "ㅤㅤ","https://i.pinimg.com/736x/6b/98/6c/6b986cc7e7e305669cda15918c668915.jpg", ""],
      [" Salaryman ga Isekai ni Ittara Shitennou ni Natta Hanashi  ", "ㅤㅤ","https://i.pinimg.com/736x/19/e1/b7/19e1b7cb908b0c0ac538a93739448821.jpg", ""],
      [" Sentai Daishikkaku ", "ㅤㅤ","https://i.pinimg.com/736x/aa/31/83/aa3183083f5b2faed80564b50d0dbac3.jpg", ""],
      [" Tondemo Skill de Isekai Hourou Meshi ", "ㅤㅤ","https://i.pinimg.com/736x/53/b9/02/53b9028360b4976f0c10f78e8e4df117.jpg", ""],
      [" Tougen Anki      ", "ㅤㅤ","https://i.pinimg.com/736x/d3/8e/54/d38e5463348e980baa48b4d317131ae2.jpg", ""],
      ["  Guimi Zhi Zhu: Xiaochou Pian (Lord of Mysteries)     ", "ㅤㅤ","https://i.pinimg.com/736x/61/d3/db/61d3db97b961e79717293b002b86f7d9.jpg", ""],
      ["  Tsuyokute New Saga     ", "ㅤㅤ","https://i.pinimg.com/736x/cb/ee/8a/cbee8a4fce810038f6587dbb6550314e.jpg", ""],
      ["  Toaru Ossan no VRMMO Katsudou Ki    ", "ㅤㅤ","https://i.pinimg.com/1200x/7f/67/36/7f673652a24a18fadb87d438a2fe67c8.jpg", ""],
      ["  Clevatess   ", "ㅤㅤ","https://i.pinimg.com/736x/00/cd/4b/00cd4bc70b7949db2fa3a87d90c8a5fa.jpg", ""],
      ["  Dekoboko Majo no Oyako Jijou    ", "ㅤㅤ","https://i.pinimg.com/1200x/47/ba/1e/47ba1e43cc65c5ea7ffb6f78524b3418.jpg", ""],
      ["  Yuusha Party o Tsuihou Sareta Shiro Madoushi   ", "ㅤㅤ","https://i.pinimg.com/736x/69/1d/1c/691d1c5e8a5f9392d7e169886bb72e8c.jpg", ""],
      ["  One Room, Hiatari Futsuu, Tenshi-tsuki  ", "ㅤㅤ","https://i.pinimg.com/736x/6d/b0/ef/6db0efded3e64331c1ed5c5f17a0e8f0.jpg", ""],
      ["  Boushoku no Berserk  ", "ㅤㅤ","https://i.pinimg.com/736x/c7/51/2f/c7512f823da52cb3e00807c3bdfa3e0d.jpg", ""],
      ["  Chao Neng Lifang Chaofan Pian  ", "ㅤㅤ","https://i.pinimg.com/736x/12/e8/6d/12e86d5beed80188656d4f1e217009c1.jpg", ""],
      ["  Please spare my life  ", "ㅤㅤ","https://i.pinimg.com/736x/54/b5/2b/54b52b3d92fb149d7d8af138e58ad95a.jpg", ""],
      ["  Isekai Shoukan wa Nidome desu  ", "ㅤㅤ","https://i.pinimg.com/736x/06/f7/31/06f7311ff7241bcac6f9c041c2ee1e24.jpg", ""],
      ["  Busamen Gachi Fighter  ", "ㅤㅤ","https://i.pinimg.com/736x/5e/72/56/5e72560fb334d009d8bcea61424fb150.jpg", ""],






            
            // Premium content
            ["S-Rank Monster no Behemoth", "Premium Content", "https://i.pinimg.com/736x/4c/89/67/4c89679ae06bad2b6d8cce351c312d10.jpg", "#", true],
            ["Bikini Warriors BD", "Premium Content", "https://i.pinimg.com/736x/83/66/dc/8366dc6af9e4d089292895d9fe89dd20.jpg", "#", true],
            ["Isekai Onsen Paradise", "Premium Content", "https://i.pinimg.com/736x/7d/66/5f/7d665fad3847d4e475a820b352df2d43.jpg", "#", true]
        ];

        // DOM elements
        const heroSection = document.getElementById('hero-section');
        const mainContent = document.getElementById('main-content');
        const profileModal = document.getElementById('profile-modal');
        const searchInput = document.getElementById('search-input');
        const sortSelect = document.getElementById('sort-select');
        const resultsContainer = document.getElementById('results');
        const netflixHeader = document.getElementById('netflix-header');

        // Initialize app
        function initializeApp() {
            // Create default user profile
            userProfile = {
                name: 'Usuario',
                avatar: avatars[0],
                isKids: false,
                favorites: [],
                history: [],
                createdAt: Date.now()
            };

            // Show hero section by default
            showHero();
            
            // Load saved profile if exists
            const savedProfile = localStorage.getItem('animeUserProfile');
            if (savedProfile) {
                userProfile = JSON.parse(savedProfile);
            }
        }

        function showHero() {
            heroSection.style.display = 'flex';
            mainContent.classList.remove('active');
        }

        function showAnimeSection() {
            heroSection.style.display = 'none';
            mainContent.classList.add('active');
            updateResults();
        }

        function startWatching() {
            showAnimeSection();
            // Smooth scroll to results
            setTimeout(() => {
                document.getElementById('results').scrollIntoView({ 
                    behavior: 'smooth',
                    block: 'start'
                });
            }, 300);
        }

        function showMoreInfo() {
            alert('¡Bienvenido a Anime Tube!\n\nDisfruta de miles de episodios de anime en latino y castellano.\n\n• Catálogo completo actualizado\n• Calidad HD\n• Sin publicidad\n• Contenido premium disponible');
        }

        function openProfileModal() {
            profileModal.classList.add('active');
            loadAvatarSelection();
            
            // Pre-fill with current profile
            if (userProfile) {
                document.getElementById('profile-name-input').value = userProfile.name;
                document.getElementById('kids-profile').checked = userProfile.isKids;
                selectedAvatar = userProfile.avatar;
            }
        }

        function closeProfileModal() {
            profileModal.classList.remove('active');
        }

        function loadAvatarSelection() {
            const avatarSelection = document.getElementById('avatar-selection');
            avatarSelection.innerHTML = '';
            
            avatars.forEach((avatar, index) => {
                const img = document.createElement('img');
                img.src = avatar;
                img.className = 'avatar-option';
                img.onclick = () => selectAvatarOption(img, avatar);
                if (selectedAvatar === avatar || (!selectedAvatar && index === 0)) {
                    img.classList.add('selected');
                    selectedAvatar = avatar;
                }
                avatarSelection.appendChild(img);
            });
        }

        function selectAvatarOption(element, avatar) {
            document.querySelectorAll('.avatar-option').forEach(img => {
                img.classList.remove('selected');
            });
            element.classList.add('selected');
            selectedAvatar = avatar;
        }

        function createProfile(event) {
            event.preventDefault();
            
            const name = document.getElementById('profile-name-input').value.trim();
            const isKids = document.getElementById('kids-profile').checked;
            
            if (!name) {
                alert('Por favor ingresa tu nombre');
                return;
            }
            
            userProfile = {
                name: name,
                avatar: selectedAvatar || avatars[0],
                isKids: isKids,
                favorites: userProfile?.favorites || [],
                history: userProfile?.history || [],
                createdAt: Date.now()
            };
            
            localStorage.setItem('animeUserProfile', JSON.stringify(userProfile));
            closeProfileModal();
        }

        function setFilter(filter) {
            currentFilter = filter;
            document.querySelectorAll('.filter-tab').forEach(tab => tab.classList.remove('active'));
            
            const tabs = document.querySelectorAll('.filter-tab');
            tabs.forEach(tab => {
                if ((filter === 'all' && tab.textContent === 'Todos') ||
                    (filter === 'favorites' && tab.textContent === 'Favoritos') ||
                    (filter === 'recent' && tab.textContent === 'Recientes') ||
                    (filter === 'action' && tab.textContent === 'Acción') ||
                    (filter === 'romance' && tab.textContent === 'Romance') ||
                    (filter === 'comedy' && tab.textContent === 'Comedia')) {
                    tab.classList.add('active');
                }
            });
            
            updateResults();
        }

        function toggleFavorite(animeTitle) {
            if (!userProfile) return;
            
            const index = userProfile.favorites.indexOf(animeTitle);
            if (index > -1) {
                userProfile.favorites.splice(index, 1);
            } else {
                userProfile.favorites.push(animeTitle);
            }
            
            localStorage.setItem('animeUserProfile', JSON.stringify(userProfile));
            updateResults();
        }

        function addToHistory(animeTitle) {
            if (!userProfile) return;
            
            const index = userProfile.history.indexOf(animeTitle);
            if (index > -1) {
                userProfile.history.splice(index, 1);
            }
            
            userProfile.history.unshift(animeTitle);
            
            if (userProfile.history.length > 20) {
                userProfile.history = userProfile.history.slice(0, 20);
            }
            
            localStorage.setItem('animeUserProfile', JSON.stringify(userProfile));
        }

        function normalizeString(str) {
            return str.normalize("NFD").replace(/[\u0300-\u036f]/g, "").toLowerCase();
        }

        function highlightMatch(text, searchTerm) {
            if (!searchTerm) return text;
            const regex = new RegExp(`(${searchTerm})`, 'gi');
            return text.replace(regex, '<mark>$1</mark>');
        }

        function checkPremiumAccess(searchTerm) {
            if (normalizeString(searchTerm) === normalizeString(PREMIUM_KEY)) {
                premiumUnlocked = true;
                searchInput.value = '';
                alert('¡Contenido premium desbloqueado! ✨');
                updateResults();
                return true;
            }
            return false;
        }

        function updateResults() {
            const searchTerm = normalizeString(searchInput.value);
            const sortOrder = sortSelect.value;

            if (checkPremiumAccess(searchTerm)) return;

            let filteredAnime = animeList.filter(anime => {
                const isPremiumMatch = (!anime[4] || premiumUnlocked);
                const isKidsMatch = !userProfile?.isKids || !anime[4]; // Kids can't see premium content
                const isSearchMatch = (normalizeString(anime[0]).includes(searchTerm) ||
                                    normalizeString(anime[1]).includes(searchTerm));
                
                let isCategoryMatch = true;
                if (currentFilter === 'favorites') {
                    isCategoryMatch = userProfile?.favorites.includes(anime[0]);
                } else if (currentFilter === 'recent') {
                    isCategoryMatch = userProfile?.history.includes(anime[0]);
                }
                
                return isPremiumMatch && isKidsMatch && isSearchMatch && isCategoryMatch;
            });

            filteredAnime.sort((a, b) => {
                switch (sortOrder) {
                    case 'desc':
                        return b[0].localeCompare(a[0]);
                    case 'rating':
                        return Math.random() - 0.5;
                    case 'recent':
                        return Math.random() - 0.5;
                    default:
                        return a[0].localeCompare(b[0]);
                }
            });

            resultsContainer.innerHTML = filteredAnime.map((anime, index) => {
                const isFavorite = userProfile?.favorites.includes(anime[0]);
                
                return `
                    <div class="anime-card ${anime[4] ? 'premium' : ''} ${!premiumUnlocked && anime[4] ? 'premium-locked' : ''}" role="listitem">
                        <div class="anime-number">#${index + 1}</div>
                        <div class="anime-image-container">
                            <img class="anime-image" src="${anime[2]}" alt="${anime[0]}" onerror="this.src='https://via.placeholder.com/300x450/333/fff?text=Anime'">
                        </div>
                        <div class="anime-info">
                            <div class="anime-title">${highlightMatch(anime[0], searchInput.value)}</div>
                            <div class="anime-description">${highlightMatch(anime[1], searchInput.value)}</div>
                            <div class="anime-actions">
                                <a href="${!premiumUnlocked && anime[4] ? '#' : anime[3]}"
                                   target="_blank"
                                   rel="noopener noreferrer"
                                   class="watch-button"
                                   onclick="${!premiumUnlocked && anime[4] ? 'return false;' : `addToHistory('${anime[0].replace(/'/g, "\\'")}')`}">
                                    ${!premiumUnlocked && anime[4] ? '🔒 Premium' : '▶️ Ver'}
                                </a>
                                <button class="favorite-button ${isFavorite ? 'active' : ''}" onclick="toggleFavorite('${anime[0].replace(/'/g, "\\'")}')">
                                    ${isFavorite ? '❤️' : '🤍'}
                                </button>
                            </div>
                        </div>
                    </div>
                `;
            }).join('');

            if (filteredAnime.length === 0) {
                let message = 'No se encontraron resultados';
                if (currentFilter === 'favorites') {
                    message = 'No tienes favoritos aún. ¡Agrega algunos!';
                } else if (currentFilter === 'recent') {
                    message = 'No has visto nada recientemente';
                }
                resultsContainer.innerHTML = `<div style="text-align: center; padding: 40px; font-size: 1.2rem; opacity: 0.7;">${message}</div>`;
            }
        }

        // Header scroll effect
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                netflixHeader.classList.add('scrolled');
            } else {
                netflixHeader.classList.remove('scrolled');
            }
        });

        // Event listeners
        searchInput.addEventListener('input', updateResults);
        sortSelect.addEventListener('change', updateResults);

        // Close modal when clicking outside
        profileModal.addEventListener('click', function(event) {
            if (event.target === profileModal) {
                closeProfileModal();
            }
        });

        // Secret premium unlock
        document.addEventListener('keydown', function(event) {
            if (event.key.toLowerCase() === 'x') {
                xKeyPressCount++;
                if (xKeyPressCount === 10) {
                    premiumUnlocked = true;
                    alert('¡Contenido premium desbloqueado secretamente! 🎉');
                    updateResults();
                    xKeyPressCount = 0;
                }
            }
        });

        // Initialize app
        initializeApp();
    </script>
</body>
</html>

<!-- Audio sincronizado con el video -->
<script>
(function() {
    'use strict';

    const heroVideo = document.getElementById('hero-video');
    let userInteracted = false;

    // Función para activar el audio del video
    function enableVideoAudio() {
        if (!heroVideo || userInteracted) return;

        heroVideo.muted = false;
        heroVideo.volume = 0.3;

        heroVideo.play().then(() => {
            userInteracted = true;
        }).catch((error) => {
            console.log('Esperando interacción del usuario para reproducir audio');
        });
    }

    // Función para manejar la interacción del usuario
    function handleUserInteraction() {
        if (!userInteracted && heroVideo) {
            enableVideoAudio();
        }
    }

    // Inicializar cuando el DOM esté listo
    function init() {
        if (!heroVideo) return;

        // Intentar reproducir automáticamente
        setTimeout(enableVideoAudio, 100);

        // Escuchar eventos de interacción del usuario
        const events = [
            'click', 'touchstart', 'touchend', 'keydown',
            'mousemove', 'mousedown', 'scroll'
        ];

        events.forEach(eventName => {
            document.addEventListener(eventName, handleUserInteraction, {
                once: true,
                passive: true,
                capture: true
            });
        });

        // Botón de control de audio visible
        const heroContent = document.querySelector('.hero-content');
        if (heroContent) {
            const audioControl = document.createElement('button');
            audioControl.innerHTML = '🔊';
            audioControl.style.cssText = `
                position: absolute;
                bottom: 2rem;
                right: 2rem;
                background: rgba(0, 0, 0, 0.7);
                border: 2px solid rgba(255, 255, 255, 0.3);
                color: white;
                width: 50px;
                height: 50px;
                border-radius: 50%;
                cursor: pointer;
                font-size: 1.5rem;
                display: flex;
                align-items: center;
                justify-content: center;
                transition: all 0.3s ease;
                backdrop-filter: blur(10px);
                z-index: 10;
            `;

            audioControl.addEventListener('mouseenter', function() {
                this.style.transform = 'scale(1.1)';
                this.style.background = 'rgba(229, 9, 20, 0.8)';
            });

            audioControl.addEventListener('mouseleave', function() {
                this.style.transform = 'scale(1)';
                this.style.background = 'rgba(0, 0, 0, 0.7)';
            });

            audioControl.addEventListener('click', function(e) {
                e.stopPropagation();
                if (heroVideo.muted || heroVideo.volume === 0) {
                    heroVideo.muted = false;
                    heroVideo.volume = 0.3;
                    this.innerHTML = '🔊';
                    heroVideo.play();
                    userInteracted = true;
                } else {
                    heroVideo.volume = 0;
                    this.innerHTML = '🔇';
                }
            });

            document.querySelector('.hero-section').appendChild(audioControl);
        }

        // Mantener el video reproduciéndose
        heroVideo.addEventListener('pause', () => {
            if (userInteracted) {
                heroVideo.play();
            }
        });

        // Reactivar cuando la página obtiene foco
        window.addEventListener('focus', () => {
            if (userInteracted && heroVideo.paused) {
                heroVideo.play();
            }
        });
    }

    // Ejecutar cuando el DOM esté listo
    if (document.readyState === 'loading') {
        document.addEventListener('DOMContentLoaded', init);
    } else {
        init();
    }

})();
</script>
