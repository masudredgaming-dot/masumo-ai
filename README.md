# MASU MO AI — Starter Build

Ei zip e ekta chalu starter app ache: cute Orb screen, Groq/Gemini key paste ar auto-detect, ar chat.

## Ja ache
- Orb screen (pulse animation)
- Groq (`gsk_...`) ar Gemini (`AIza...`) key auto-detect
- Simple chat with the selected provider
- Launcher icon ar `assets/logo.svg`

## Ja ekhono nei (next steps)
Wake word, Orb overlay, accessibility control, screen capture, planner/agent, ElevenLabs voice, Room history, model dropdown. Ei gulo master prompt (masu_mo_master_prompt) diye poroborti build e add kora jabe.

## APK banabo kivabe

### Option A (sohoj, Termux na): GitHub diye
1. GitHub e ekta new repository banao (Private/Public jeta chao).
2. Ei folder er sob file upload koro (`.github` folder sho).
3. Upload hoye gele **Actions** tab e jao. "Build APK" run hobe automatically.
4. Run complete hole **MASU_MO_AI_APK** artifact theke zip download koro, bhitore `app-debug.apk` pabe.
5. Phone e APK install koro (Settings e "Unknown apps install" allow koro).

### Option B: Android Studio (laptop)
Folder ta Android Studio te open koro, Build > Build APK(s) chapo.

### Option C: Termux (phone)
Termux e full Android SDK + Gradle setup kora kothin ar onek somoy lage, tai Option A ba AIDE app (phone e) recommend kori. Termux e try korte chaile: `pkg install openjdk-17 gradle` diye java/gradle install koro, tarpor Android SDK command-line tools lagbe. Problem hole Option A te jao.

## Important
- API key phone e save hoy shadhoron prefs e. Production er age EncryptedSharedPreferences e shoriye nao.
- Gemini key URL e jay, tai log/screenshot e share korar age sabdhan.
- Eta debug build, Play Store er jonno na.
