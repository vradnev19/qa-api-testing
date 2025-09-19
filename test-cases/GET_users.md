# Test Case: GET /api/users?page=2

## Preconditions
- API: https://reqres.in

## Steps
1. Изпрати GET заявка към /api/users?page=2
2. Наблюдавай отговора

## Expected
- Status code = 200
- Response съдържа поле "data"
- "data" е масив с потребители
- Response time < 2000ms
