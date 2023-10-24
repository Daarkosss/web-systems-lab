1. **Walidacja formularzy**:
   - Walidacja formularzy to proces weryfikacji, czy dane wprowadzone przez użytkownika są poprawne zanim zostaną przesłane do serwera. Istnieją dwa główne typy walidacji: po stronie klienta (przeglądarki) i po stronie serwera.
   - **Walidacja po stronie klienta** jest przeprowadzana przez przeglądarkę przed wysłaniem formularza. Może być realizowana dzięki wbudowanym atrybutom HTML5, takim jak `required`, `pattern` czy typy `email`, `tel` itp.
   - **Walidacja po stronie serwera** jest niezbędna, ponieważ walidacja po stronie klienta może być pominięta (np. przez wyłączenie JavaScriptu) lub manipulowana przez użytkownika.
   - Nie wszystkie dane są automatycznie walidowane. Domyślna walidacja w przeglądarkach zachodzi tylko dla pewnych atrybutów lub typów pól input.
   - Aby wyłączyć automatyczną walidację formularza w HTML5, można dodać atrybut `novalidate` do tagu `<form>`. Na przykład: `<form novalidate>`.
   
2. **Typ elementu wejściowego `date`**:
   - Nie, element wejściowy o typie `date` nie jest wyświetlany tak samo we wszystkich przeglądarkach.
   - Większość nowoczesnych przeglądarek oferuje wybór daty za pomocą interfejsu kalendarza. Jednakże sposób wyświetlania tego kalendarza oraz jego funkcje mogą się różnić w zależności od przeglądarki.
   - W niektórych starszych przeglądarkach lub przeglądarkach, które nie obsługują tego typu, pole `date` będzie wyświetlane jako standardowe pole tekstowe.
   - Dlatego ważne jest, aby zawsze przeprowadzać testy we wszystkich głównych przeglądarkach, aby upewnić się, że formularze działają poprawnie.

3. **Atrybut `placeholder`**:
   - Atrybut `placeholder` określa krótki podpowiedź wyświetlaną w polu wejściowym, zanim użytkownik wprowadzi wartość.
   - Nie można go zastosować do wszystkich typów elementów wejściowych. Oto trzy typy, do których nie można zastosować atrybutu `placeholder`:
     1. `input` typu `file`
     2. `input` typu `radio`
     3. `input` typu `checkbox`
   - Ponadto, atrybut `placeholder` nie jest stosowany do elementów `<textarea>`, chociaż dla `<textarea>` jest on właściwie obsługiwany i często używany.