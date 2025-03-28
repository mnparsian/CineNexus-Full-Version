# CineNexus

CineNexus is a full-stack social media platform tailored for movie and TV show enthusiasts. It allows users to discover, track, review, and discuss movies and series, while also offering a social experience through friend connections, real-time chat, and AI-based personalized recommendations.

---

## 🚀 Technologies Used

### Frontend
- **React 19** with **Vite** for blazing-fast builds
- **Tailwind CSS** for modern and responsive UI
- **Redux Toolkit** for state management
- **ShadCN UI** & **Lucide React** for clean and animated components
- **Framer Motion** for smooth transitions
- **React Router Dom** for routing

### Backend
- **Spring Boot** + **Spring Data JPA**
- **PostgreSQL** hosted on **Render**
- **JWT Authentication** with Role-Based Access
- **WebSocket** for real-time messaging
- **PayPal API** for subscription-based payments
- **TMDB API** for movie & TV show data

---

## 🌟 Key Features

### 🔐 Authentication
- Register, Login (JWT-based)
- Role-based access control: Admin / User
- Public & Private user profiles
- OTP module (for future use)

### 🎬 Movie & TV Management
- Fetch from TMDB: popular, top-rated, trending, upcoming
- Full details page for each media with:
  - Cast & Crew
  - Genres, Ratings, Trailers
  - Add to Watchlist / Favorites
- User reviews and comments with edit/delete options

### 📋 Watchlist System
- Add/remove items to Watchlist & Favorites
- Custom status: "Watching", "To Watch", etc.
- Drag-and-drop reordering
- Carousel-style UI with responsive design

### 📨 Comments & Reviews
- Add, Edit, Delete comments & reviews for any media
- Reviews are displayed in user profiles
- Each comment is styled in modals with animations

### 💬 Real-Time Chat System
- Private & group messaging using **WebSocket (STOMP)**
- Emoji reactions to messages
- File uploads (images, video, PDF)
- Seen/unseen status
- Notifications inside the app

### 🧑‍🤝‍🧑 Friend System
- Users can:
  - Search for other users
  - Send, accept, reject friend requests
  - View friends on their profile
- After friendship:
  - A private chat room is automatically created
  - Mutual movies & reviews are visible
- Backend logic ensures no duplicate or circular requests
- Everything is stored in `FriendRequest` and `Friendship` tables

### 🌐 Admin Panel
- Accessible only to admins
- Add/Edit/Delete users
- Change user roles
- Reset passwords

### 💳 Subscription & Payment System
- Users can subscribe to get access to AI recommendations
- Payment handled via **PayPal** or local gateways
- Subscription details are stored and validated with JWT

### 🤖 AI Movie Recommendation (Premium Feature)
- AI suggests movies based on:
  - User's watchlist, favorites, and genres
  - Similar users' preferences
- Built with a custom recommendation engine
- Future versions will support "mood-based" suggestions (e.g., sad, happy)
- Accessible only after successful payment
- Delivered via `/api/ai/recommendations`

### 📱 Responsive UI / Dark Mode Support
- Fully mobile responsive (phones, tablets, desktops)
- Dark/Light mode toggle with animated icons
- Clean minimalist UI with user-friendly interactions

---

## 📊 User Profile Page
- Avatar, Bio, Country, Language
- Tabs:
  - Watchlist
  - Favorites
  - Reviews
  - Friends
  - Activity
- Stats section:
  - Total watched, reviews written, friends
  - Favorite genres (visualized with badges)

---

## 🔍 Search & Filters
- Full-text search for movies, TV shows, users
- Filters for:
  - Genre
  - Year
  - Rating
  - Type (Movie / TV Show)

---

## 🛠️ Deployment
- **Backend**: Spring Boot hosted on Render
- **Frontend**: React deployed on Vercel
- PostgreSQL hosted on Render with proper CORS configuration
- Environment variables stored securely in `.env`

---

## 📁 Project Structure (Frontend)
```
/src
 ├── features/         # Redux slices and feature logic
 ├── pages/            # Page components (Home, Details, Profile)
 ├── components/       # Shared components (Navbar, Cards, etc.)
 ├── utils/            # Helper functions
 ├── hooks/            # Custom React hooks
 └── store.js         # Redux store setup
```

---

## 🧠 Future Features
- Mood-based movie suggestions with GPT
- Group chats & watch parties
- Profile badges & rankings
- Admin analytics dashboard

---

## 👏 Credits
- TMDB API
- ShadCN UI / Tailwind CSS
- Spring Boot Team
- PayPal Sandbox API
- OpenAI (planned)

---

## 📌 Final Notes
CineNexus is a showcase of modern full-stack web development with a focus on:
- Real-world use of microservices
- Complex state management
- Seamless user experience with real-time communication
- AI integration in media recommendations

> Built with by Mahdi Nazari  
> LinkedIn: [https://www.linkedin.com/in/mahdi-nazari7/](https://www.linkedin.com/in/mahdi-nazari7)

---

---

## 📄 License

This project is licensed under the **MIT License**.  
See the [LICENSE](./LICENSE) file for full details.


# 🇮🇹 CineNexus (Italiano)

CineNexus è una piattaforma social full-stack pensata per gli appassionati di film e serie TV. Permette agli utenti di scoprire, tracciare, recensire e discutere film e serie, offrendo anche un'esperienza sociale con connessioni tra amici, chat in tempo reale e suggerimenti personalizzati basati sull'intelligenza artificiale.

---

## 🚀 Tecnologie Utilizzate

### Frontend
- **React 19** con **Vite** per build veloci
- **Tailwind CSS** per un'interfaccia moderna e reattiva
- **Redux Toolkit** per la gestione dello stato
- **ShadCN UI** & **Lucide React** per componenti puliti e animati
- **Framer Motion** per transizioni fluide
- **React Router Dom** per il routing

### Backend
- **Spring Boot** + **Spring Data JPA**
- **PostgreSQL** ospitato su **Render**
- **Autenticazione JWT** con controllo basato sui ruoli
- **WebSocket** per messaggistica in tempo reale
- **PayPal API** per pagamenti in abbonamento
- **TMDB API** per dati su film e serie TV

---

## 🌟 Funzionalità Principali

### 🔐 Autenticazione
- Registrazione e login con JWT
- Controllo accessi basato sui ruoli: Admin / Utente
- Profili pubblici e privati
- Modulo OTP (per uso futuro)

### 🎬 Gestione Film e Serie TV
- Dati da TMDB: popolari, più votati, in tendenza, prossimamente
- Pagina dettagliata con:
  - Cast & Crew
  - Generi, valutazioni, trailer
  - Aggiunta a Watchlist / Preferiti
- Recensioni e commenti con modifica/eliminazione

### 📋 Watchlist
- Aggiunta/rimozione di elementi da Watchlist e Preferiti
- Stato personalizzato: "In visione", "Da vedere", ecc.
- Ordinamento tramite drag & drop
- Interfaccia in stile carosello reattiva

### 📨 Commenti e Recensioni
- Aggiunta, modifica ed eliminazione
- Visualizzazione nelle pagine profilo
- Stile in modali con animazioni

### 💬 Chat in Tempo Reale
- Chat private e di gruppo con **WebSocket (STOMP)**
- Reazioni emoji
- Invio file (immagini, video, PDF)
- Stato visto/non visto
- Notifiche in-app

### 🧑‍🤝‍🧑 Sistema Amici
- Cerca utenti, invia/ricevi richieste di amicizia
- Visualizza amici nel profilo
- Crea automaticamente chat privata dopo l'amicizia
- Film e recensioni condivisi visibili
- Logica backend evita duplicati

### 🌐 Pannello Admin
- Accesso solo per admin
- Aggiunta, modifica, eliminazione utenti
- Cambio ruoli e reset password

### 💳 Abbonamento e Pagamenti
- Accesso a raccomandazioni AI tramite abbonamento
- Pagamento con **PayPal** o gateway locali
- Dati di abbonamento validati con JWT

### 🤖 Raccomandazioni AI (Premium)
- Suggerimenti basati su:
  - Watchlist, preferiti, generi dell'utente
  - Preferenze utenti simili
- Motore di raccomandazione personalizzato
- Versioni future con suggerimenti basati sull'umore
- Accessibile dopo il pagamento
- Endpoint: `/api/ai/recommendations`

### 📱 UI Responsive / Modalità Chiaro/Scuro
- Totalmente responsive
- Toggle dark/light mode
- UI minimalista, moderna e user-friendly

---

## 📊 Profilo Utente
- Avatar, bio, paese, lingua
- Tab:
  - Watchlist
  - Preferiti
  - Recensioni
  - Amici
  - Attività
- Statistiche:
  - Totale visti, recensioni, amici
  - Generi preferiti con badge

---

## 🔍 Ricerca e Filtri
- Ricerca full-text per film, serie, utenti
- Filtri per:
  - Genere
  - Anno
  - Valutazione
  - Tipo (Film / Serie)

---

## 🛠️ Deployment
- **Backend**: Spring Boot su Render
- **Frontend**: React su Vercel
- PostgreSQL su Render con CORS configurato
- Variabili `.env` gestite in sicurezza

---

## 📁 Struttura del Progetto (Frontend)
```
/src
 ├── features/         # Slice Redux
 ├── pages/            # Pagine (Home, Dettagli, Profilo)
 ├── components/       # Componenti condivisi
 ├── utils/            # Funzioni di utilità
 ├── hooks/            # Hook personalizzati
 └── store.js         # Setup Redux
```

---

## 🧠 Funzionalità Future
- Suggerimenti AI basati sull’umore (GPT)
- Chat di gruppo e watch party
- Badge e classifiche profilo
- Dashboard admin con statistiche

---

## 👏 Crediti
- TMDB API
- ShadCN UI / Tailwind CSS
- Spring Boot Team
- PayPal Sandbox API
- OpenAI (previsto)

---

## 📌 Note Finali
CineNexus è un esempio di sviluppo web full-stack moderno con focus su:
- Microservizi reali
- Gestione avanzata dello stato
- Esperienza utente fluida e in tempo reale
- Integrazione AI nelle raccomandazioni

> Realizzato con da Mahdi Nazari 
LinkedIn: [https://www.linkedin.com/in/mahdi-nazari7/](https://www.linkedin.com/in/mahdi-nazari7)
>
> # 🇮🇷 CineNexus (فارسی)

CineNexus یک پلتفرم شبکه اجتماعی تمام‌عیار برای علاقه‌مندان به فیلم و سریال است. کاربران می‌توانند:

- فیلم‌ها و سریال‌ها را جستجو و کشف کنند.
- آن‌ها را به لیست واچ‌لیست یا علاقه‌مندی اضافه یا حذف کنند.
- نقد و بررسی بنویسند و کامنت بگذارند.
- با دوستان خود ارتباط برقرار کنند، درخواست دوستی بفرستند یا چت کنند.
- از سیستم پیشرفته پیشنهاد فیلم بر اساس سلیقه یا مود استفاده کنند (ویژه مشترکین).

---

## 🎯 ویژگی‌های کلیدی

- **احراز هویت با JWT** و نقش‌ها (ادمین، کاربر)
- **مدیریت فیلم و سریال‌ها** از طریق TMDB API
- **واچ‌لیست قابل شخصی‌سازی** با دراگ و دراپ
- **نقد و نظر** با قابلیت ویرایش و حذف
- **چت لحظه‌ای** با WebSocket، ارسال فایل، ایموجی و وضعیت مشاهده پیام‌ها
- **سیستم دوستان**: ارسال، پذیرش، رد درخواست و نمایش لیست دوستان
- **پیشنهاد فیلم توسط هوش مصنوعی** (براساس علاقه‌مندی‌ها و کاربران مشابه)
- **پنل مدیریت کاربران برای ادمین**
- **پرداخت و اشتراک با PayPal** برای فعال‌سازی سیستم پیشنهاد هوشمند
- **طراحی کاملاً ریسپانسیو و پشتیبانی از دارک/لایت مود**

---

## 📦 تکنولوژی‌ها

- فرانت‌اند: React + Vite + Tailwind CSS + Redux Toolkit + ShadCN UI
- بک‌اند: Spring Boot + PostgreSQL + JWT Auth + WebSocket
- API خارجی: TMDB برای دریافت اطلاعات فیلم، PayPal برای پرداخت‌ها

---

> توسعه داده شده با  توسط مهدی نظری  
>  LinkedIn: [https://www.linkedin.com/in/mahdi-nazari7/](https://www.linkedin.com/in/mahdi-nazari7)

