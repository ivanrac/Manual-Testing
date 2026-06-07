# Test Cases

## TC-REG-001

**Názov:** Overenie dostupnosti tlačidla Registrácia

**Predpodmienky:**

* Domovská stránka Medirex je dostupná.
* Používateľ nie je prihlásený.

**Kroky:**

1. Otvor domovskú stránku Medirex.
2. Vyhľadaj tlačidlo alebo odkaz Registrácia.

**Očakávaný výsledok:**

* Tlačidlo Registrácia je zobrazené a dostupné používateľovi.

**Výsledok:**

* PASS

---

## TC-REG-002

**Názov:** Overenie presmerovania na registračnú stránku

**Predpodmienky:**

* Používateľ sa nachádza na domovskej stránke.

**Kroky:**

1. Klikni na tlačidlo Registrácia.

**Očakávaný výsledok:**

* Používateľ je presmerovaný na registračný formulár.

**Výsledok:**

* PASS

---

## TC-REG-003

**Názov:** Overenie správania formulára pri prázdnom e-maili

**Predpodmienky:**

* Používateľ sa nachádza na registračnej stránke.

**Kroky:**

1. Nechaj pole E-mail prázdne.
2. Pokús sa pokračovať v registrácii.

**Očakávaný výsledok:**

* Používateľ nemôže pokračovať v registrácii.
* Povinné pole E-mail musí byť vyplnené.

**Výsledok:**

* PASS

---

## TC-REG-004

**Názov:** Overenie validácie neplatného e-mailu

**Predpodmienky:**

* Používateľ sa nachádza na registračnej stránke.

**Kroky:**

1. Do poľa E-mail zadaj hodnotu `abc@`.
2. Klikni na Pokračovať.

**Očakávaný výsledok:**

* Formulár nepokračuje ďalej.
* Zobrazí sa chybová hláška o neplatnom formáte e-mailu.
* Pole bude označené ako neplatné.

**Výsledok:**

* PASS

---

## TC-REG-005

**Názov:** Overenie validácie platného e-mailu

**Predpodmienky:**

* Používateľ sa nachádza na registračnej stránke.

**Kroky:**

1. Do poľa E-mail zadaj platný e-mail.
2. Klikni na Pokračovať.

**Očakávaný výsledok:**

* E-mail je akceptovaný.
* Používateľ môže pokračovať na ďalší krok registrácie.

**Výsledok:**

* PASS

---

## TC-REG-006

**Názov:** Overenie minimálnej dĺžky mena

**Predpodmienky:**

* Používateľ sa nachádza v kroku Osobné údaje.

**Kroky:**

1. Do poľa Meno zadaj minimálny povolený počet znakov.
2. Opusť pole.

**Očakávaný výsledok:**

* Meno je akceptované.
* Pole je označené ako validné.

**Výsledok:**

* PASS

---

## TC-REG-007

**Názov:** Overenie maximálnej dĺžky mena

**Predpodmienky:**

* Používateľ sa nachádza v kroku Osobné údaje.

**Kroky:**

1. Do poľa Meno zadaj maximálny povolený počet znakov.
2. Opusť pole.

**Očakávaný výsledok:**

* Meno je akceptované.
* Pole je označené ako validné.

**Výsledok:**

* PASS

---

## TC-REG-008

**Názov:** Overenie prekročenia maximálnej dĺžky mena

**Predpodmienky:**

* Používateľ sa nachádza v kroku Osobné údaje.

**Kroky:**

1. Do poľa Meno zadaj viac znakov ako povoľuje limit.
2. Opusť pole.

**Očakávaný výsledok:**

* Zobrazí sa validácia.
* Používateľ je upozornený na prekročenie limitu.

**Výsledok:**

* PASS

---

## TC-REG-009

**Názov:** Overenie validácie priezviska s diakritikou

**Predpodmienky:**

* Používateľ sa nachádza v kroku Osobné údaje.

**Kroky:**

1. Do poľa Priezvisko zadaj hodnotu obsahujúcu diakritiku.
2. Opusť pole.

**Očakávaný výsledok:**

* Priezvisko je akceptované.
* Pole je označené ako validné.

**Výsledok:**

* PASS

---

## TC-REG-010

**Názov:** Overenie validácie neplatného rodného čísla

**Predpodmienky:**

* Používateľ sa nachádza v kroku Osobné údaje.

**Kroky:**

1. Do poľa Rodné číslo zadaj neplatnú hodnotu.
2. Opusť pole.

**Očakávaný výsledok:**

* Pole je označené ako neplatné.
* Zobrazí sa chybová hláška.

**Výsledok:**

* PASS

---

## TC-REG-011

**Názov:** Overenie prepnutia formulára pri voľbe bez rodného čísla

**Predpodmienky:**

* Používateľ sa nachádza v kroku Osobné údaje.

**Kroky:**

1. Zaškrtni možnosť „Nemám pridelené rodné číslo/identifikátor Slovenskou republikou“.

**Očakávaný výsledok:**

* Pole Rodné číslo je nahradené poľami Dátum narodenia a Číslo dokladu totožnosti.

**Výsledok:**

* PASS

---

## TC-REG-012

**Názov:** Overenie úspešného prechodu na ďalší krok registrácie

**Predpodmienky:**

* Všetky povinné údaje sú vyplnené správne.

**Kroky:**

1. Vyplň všetky povinné polia.
2. Klikni na tlačidlo Pokračovať.

**Očakávaný výsledok:**

* Používateľ je presmerovaný na ďalší krok registrácie.

**Výsledok:**

* PASS


