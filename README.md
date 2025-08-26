# 🏫 Svenska Förskolor Karta

En interaktiv 3D-karta för att upptäcka och jämföra förskolor i Sverige med omfattande statistik och funktioner.

![Svenska Förskolor](https://img.shields.io/badge/Förskolor-540+-brightgreen)
![React](https://img.shields.io/badge/React-18+-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5+-blue)
![Mapbox](https://img.shields.io/badge/Mapbox-GL-orange)

## 🌟 Funktioner

### 🗺️ Interaktiv 3D-Karta
- **Mapbox GL** integration med anpassad styling
- **Förskolemarkörer** med kluster-funktionalitet
- **3D-byggnadsextrudering** för realistisk visualisering
- **Värmekartor** för olika statistiska data
- **Interaktiva popups** med detaljerad information

### 📊 Omfattande Statistik
- **Kommunjämförelser** med visuell data
- **Statistiska överlagringar** (personaltäthet, kvalifikationer, etc.)
- **Filtersystem** efter kommun, betyg, etc.
- **Realtidsdata** från Supabase

### 🔍 Smart Sökning & Upptäckt
- **Intelligent sökfält** med autoifyllning
- **Geografisk filtrering** baserat på plats
- **Favoritssystem** för sparade förskolor
- **Jämförelseverktyg** mellan olika förskolor

### 📱 Responsiv Design
- **Mobiloptimerad** interface
- **Pekskärmsvänliga** kartkontroller
- **Adaptiva layouter** för alla skärmstorlekar
- **Mörkt/ljust läge** support

## 🚀 Kom Igång

### Förutsättningar
- Node.js 18+
- npm eller yarn
- Git

### Installation
```bash
# Klona repositoriet
git clone https://github.com/KSAklfszf921/svenska-forskolor-karta.git
cd svenska-forskolor-karta

# Installera beroenden
npm install

# Starta utvecklingsserver
npm run dev
```

### Miljövariabler
Skapa `.env.local` fil:
```env
# Supabase Configuration
VITE_SUPABASE_URL=https://zfeqsdtddvelapbrwlol.supabase.co
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key

# Mapbox (för 3D-kartor)
VITE_MAPBOX_TOKEN=your_mapbox_token

# Google APIs (valfritt - för förbättrad data)
VITE_GOOGLE_MAPS_API_KEY=your_google_api_key
```

## 📊 Data Källor

- **Skolverket** - Officiell svensk förskoledata (540+ förskolor)
- **Google Places API** - Recensioner, betyg, kontaktinfo
- **Supabase** - Realtids databas och backend
- **OpenStreetMap/Mapbox** - Kartdata och geografisk information

## 🛠️ Teknisk Stack

### Frontend
- **React 18** - Modern UI-bibliotek
- **TypeScript** - Typesäkerhet och utvecklarupplevelse
- **Vite** - Snabb byggprocess och utveckling
- **Tailwind CSS** - Utility-first CSS framework
- **shadcn/ui** - Komponentbibliotek

### Backend & Data
- **Supabase** - Backend-as-a-Service
- **PostgreSQL** - Relationsdatabas
- **Edge Functions** - Serverless funktioner

### Kartor & Visualisering
- **Mapbox GL JS** - Interaktiva 3D-kartor
- **Custom Layers** - Specialiserade visualiseringar
- **Clustering** - Optimerad prestanda för stora dataset

## 📁 Projektstruktur

```
svenska-forskolor-karta/
├── src/
│   ├── components/          # React-komponenter
│   │   ├── Map3D.tsx       # Huvud 3D-kartkomponent
│   │   ├── PreschoolDetails.tsx # Detaljerad förskoleinformation
│   │   ├── StatisticsPanel.tsx  # Datavisualisering
│   │   └── ui/             # Återanvändbara UI-komponenter
│   ├── hooks/              # Custom React hooks
│   ├── stores/             # Zustand state management
│   ├── integrations/       # Supabase integration
│   └── utils/              # Hjälpfunktioner
├── supabase/
│   ├── migrations/         # Databasschema
│   ├── functions/          # Edge-funktioner
│   └── config.toml         # Supabase-konfiguration
├── public/                 # Statiska filer
└── .github/workflows/      # GitHub Actions
```

## 🚀 Deployment

### GitHub Pages (Automatisk)
Sidan deployas automatiskt till GitHub Pages när kod pushes till main-branchen:
- **URL**: https://ksaklfszf921.github.io/svenska-forskolor-karta/
- **Workflow**: `.github/workflows/build-deploy.yml`

### Manuell Byggprocess
```bash
# Bygg för produktion
npm run build

# Förhandsgranska byggd version
npm run preview
```

## 📈 Prestandaoptimering

- **Koddelning** - Mapbox, Supabase, vendor chunks separerade
- **Bildoptimering** - Korrekta format och storlekar
- **Lazy loading** - Komponenter och data laddas vid behov
- **Cachingstrategier** - För API-svar och kartdata

## 🛡️ Säkerhet

- **Miljövariabler** - Inga hemligheter i koden
- **RLS-policyer** - Databasåtkomstkontroll
- **API rate limiting** - Google/Mapbox användningsgränser
- **Inputvalidering** - Säkra sök- och filterinmatningar

## 🤝 Bidrag

Bidrag är välkomna! Vänligen:
1. Forka repositoriet
2. Skapa en feature branch (`git checkout -b feature/AmazingFeature`)
3. Committa dina ändringar (`git commit -m 'Add some AmazingFeature'`)
4. Push till branchen (`git push origin feature/AmazingFeature`)
5. Öppna en Pull Request

## 📄 Licens

Detta projekt är licensierat under MIT-licensen - se [LICENSE](LICENSE) filen för detaljer.

## 🙏 Acknowledgments

- **Skolverket** för tillhandahållande av öppen förskoledata
- **Mapbox** för 3D-kartteknologi
- **Supabase** för backend-infrastruktur
- **Google Places API** för berikad data
- **React Community** för fantastiska verktyg och bibliotek

## 📞 Kontakt

**Live Demo**: https://ksaklfszf921.github.io/svenska-forskolor-karta/
**Repository**: https://github.com/KSAklfszf921/svenska-forskolor-karta
**Issues**: https://github.com/KSAklfszf921/svenska-forskolor-karta/issues

---

Utvecklat med ❤️ för svenska föräldrar och förskolor.

*Upptäck, jämför och hitta den perfekta förskolan för ditt barn!*