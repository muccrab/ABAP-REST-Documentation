# Smart Subrouter Class
Finds Best Matching Route.
Rules to finding a route:
>- The endpoint that is contained in URI is selected.
>- Every other value is then taken as a parameter to the last endpoint part.
>- If there are more endpoints that are contained in URI, the one that has parts sooner in URI is selected.
>- For instance if We have endpoints /ep1/ep2/ep3 and ep1/ep4/ep3 and URI ep1/value1/ep2/ep4/value2/value3/ep3, then the first one is selected.
With values ep1->value1, ep4->value2, ep4->value3
## Interfaces
[ZIF_REST_SUBROUTER](/interfaces/ZIF_REST_SUBROUTER)