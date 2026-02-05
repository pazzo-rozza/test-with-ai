# 📌 Task Case – Controlli Funzionali

## 1. Controllo Nazionalità
| ID  | Descrizione                  | Input     | Output Atteso                                   |
|-----|------------------------------|-----------|-------------------------------------------------|
| N1  | Selezione nazionalità valida | Italia    | Il sistema accetta la selezione                 |
| N2  | Nazionalità non prevista     | Atlantide | Errore: nazionalità non riconosciuta            |
| N3  | Nessuna selezione            | —         | Richiesta di selezionare una nazionalità        |
| N4  | Cambio nazionalità           | IT → FR   | Il sistema aggiorna correttamente il valore     |

---

## 2. Controllo Numero Persone
| ID  | Descrizione                        | Input | Output Atteso                                   |
|-----|------------------------------------|--------|-------------------------------------------------|
| P1  | Inserimento numero valido          | 3      | Valore accettato                                |
| P2  | Numero minimo                      | 1      | Accettato                                       |
| P3  | Numero massimo consentito          | 10     | Accettato                                       |
| P4  | Numero superiore al massimo        | 11     | Errore: limite superato                         |
| P5  | Caratteri non numerici             | abc    | Errore: input non valido                        |
| P6  | Campo vuoto                        | —      | Richiesta compilazione                          |

---

## 3. Controllo Genere
| ID  | Descrizione               | Input    | Output Atteso                                   |
|-----|---------------------------|----------|-------------------------------------------------|
| G1  | Selezione genere valido   | Maschio  | Accettato                                       |
| G2  | Selezione genere valido   | Femmina  | Accettato                                       |
| G3  | Selezione "Altro"         | Altro    | Accettato                                       |
| G4  | Nessuna selezione         | —        | Richiesta di selezionare un genere              |

---

## 4. Controllo Reset
| ID  | Descrizione                 | Azione      | Output Atteso                                   |
|-----|-----------------------------|-------------|-------------------------------------------------|
| R1  | Reset con campi compilati   | Click Reset | Tutti i campi tornano vuoti                     |
| R2  | Reset con campi vuoti       | Click Reset | Nessun errore, nessuna modifica                 |
| R3  | Reset dopo errore           | Click Reset | Errori rimossi, form pulito                     |

---

## 5. Controllo Caricamento Foto
| ID  | Descrizione                         | Input     | Output Atteso                                   |
|-----|-------------------------------------|-----------|-------------------------------------------------|
| F1  | Caricamento foto valida             | JPG 2MB   | Caricamento riuscito                            |
| F2  | File troppo grande                  | JPG 15MB  | Errore: dimensione non valida                   |
| F3  | Formato non supportato              | PDF       | Errore: formato non valido                      |
| F4  | Nessun file selezionato             | —         | Richiesta di selezionare un file                |
| F5  | Caricamento multiplo non consentito | 2 file    | Errore: caricamento multiplo non permesso       |

---

## 6. Controllo Funzionalità Donazione
| ID  | Descrizione                        | Input   | Output Atteso                                   |
|-----|------------------------------------|---------|-------------------------------------------------|
| D1  | Donazione con importo valido       | 10€     | Transazione accettata                           |
| D2  | Importo minimo                     | 1€      | Accettato                                       |
| D3  | Importo sotto il minimo            | 0.50€   | Errore: importo non valido                      |
| D4  | Importo non numerico               | abc     | Errore: input non valido                        |
| D5  | Metodo pagamento mancante          | —       | Richiesta selezione metodo                      |
| D6  | Donazione completata               | Dati OK | Conferma donazione                              |
| D7  | Donazione annullata                | Annulla | Nessuna transazione effettuata                  |
