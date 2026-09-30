# NestJS Guards vs Interceptors

Guards decide if a request is allowed to proceed (auth/authorization) and run before the route handler; interceptors wrap the handler and can transform both the request and response, run before and after.
