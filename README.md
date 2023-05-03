# Simple Books API
W niniejszym repozytorium przedstawiono [scenariusz testowy](https://github.com/MichalakMarta/Simple_Books_API/blob/main/Simple%20Books%20API%20Postman%20-%20scenariusz%20testowy.pdf) do wykonania testów API **Simple Books API** [link do api](https://simple-books-api.glitch.me), 
[dokumentacja](https://github.com/vdespa/introduction-to-postman-course/blob/main/simple-books-api.md)). 
Wyodrębnione zostały przypadki testowe poszczególnych endpointów. Do każdego przypadku testowego podane zostały:

1) nazwa testu,
2) warunki wstępne (jeśli występują),
3) kroki wykonania,
4) oczekiwany rezultat.

Przypadki testowe wprowadzono do programu Postman i udostępniono kolekcję w pliku o nazwie **Simple Books API.postman_collection.json**.

![alt text](/../main/collection%20preview.jpg?raw=true)


Do wykonania niektórych testów niezbędny jest **Bearer Token** wprowadzony w zakładce **Authorization**. Należy go uzyskać wysyłając request **Register API client**, zawarty w folderze **Authorization and register API client**.

![alt text](https://github.com/MichalakMarta/Simple_Books_API/blob/main/bearerToken.png)

Przypadki testowe zawierają również testy automatyczne sprawdzające status zwracanej odpowiedzi oraz poprawność zwracanych danych. W zależności od przypadku testowego, sprawdzeniu podlega typ zwracanych danych lub ich wartość. 

![alt text](https://github.com/MichalakMarta/Simple_Books_API/blob/main/listOfAllBooks.png)

Przypadek dotyczący rejestracji API klienta zawiera również zdefiniowane **pre-request Script**. Przed wysłaniem właściwego requestu losowane są dane dla **clientName** i **clientEmail**, w celu zaoszczędzenia czasu na ich manualne uzupełnianie, aby możliwe było ponowne wykonanie testu. 

![alt text](https://github.com/MichalakMarta/Simple_Books_API/blob/main/registerAPIClient.png)

Repozytorium zawiera również raport w html z przebiegu testów, do którego wykorzystany został **Newman**.

![alt text](https://github.com/MichalakMarta/Simple_Books_API/blob/main/newmanRaport.png)

