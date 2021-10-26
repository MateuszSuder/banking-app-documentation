# Auth
 *Metoda do walidowania JWT użytkownika uzyskanego w headerze (Authorization: Bearer JWT). Może zostać zaimplementowana jako Proxy, które zawsze sprawdza czy użytkownik ma prawa i do jakich kont ma dostęp (na podstawie ID użytkownika).*
 
##### Mając - JWT użytkownika
##### Kiedy - Użytkownik wykonuje zapytanie
##### Wtedy - Sprawdź poprawność JWT oraz zwróć do jakich kont (kont bankowych) użytkownik ma prawa.

Co można użyc:
* https://medium.com/trabe/validate-jwt-tokens-using-jwks-in-java-214f7014b5cf?
* Informacje o domenie podpisującej token (Auth0)!!!


 