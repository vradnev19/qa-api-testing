# 🐞 Bug Reports — Reqres.in API Testing

Този файл съдържа документирани бъгове/наблюдения, открити при тестовете с Postman и Newman.

---

## Bug 1: Unexpected 401 Unauthorized при `POST /api/users`

**ID:** BUG-001  
**Описание:**  
При изпълнение на заявка `POST https://reqres.in/api/users` с валидно JSON body  
(например `{"name": "maria", "job": "tester"}`) API връща **401 Unauthorized**, вместо очакван **201 Created**.

**Стъпки за възпроизвеждане:**
1. Изпрати `POST` заявка към `/api/users`  
2. Задай header: `Content-Type: application/json`  
3. Body:  
   ```json
   {
     "name": "maria",
     "job": "tester"
   }
