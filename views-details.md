# JoinToDive - Lista widoków aplikacji

## Widoki główne
- `dashboard-view` - strona główna
- `profile-view` - profil użytkownika

## Widoki list
- `courses-list-view` - lista wszystkich kursów
- `events-list-view` - lista wszystkich wydarzeń
- `partners-list-view` - lista wszystkich partnerów nurkowych

## Widoki szczegółowe dla uczestnika
- `course-detail-view` - szczegóły kursu z wyśrodkowanym formularzem zapisu
- `event-detail-view` - szczegóły wydarzenia z wyśrodkowanym formularzem zapisu
- `partner-detail-view` - szczegóły partnera nurkowego z możliwością propozycji wspólnego nurkowania

## Widoki tworzenia (Organizator)
- `create-course-view` - tworzenie nowego kursu (formularz wyśrodkowany)
- `create-event-view` - tworzenie nowego wydarzenia (formularz wyśrodkowany)
- `create-dive-view` - tworzenie nowego nurkowania (formularz wyśrodkowany)

## Widoki dla organizatora
- `organizer-list-view` - lista organizowanych wydarzeń (kursy, wydarzenia, nurkowania)
- `organizer-course-detail-view` - szczegóły organizowanego kursu (zarządzanie zgłoszeniami, uczestnikami, historia, edycja)
- `organizer-event-detail-view` - szczegóły organizowanego wydarzenia (zarządzanie zgłoszeniami, uczestnikami, historia, edycja)
- `organizer-dive-detail-view` - szczegóły organizowanego nurkowania (zarządzanie zgłoszeniami, uczestnikami, historia, edycja)

## Widoki dla zapisanych elementów
- `registered-list-view` - lista zapisanych elementów (kursy, wydarzenia, nurkowania) - nowy layout
- `registered-course-detail-view` - szczegóły zapisanego kursu
- `registered-event-detail-view` - szczegóły zapisanego wydarzenia
- `registered-partner-detail-view` - szczegóły zapisanego nurkowania z partnerem

## Funkcje JavaScript
Każdy widok ma swoją funkcję JavaScript do wyświetlania:
- `showDashboard()` - wyświetla dashboard
- `showProfile()` - wyświetla profil
- `showCoursesList()` - wyświetla listę kursów
- `showEventsList()` - wyświetla listę wydarzeń
- `showPartnersList()` - wyświetla listę partnerów
- `showCourseDetail()` - wyświetla szczegóły kursu (uczestnik)
- `showEventDetail()` - wyświetla szczegóły wydarzenia (uczestnik)
- `showPartnerDetail()` - wyświetla szczegóły partnera
- `showCreateCourseView()` - wyświetla formularz tworzenia kursu
- `showCreateEventView()` - wyświetla formularz tworzenia wydarzenia
- `showCreateDiveView()` - wyświetla formularz tworzenia nurkowania
- `showOrganizerList()` - wyświetla listę organizowanych wydarzeń
- `showOrganizerCourseDetail()` - wyświetla szczegóły organizowanego kursu
- `showOrganizerEventDetail()` - wyświetla szczegóły organizowanego wydarzenia
- `showOrganizerDiveDetail()` - wyświetla szczegóły organizowanego nurkowania
- `showRegisteredList()` - wyświetla listę zapisanych elementów (nowy layout)
- `showRegisteredCourseDetail()` - wyświetla szczegóły zapisanego kursu
- `showRegisteredEventDetail()` - wyświetla szczegóły zapisanego wydarzenia
- `showRegisteredPartnerDetail()` - wyświetla szczegóły zapisanego nurkowania z partnerem

## Funkcje pomocnicze
- `hideAllViews()` - ukrywa wszystkie widoki
- `toggleDepthFilter()` - przełącza filtr głębokości

Każda funkcja wyświetlająca ukrywa wszystkie inne widoki podczas wyświetlania wybranego widoku.

## Nawigacja
- **Navbar**: Logo (powrót do dashboard), Kursy, Wydarzenia, Nurkowanie
- **Prawa strona navbar**: Uczestnik, Organizator (dropdown), Profil
- **Menu Organizator**: Utwórz kurs, Utwórz wydarzenie, Utwórz nurkowanie, Zarządzaj

## Struktura widoków organizatora
Wszystkie widoki organizatora (`organizer-course-detail-view`, `organizer-event-detail-view`, `organizer-dive-detail-view`) zawierają:
- Podstawowe informacje o wydarzeniu
- Sekcję "Zgłoszenia" z uczestnikami oczekującymi na decyzję
- Sekcję "Zaakceptowani uczestnicy" z możliwością zarządzania
- Sekcję "Historia zmian" z logiem działań
- Przyciski do edycji i anulowania wydarzenia

## Struktura widoków uczestnika
Wszystkie widoki uczestnika (`course-detail-view`, `event-detail-view`, `registered-course-detail-view`, `registered-event-detail-view`, `registered-partner-detail-view`) zawierają:
- Szczegółowe informacje o kursie/wydarzeniu/nurkowaniu
- Wyśrodkowany formularz zapisu (dla kursu i wydarzenia)
- Status zapisu (dla zapisanych: Potwierdzony/Oczekujący/Odrzucony)
- Możliwość wysłania wiadomości do organizatora (dla zapisanych)
- Możliwość rezygnacji z udziału (dla zapisanych) 