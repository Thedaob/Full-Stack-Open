# Full-Stack-Open
Par001
![image](https://github.com/Thedaob/Full-Stack-Open/assets/53585546/9f8e3832-2da2-4007-9b1b-8082069849f9)


  
actor Navegador
participant Servidor

Navegador -> Servidor: POST /new_note
Servidor --> Navegador: 302 Found\nLocation: /notes
Navegador -> Servidor: GET /notes
Servidor --> Navegador: 200 OK
Navegador -> Servidor: GET /main.css
Servidor --> Navegador: 200 OK
Navegador -> Servidor: GET /main.js
Servidor --> Navegador: 200 OK
Navegador -> Servidor: GET /data.json
Servidor --> Navegador: 200 OK

![image](https://github.com/Thedaob/Full-Stack-Open/assets/53585546/1e288957-1695-4847-8389-e86409bb6aae)



actor Navegador
participant Servidor

Navegador -> Servidor: POST /new_note_spa
note right of Navegador: Content-Type: application/json\n{ "content": "Contenido de la nota", "date": "2024-05-16T12:00:00Z" }
Servidor --> Navegador: 201 Created

![image](https://github.com/Thedaob/Full-Stack-Open/assets/53585546/46171fe4-2aa9-45a4-b465-bd5da5a77f3b)





