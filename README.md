Chạy trên cổng 3001.

## Api

-   `[POST] /api/user/signup`: signup.
    -   body: {name: String, username: String, password: String, confirmPassword: String}.
    -   result: {status: String, message: String, data: {}}.
-   `[POST] /api/user/login`: login.
    -   body: {username: String, password: String}.
    -   result: {status: String, message: String,accessToken: String, refreshToken: String}.
-   `[POST] /api/user/logout`: logout.
    -   result: {status: String, message: String,}.
-   `[PUT] /api/user/updateUser/:id`: update User
    -   body: {data}.
    -   result: {status: String, message: String, data: {}}.
-   `[DELETE] /api/user/deleteUser/:id`: delete User
    -   result: {status: String, message: String}.
-   `[GET] api/user/getAllUser`: get All User
    -   result: {status: String, message: String, data: [{}]}.
-   `[GET] /api/user/getDetails/:id`: get Details User
    -   result: {status: String, message: String, data: {}}.
-   `[POST] api/user/refreshToken`: refresh Token
    -   result: {status: String, message: String, accessToken: String}.
