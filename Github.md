# Komendy w GitBash: #
 - clear (czyści okno poleceń).
 - cd (przechodzenie do pliku/folderu)
 - cd .. (powrót do poprzedniego folderu)
 - cd ~ (powrót do katalogu głównego)
 - pwd (sprawdzenie ścieżki folderu)
 - ls/dir (wyświetlanie elementów w folderze)
 - mkdir (stowrzenie folderu)
 - touch (storzenie pliku)
 - notepad ( otworzenie pliku)
 - code (otworzenie pliku w VSC)
 - >> (tworzenie pliku)
 - echo (tworzenie pliku)
 - rm+nazwa pliku (usunięcie danego pliku)
 - rm *.html (usunięcie wszystlkich plików  .html)

# Tworzenie repozytorium// Konfiguracja Gita: #
(4 stany plików w repozytorium (dla czytelności)
- nieśledzony (untracked) - gdy dodamy nowy plik (lub usuniemy ze
śledzonych)
- śledzony niezmodyfikowany (tracked unmodified) - pliki które zostały już
dodane do repozytorium (gdy wykonamy commit) i od tego czasu w
katalogu roboczym nie był zmieniany
- śledzony zmodyfikowany (tracked modified) - plik dodany wcześniej do
repozytorium, a aktualnie zmieniony (edytowany) w folderze roboczym
- śledzony w poczekalni (tracked staged) - plik, który został dodany do
indeksu (stage area) i oczekuje na commit (wcześniej mógł to być
nieśledzony czy śledzony zmodyfikowany).)


 - git init (stworzenie repozytorium gita tworzy folder .git)
 - git status ( informuje o tym co wie git)

 -- git config --global user.name (ustawienia globalne do wszystkich repozytoium)
 -- git config --global user.email
 -- git config --globa core.editor (sprawdzenie ustawienia edytora podczas instalacji)
 -- git config --global --unset (usunięcie danych)
 -- git init --help (dokumentacja)
 -- git init --h (parametry ktorych można użyć)
 -- git add + nazwa pliku 
 -- git commit 
 -- git log 
 -- git log --oneline
 -- git commit -m "tekst commitu"
 -- git add --all (dodanie wszystkich plików)

# Klonowanie repozytorium: #
- git clone (folder/link który jest do sklonowania) (nazwa nowego folderu)
.gitignore

