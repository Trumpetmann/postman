//Регистрируемся (Registration)
//POST https://blog.kata.academy/api/users
//Body:
{
  "user": {
    "username": "Stanislav",
    "email": "eyoemail@bk.com",
    "password": "gfhfgfhfgf"
  }
}
//Response:
{
  "user": {
      "username": "stanislav",
      "email": "eyoemail@bk.com",
      "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzE3ZGU2M2NmNzA1MWIwMDgyYTg2NiIsInVzZXJuYW1lIjoic3RhbmlzbGF2IiwiZXhwIjoxNjY5MzcxODc4LCJpYXQiOjE2NjQxODc4Nzh9.hdGqBMNLoJH-Llaim2cA29ug3VOVrxIIi8LMytkD2JY"
  }
}


//Логинимся (Authentication)
//POST https://blog.kata.academy/api/users/login
//Body: 
{
  "user": {
    "email": "eyoemail@bk.com",
    "password": "gfhfgfhfgf"
  }
}
//Response:
{
  "user": {
      "username": "stanislav",
      "email": "eyoemail@bk.com",
      "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzE3ZGU2M2NmNzA1MWIwMDgyYTg2NiIsInVzZXJuYW1lIjoic3RhbmlzbGF2IiwiZXhwIjoxNjY5MzcyMTYyLCJpYXQiOjE2NjQxODgxNjJ9.Jbz9sQT8mjC8oLeXOQXujOYaSw5a6Q6hm40JGxcXy0Q"
  }
}

//Получить данные текущего пользователя
//GET https://blog.kata.academy/api/user
//Headers: 
//Authorization: Token eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzE3ZGU2M2NmNzA1MWIwMDgyYTg2NiIsInVzZXJuYW1lIjoic3RhbmlzbGF2IiwiZXhwIjoxNjY5MzcxODc4LCJpYXQiOjE2NjQxODc4Nzh9.hdGqBMNLoJH-Llaim2cA29ug3VOVrxIIi8LMytkD2JY 
//Response:
{
  "user": {
      "username": "stanislav",
      "email": "eyoemail@bk.com",
      "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjYzMzE3ZGU2M2NmNzA1MWIwMDgyYTg2NiIsInVzZXJuYW1lIjoic3RhbmlzbGF2IiwiZXhwIjoxNjY5MzczNDc0LCJpYXQiOjE2NjQxODk0NzR9.8N8o81y0TvP-fbklMscFQQOzn1FSUMpdLwEvEm1ZqC8"
  }
}
