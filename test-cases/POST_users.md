# Test Case: POST /api/users

## Preconditions
- API: https://reqres.in

## Steps
1. Изпрати POST заявка към /api/users
   - Body:
     ```json
     {
       "name": "maria",
       "job": "tester"
     }
     ```

## Expected
- Status code = 201
- Response съдържа "id"
- Response съдържа "createdAt"

---

## Negative scenario
### Steps
1. Изпрати POST заявка към /api/users с празно body: `{}`

### Expected
- Очакван резултат: API може да върне 400 или 201 (поведението трябва да се документира)
