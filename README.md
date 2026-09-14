# Study Helper AI

Study Helper AI to aplikacja webowa we Flasku pomagająca studentom w nauce.

## Funkcje

- rejestracja i logowanie użytkowników
- hashowanie haseł bcrypt
- sesje Flask
- endpointy AI dostępne tylko po zalogowaniu
- zadawanie pytań AI
- streszczanie dowolnego tekstu
- generowanie quizów z notatek
- upload i analiza plików CSV
- generowanie raportu HTML
- walidacja danych wejściowych
- ochrona przed prompt injection
- walidacja odpowiedzi modelu
- rate limiting przez Flask-Limiter
- nagłówki bezpieczeństwa przez Flask-Talisman
- przygotowanie do wdrożenia na Render/Railway

## Technologie

Python, Flask, Jinja2, pandas, Gemini API, bcrypt, Flask-Limiter, Flask-Talisman, HTML, CSS.

## Zmienne środowiskowe

Aplikacja wymaga:

GEMINI_API_KEY - klucz API do Gemini  
SECRET_KEY - sekret Flask do sesji  
GEMINI_MODEL - opcjonalnie, domyślnie gemini-3.6-flash

## Uruchomienie lokalne

pip install -r requirements.txt  
python app.py

## Wdrożenie

Build command:

pip install -r requirements.txt

Start command:

gunicorn app:app

## Prywatność

Aplikacja jest projektem edukacyjnym. Nie należy przesyłać danych wrażliwych.
Hasła są zapisywane wyłącznie jako hash bcrypt.
